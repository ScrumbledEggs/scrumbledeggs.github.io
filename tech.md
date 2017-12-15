---
title: Tech
permalink: "/tech/"
layout: page
---

BoardBot is an integrated system of _nontrivial_ **Mechanical**, **Electrical**, and **Software** components.

## Read more about each subsystem:

- [Mechanical]({{ site.baseurl }}{% link mechanical.md %})
- [Electrical]({{ site.baseurl }}{% link electrical.md %})
- [Software]({{ site.baseurl }}{% link software.md %})


## Overview of the system
![system diagram](http://www.relatably.com%2Fm%2Fimg%2Fdoge-meme-gif-imgur%2F3U9oYna.jpg)

SVG images are processed in Python and sent to an arduino via USB serial. The arduino converts points to belt lengths. Using a non-proprietary control algorithm, it drives the motors to the desired positions using DRV8825 stepper motor drivers. The arduino controls the tool changer servo with PWM.
