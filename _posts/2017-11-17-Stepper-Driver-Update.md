---
title: Stepper Driver Update
date: 2017-11-17 17:27:26.577000000 Z
layout: post
author: adam
---

I talked to Stan today about what steps to do to implement the new stepper driver:

Our steppers are Nema 17s, (17hs15-0404s). They are spec'ed for 12V, 0.4A.

1. Set the current limit on the DRV8825 to the maximum stepper current. (0.4A)
2. Power the drivers with 24v. This will charge the inductors faster, and then the current limiting will kick in, keeping the steppers from burning out.
3. Set microstepping with jumpers on the m0,m1,m2 pins. Higher micorstepping does higher fidelity in exchange for lower torque and speed. Our physical gearing is already fine, so we will start with full steps and go lower if needed.

Stan's library looks fully featured for what we need, and the initial software implementation appears to be straightforward. In the future, I want to have more intelligent decisions on velocity by looking ahead one or more points, and not needing to stop after each line.