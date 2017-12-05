---
title: Electrical System
permalink: "/tech/electrical/"
layout: page
---

Electrical Parts:
* Arduino Uno microcontroller
* CNC stepper motor shield with DRV8825
* Nema 17 Stepper Motors (12V 0.4A)
* Servo motor - hobby grade

![block diagram]({{ site.baseurl }}/assets/images/electrical_block_diagram.png)

The Arduino receives instructions over serial, calculates the paths needed to move the steppers. It then runs the steppers until.

## Decisions:
We chose to use Nema 17 stepper motors because they are a good compromise between cost, size, and performance. The end-effector is not very heavy and with counterweights. We are pleased with the precision and speed of these motors.

We use a standard CNC stepper motor shield with DRV8825 stepper drivers. This is a standard way to drive stepper motors

A hobby grade servo is good enough for a tool changer that moves a delron pin and a small eraser.
