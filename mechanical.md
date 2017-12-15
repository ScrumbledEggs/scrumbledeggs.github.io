---
title: Mechanical
permalink: "/tech/mechanical/"
layout: page
---

## Basic Structure
We draw on the whiteboard by moving a tool carrier slung between two stepper motors, suspended via timing belts. This allows for very cheap and easy scalability compared to more traditional gantry systems. The only change when scaling up and down is different lengths of wire and timing belt.

## Hardware parts
Our Mechanical System is composed of 
* Stepper Mounts
* Tool Changer
* Microcontroller Mount
* Counterweights
* Timing Belts

### Stepper Mounts

These mount on the rail on top of the whiteboard. The steppers face inward, in order to have the belt as close to the surface of the whiteboard as possible. An idler facilitates full engagement of the timing belt on the driving pulley. NEMA 17 steppers are commonplace, and cheap due to widespread adoption.

![StepperMountClear.jpg](/uploads/StepperMountClear.jpg)


### Tool Changer
This assembly carries the marker, and a servo enables erasing, along with travel without drawing.


![Toolchangertop.jpg](/uploads/Toolchangertop.jpg)
> Tool changer: top view

This is the neutral position of the tool that allows for the the marker to draw on the board.  The two tools can be rotated using the servo to a forward position which will push the marker away from the board. Depending on the direction the arms are rotated this will put it in a move or erase mode.

![Toolchangerside.jpg](/uploads/Toolchangerside.jpg)
> Tool changer: side view

The long screws on the side of the tool changer serve as adjustable contact points for the belt. They contact area can be moved back and forth to compensate for the center of mass of the assembly, ensuring level hanging.

### Microcontroller Mount

Similar to the stepper mounts, provides an simple but stable attachment method for the Arduino and motor controller shield.

### Counterweights

We added adjustable counterweights to balance mass of the the tool changer, taking load off of the stepper motors. The counterweights use standard water bottles for cheap, continuous weight adjustment. They are affixed to the belts by an adjustable self-locking loop of timing belt.

### Timing belts
We use GT2 timing belts, again because of their widespread use in 3D printers. They do not stretch or slip, and are exceedingly easy to work with. 