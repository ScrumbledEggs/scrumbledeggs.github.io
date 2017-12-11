---
title: Sprint 3
author: Ian
layout: page
---

## What We Did in Sprint 3

* Made SVG toolchain.
* Implemented better stepper motor driver.
  * DRV8825
* Calibrated positioning
* Belts
* Added eraser to end-effector

## Current Status

(Here)[https://drive.google.com/file/d/1BGX7SfhieQuRmbrAQXPJCnek5YCE_1QQ/view?usp=sharing] is a video of the robot.

(Here)[https://docs.google.com/presentation/d/1plyTCBBu1P18bXn1_NWeWUgOcgUoGsLP4vZLkrV1ub0/edit?usp=sharing] are our slides from our sprint 3 review.

## Reframing

We changed some of our end goals in sprint 3. We've removed wireless communication as a goal; it seemed to be significantly harder than wired communication, required several more components, and wouldn't provide all that much extra functionality. One thing we decided to focus more on was cost. We used less than half our budget up until this point so we decided to make that a selling point and build a second Boardbot for documentation purposes. Finally we decided not to build a system for capturing whiteboards, that wasn't in line with any of our learning goals so we cut that from our stretch goals. 

## Previous Risks

### Wireless

Last sprint we were concerned about some of our wires and considered going wireless. We found in this sprint that there weren't any issues caused by having wires so we decided not to go wireless. For our final Boardbot we decided to build nice wiring harnesses so that the wires are easy to attach.

### Scaling

We wanted to make sure that the drawing area on the whiteboard was sufficient, since we'd only been testing and demoing on a small area. For this sprint we got it so that we could draw on almost all of the area inside our motors. 

### Computer Vision

Last sprint we listed doing the computer vision to capture a whiteboard as a risk. This sprint we've addressed this risk by cutting this out from our final deliverable. Building this system isn't in line with anyone's learning goals and it would take away from our other goals if we focused on this.

### Dropping Quality for Quantity

We were concerned that we had a lot of features we could build and by focusing on those it would reduce the quality of the features we needed to build. By having clear goals and assigning people tasks relevant to the core of the system we addressed this risk. We kept 2 people assigned primarily to documentation and management roles so that these would remain priorities as we closed in on the deadline.

## Detailed updates

### End effector

![tool selector]({{ site.baseurl }}/assets/images/toolselector.jpg)

We have all 3 modes available on our marker now. The servo can either let the marker draw on the board, put an eraser tip down to erase, or put a delrin tip down to move without writing or erasing.

### Driver

![driver]({{ site.baseurl }}/assets/images/driver.jpeg)

We've installed the new motor driver for this sprint and it drives well. It mounts nicely with the Arduino.

### New mounts

![new mount]({{ site.baseurl }}/assets/images/newmount.jpeg)

We built new motor mounts that place them closer to the board. This helps put pressure on the pen so our lines are clean.

### Counterweights

![counterweight]({{ site.baseurl }}/assets/images/counterweight.jpeg)

We've installed counterweights to help the steppers move accurately and without strain.

## Risks

* Using SVGs is still hard. The code to draw from SVGs works but it's slow and the Arduino resets frequently during communication. This is something we'd like fixed by demo day.

* Some parts of our mechanical system are still a little kludgy, to make this easily reproducible we'd need to fix these aspects.

* We haven't done too much planning on what a cross whiteboard mounting system would look like. If we want to include this for demo day it would require time to both design it and fabricate it. 

* Having too many goals. There are a lot of things that different people want to accomplish before demo day; we need to make sure we don't overscope. 