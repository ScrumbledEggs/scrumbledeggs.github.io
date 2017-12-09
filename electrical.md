---
title: Electrical System
permalink: "/tech/electrical/"
layout: page
---

Electrical Parts:
* Arduino Uno microcontroller
* CNC stepper motor shield with DRV8825 stepper motor drivers
* Nema 17 Stepper Motors (12V 0.4A)
* Servo motor - hobby grade

![block diagram]({{ site.baseurl }}/assets/images/electrical_block_diagram.png)

The Arduino receives instructions from a computer over serial.
It drives the steppers with a CNC stepper motor shield with DRV8825 stepper motor drivers.


## Decisions:
We chose to use **Nema 17 stepper motors** because they are a good compromise between cost, size, and performance. The end-effector is not very heavy, and with counterweights the motors zoom it around the board with ease. We are pleased with the precision and speed of these motors.

We use a standard CNC stepper motor shield with DRV8825 stepper drivers. This is a standard way to drive stepper motors. The DRV8825 is controlled with two pins, one is used to indicate direction, the other triggers a step.

You can read more about the stepper motors and shield [here]({{ site.baseurl }}/2017/11/17/Stepper-Driver-Update.html).

A hobby grade servo is good enough for our tool changer. We control it using PWM.
