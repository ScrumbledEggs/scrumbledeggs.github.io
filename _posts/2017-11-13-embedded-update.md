---
title: Embedded Update
date: 2017-11-13 17:27:26.577000000 Z
layout: post
author: adam
---

After lots of debugging the embedded code, it does the things we want it to do, and is in a pretty clean state.

## Decisions:
structs for position and lengths. `XY_Pos` and `LR_Step`. This helped me find at least one bug, and made the code much cleaner. I need to finish implementing the new structs in all of the functions

`XY_Pos` is given in mm from the top left corner. This is a change from setting an artboard with unitless dimensions and then converting to mm. The advantage was that I found the problem causing scaling issues, but I think it will be nicer to set the size and position of SVGs in mm units instead of useless 'artboard' units.


## Notes:
On the current scale that we are writing on, the lines are very sensitive to starting position. If the marker is off by a few cm, visible curving occurs. We will need to figure out a user-friendly calibration. Auto-calibration with limit switches on the steppers sounds promising, and would have 0 user calibration.

While the steppers are very precise, they cause the marker to swing quite a bit. Once we get the new stepper driver, I will add acceleration to the move_motors function. One problem I see is that we might have to look ahead multiple points to draw a smooth line - I do not want it to speed up and slow down every 2cm.
The other problem with the current stepper code is that, while the steppers end up at the right spots, they do not take a straight path to get there. This will be fixed with the new code by moving along the slope of the line instead of the current pathing.
