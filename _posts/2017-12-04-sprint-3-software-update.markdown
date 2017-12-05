---
title: Sprint 3 Software Update
date: 2017-12-04 20:35:00 Z
---

# Current State

Right now the software has met our MVP. This is a non-trivial achievement, as least from my perspective, since serial communication is hard to do properly. Right now we can:
* Draw a line from one point to another
* Move from one point to another
* Erase between 2 points
* Convert an arbitrary SVG to points
* Send those points to the Arduino

## How to use

Currently this is all doable, but not in the easiest to use state. The code on the Arduino is simple enough, just reset the chip and connect your laptop over USB. From your laptop, define the file you want to send in the Python file and run that. 

# Technical Details

## How it should work

Python starts by reading in an SVG file which is encoding in XML. It parses the XML into SVG objects which exposes the underlying lines. The script then iterates through the lines and turns them into points to send to Arduino over serial. For lines it only looks at the end points, but for curves it breaks them into several points so that they appear smoother.

The points are sent using a 4 phase handshake to ensure that every point is sent and to give the motors time to draw them. Aruindo takes each point and moves to it. There are defined points with impossible (negative) values that send signals for marker down, marker up, and eraser down. 

The motors are run with constant acceleration which drives them really well close to the center of the board, but it struggles around the edges.

## How it ends up working

The handshaking ends up doing a lions share of the work here. Our Arduino(s) all had some unfortunate consistency problems. They had some serial communication issues where they wouldn't exactly get the data that python sends. I don't have an complete answer as to why this happened, but some theories involve flushing data at the wrong times or possibly don't reading at the wrong time (reading after any amount of bits are in the channel rather than reading the exact length of what I need bit by bit). One other issue is that any Arduino we tested reset in the middle of communication. This significantly slowed down data transmissions, however the handshaking protocol was resilient enough to account for this. I have no idea what caused this, but changing some bits and pieces of the code, in particular how it manages memory will hopefully fix it. 

# Next Steps

Code has grown from being a couple of simple scripts to approaching a finite state machine. Going forward, I'm going to implement the transmission protocol as an FSM and offload more of the processing to the Python side of the code. The Arduino should only be running the motors. 