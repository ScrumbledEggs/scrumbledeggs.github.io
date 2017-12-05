---
title: Software Status Sprint 2
date: 2017-11-14 17:27:00 Z
author: evan
layout: post
---

# Status
We can parse SVGs with lines and quadratic Beziers. Additionally, using the Arduino Motor shield we can drive our steppers using some handwritten interleaving code.

Transmission is a little shaky, but that wasn't the focus of our software team this sprint. 

SVG parsing is working at a really good level and the code is very extensible. 

The Arduino stepper motor driver is a bit of sticking point. Right now, it's not possible to drive both motors at the same time. We resolve this by interleaving steps - driving one motor for a few steps, then driving the other for a few steps. This works for drawing lines from one point to another but they end up looking a little jittery. This isn't a limit of the software, but a fundamental limit of the hardware. Going forward we'll work with Stan's motor shield to fix these problems. 