---
title: Sprint 2
layout: page
---

## What we did in Sprint 2:
* Integrated stepper motors
* Started processing SVGs
* Made lower-quality drawings because of the stepper driver and library
  *  Adafruit stepper driver communicates over I2C, so it is slow for 1000s of steps
* Made end-effector with move and draw (not erase)
* Started working on this website

## Current status:
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/gN-Lxg4stGI?rel=0" frameborder="0" allowfullscreen></iframe>


## Design Decisions:
Keeping constant pressure on pen is important for rich color lines. We built an end-effector that is heavier, and this has given us enough force.

Stepper motors were the logical next step for the Main actuators. We kept using the Adafruit shield but it held our control algorithms back and the switch felt like a step back. The lines were jagged, and drawing was slow.


## Future Work:
* Swapping in DRV8825 stepper motor drivers
  * Desperately needed for functional motor control
* Wireless communications to end effector?
  * The hanging wire to the servo is a hazard
  * We are considering making it wireless, with its own microcontroller, battery, and wireless communication
* Do scaling testing
  * Whiteboards are big, and we want to be able to draw on them completely
* Add eraser to the tool changer
