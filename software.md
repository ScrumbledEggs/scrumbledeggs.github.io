---
title: Software
permalink: "/tech/software/"
Author: Ian
layout: page
---

# Software

## SVG Parsing
To parse SVGs we use the svgpathtools python library and the xlm library to get the SVG data our of .svg files. With these libraries we go through each path defined in an svg file and break it into points. For straight lines we grab just the end points and for curves we grab a few points (8) along it. We scale each point from the scale of the svg file to our board size (soon to be a variable scale) and send it to the Arduino. Each path is passed in a handshake (Python sends the point one way, Arduino sends them back to confirm everything worked) and we wait for Arduino to finish a path before we send the next one.

# Firmware

## Programming the Arduino

We used a piece of software called PlatformIO to program our microcontroller. We choose PlatformIO because it had a nice command line interface and let us use our own text editors instead of the Arduino IDE. It didn't cost us any features as it has a built in serial monitor. 

## Arduino Code

### Communications

We used Arduino's serial module to communicate with our computers and the Python script. When data was available on the serial channel we'd read in 4 bytes from the serial buffer convert that to an long integer. To get a point we'd do this twice and put them into a struct of two longs. Communication was handled in terms of paths, so as Python sent points in a path, Arduino would get each point one by one and send it back to Python to confirm that it received the correct data.

### Motor Control

Our motor code is abstracted to setting marker positions as XY coordinates (with the top left being 0,0). From there we transform the XY positions (measured in mm) into lengths for the left and right spools. The lengths that the spools need to be are compared with their current lengths. Their speeds are set based on the max speed and the distance they need to go, this keeps the lines relatively straight and even.