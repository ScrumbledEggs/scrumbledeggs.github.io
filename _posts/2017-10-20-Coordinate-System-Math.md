---
title: Coordinate System Maths
date: 2017-10-20
layout: post
author: adam
---
The change-of-basis from cartesian coordinates to a two-string system turned out to be pretty simple.

We set the origin to be in the top left corner, with the y-axis extending in the positive direction downward. We chose this because the pen will never be above the motors, and it also makes the math much simpler. This also follows the SVG spec.

We ignore sagging and stretching in the cabling, because the error is small enough within the size that we draw on.

So, the left motor sits at `(0,0)`, and the right motor sits at `(width, 0)`. We use millimeter as our units everywhere because they provide enough precision, and it removes unit conversions.  

The lengths of cables can be calculated by drawing two circles centered on the motors to the pen. Their radius is the lengths.

[insert diagram here]
