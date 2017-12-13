---
title: Mechanical
permalink: "/tech/mechanical/"
layout: page
---

## Basic Structure
During the first sprint we deliberate between multiple different system structures with the main changes between these design being the usage of the motors and how they related to position. Shown Below are the three versions we considered:

# Design A Two Motors
![Design A]({{ site.baseurl }}/assets/images/MVIMG_20171026_204224.jpg)
This is the design we eventually choose due to the simplicity and in comparison to our first pass version that utilized DC motors this part would more precise with the usage of Stepper motors.

# Design B Four Motor System
![MVIMG_20171026_210831.jpg](/uploads/MVIMG_20171026_210831.jpg)
This is the second design which is a variation of the first design with more motors. This version was scrapped for a more conservative pricing in addition to simplicity.

# Design C Gantry System
![MVIMG_20171026_211311.jpg](/uploads/MVIMG_20171026_211311.jpg)
This system was a very different system but with the success of the the first system in the first pass this system was not needed for the system. With one of our original goals being cross mounting and scaling the gantry system seemed less than ideal.

## Hardware parts
Our Mechanical System is composed of these parts based upon the design A above:
* Stepper Mount
* Tool Changer
* Micro controller Mount
* Belt system
* Counterweights

## Stepper Mount

This system is just a simple mount to allow the steppers to sty on the whiteboard and allow easy connections. The design was cut out in acrylic utilizing the the measurements from the steppers and whiteboard.

Need to request a better image.
![StepperMountClear.jpg](/uploads/StepperMountClear.jpg)


## Tool Changer
This system serves various purposes:
* Has a center of mass that allows for both the eraser and marker to make solid contact with the board
* Uses a hobby type dc motor to change between the eraser, marker, and movement positions
* Integrates with the belt system to move smoothly
* Connects to the Arudino system without the wiring interfering with movement.

This tool changer was again laser cut out of acrylic and then assembled with screws. Shown below is a top view of our tool changer:
![Toolchangertop.jpg](/uploads/Toolchangertop.jpg)

This is the neutral position of the tool that allows for the the marker to draw on the board.  The two "arms" can be rotated using the motor to a different position which will push the marker away from the board. Depending on the direction the arms are rotated this will put it in a move or erase mode. Shown below is a side view with a better view of the motor:

![Toolchangerside.jpg](/uploads/Toolchangerside.jpg)

## Micro Controller Mount

This mount is similar to the stepper mounts as its function is to attach to the top of the whiteboard and support its object. The Arudino held by this mounted needed the stable support in addition to access to the necessary ports for the steppers, tool, changer, power, and computer.








