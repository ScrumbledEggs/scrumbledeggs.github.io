---
title: Sprint 1
layout: page
---

#### What we did in Sprint 1:

* Decided on this project
* Spun up team:
  * Set up team communication channels
  * Set up software and mechanical design toolchains
  * Decided on design practices
  * Discussed expectations, roles, and team dynamics
* Made a proof of concept using DC motors and hot glued string
* Calculated the [change-of-basis math]({{ site.baseurl }}/2017/10/20/Coordinate-System-Math.html)
* Upgraded the proof of concept with 3D printed parts

## Current Status:
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/lc2-iXFGe7M?rel=0" frameborder="0" allowfullscreen></iframe>

![sprint1 deliverable]({{ site.baseurl }}/assets/images/sprint1system.png)
> The sprint 1 sysem. Draws hardcoded points using dc motors and timing
>

![marker collets]({{ site.baseurl }}/assets/images/sprint1marker.jpg)

> A close up of the marker with 3D printed collets

![dc motor]({{ site.baseurl }}/assets/images/sprint1motor.jpg)

## What we learned:
* Proof of concept works
* DC motors are not precise enough

## Risks:
* Ink is too light, need more pressure on pen
* Need to design a tool changer (draw/erase/move)
* Uncertain about precision of positioning
* SVG Computer Vision processing
  * We have a working manual toolchain, automation would be nice
* Stepper motors
  * Speed and torque uncertain

## Future Considerations:
* Possibly build a CNC gantry
  * High precision at the loss of simplicity
  * No sway on the pen
* Tool changer
  * Servo with many tools on its end
    * + Compact
    * - Not versatile (limited number of tools)
  * Solenoids
    * + More extendable with number of tools
    * - Too much force? (Breaking pen tips, bouncing off the wall)
    * - High current (cannot make wireless/battery powered)

## Next Sprint Deliverables:
* Implement stepper motors
* Have a better cable/string system
* Tool changer (end effector) with pen/erase/move
* Draw vector graphics from a computer
