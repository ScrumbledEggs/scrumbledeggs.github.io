---
title: Mechanical Update 17/11/17
date: 2017-11-17 20:18:00 Z
categories:
- Mechancial
tags:
- Mechanical
- Update
---


![MVIMG_20171117_152858.jpg]({{ site.baseurl }}/uploads/MVIMG_20171117_152858.jpg)

This sprint, we transitioned from spooling twine to timing belts and pulleys for our control arms. This decision comes with several advantages:

* Fiber reinforced urethane timing belts do not stretch, compared with twine
* Tooth engagement leads to zero slip between belt and pulley
* Set screws onto the D-shaft lead to zero slip between the pulleys and motors
* Timing belts lock when folded over, creating an easy length adjustment mechanism

Our pulley has a smaller OD than our spools, leading to less distance traveled per step. This should assist with line resolution, but at the cost of drawing speed. Hopefully, our new stepper driver board allows us to both step faster and microstep if we need more resolution, mitigating the issue.

Our stepper mount design now incorporates an idler pulley as well, to keep the timing belt engaged even at high angles. Currently, this is fastened to the mount with dual M5 screws self tapped into a 3/16ths nylon spacer, which works admirably, but is not a good long term solution.

Other additions include a new top bracing plate to the stepper mounts (to assist with rigidity) and mounting the stepper motors on the other side of the plate. This puts the belt as close to the whiteboard as possible, which in turn allows us to shorten our tool changer, with the eventual goal of less sway in the pen lines.

This update's CAD is available [here](https://cad.onshape.com/documents/8f08652983ca17f06e9ac67d/v/082bedbad80e068208d81686/e/88465677413e52a9af015cfc):
