---
title: Mechanical
permalink: "/tech/mechanical/"
layout: page
---

## Basic Structure
During the first sprint we deliberate between multiple different system structures with the main changes between these design being the usage of the motors and how they related to position. Below are the three versions we considered:

#### Design A Two Motors
![Design A]({{ site.baseurl }}/assets/images/MVIMG_20171026_204224.jpg)
This is the design we choose due to ease of setup and control.

#### Design B Four Motor System
![MVIMG_20171026_210831.jpg](/uploads/MVIMG_20171026_210831.jpg)
This is the second design which is a variation of the first design with more motors. This version was scrapped for a more conservative pricing in addition to simplicity.

#### Design C Gantry System
![MVIMG_20171026_211311.jpg](/uploads/MVIMG_20171026_211311.jpg)
This system was a very different system. We considered it if we needed more precision than the two cable system could provide, but our Design A proof of concept was functional. The gantry system did not fulfill our goals for cross-whiteboard mounting and scaling.

## Hardware parts
Our Mechanical System is composed of these parts based upon the design A above:
* Stepper Mount
* Tool Changer
* Micro controller Mount
* Belt system
* Counterweights

### Stepper Mount

This system is just a simple mount to allow the steppers to hang on the whiteboard and allow easy setup.

![StepperMountClear.jpg](/uploads/StepperMountClear.jpg)


## Tool Changer
This system serves various purposes:
* Has a center of mass that allows for both the eraser and marker to make solid contact with the board
* Uses a hobby dc motor to change between the eraser, marker, and movement positions
* Integrates with the belt system
* Connects to the Arudino system without the wiring interfering with movement.


![Toolchangertop.jpg](/uploads/Toolchangertop.jpg)
> Tool changer: top view

This is the neutral position of the tool that allows for the the marker to draw on the board.  The two "arms" can be rotated using the motor to a different position which will push the marker away from the board. Depending on the direction the arms are rotated this will put it in a move or erase mode.

![Toolchangerside.jpg](/uploads/Toolchangerside.jpg)
> Tool changer: side view
