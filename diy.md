---
title: Make Your Own
link: "/diy/"
layout: page
---

With a budget of less than $250, you too can build your own BoardBot. With open source CAD and and code, you can remix your BoardBot to fit your exact needs.


#### BOM


| Name | Description | Cost (USD) | Source |
| ---  |: ----------- :| ----- :|
| Acrylic | Approximately 12"x24" | 15 | [Buy](https://www.mcmaster.com/#8505k742/=1ajxsgv)|
| Stepper Motors | Two Nema 17 Bipolar | 2x 10 | [Buy](https://www.amazon.com/gp/product/B00PNEQCLO/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1) |
| Stepper Motor Driver | CNC shield with 4x DRV8825 | 15 | [Buy](https://smile.amazon.com/gp/product/B06Y5SS2W9/ref=od_aui_detailpages00?ie=UTF8&psc=1)|
| Arduino Uno | | 10 | [Buy](https://smile.amazon.com/gp/product/B01AR7YJ3O/ref=od_aui_detailpages00?ie=UTF8&psc=1) |
| Servo | Standard hobby grade | 10 | [Buy](https://smile.amazon.com/Hitec-RCD-USA-31422-Standard/dp/B00B88FIZ0/ref=sr_1_2?s=industrial&ie=UTF8&qid=1512752431&sr=1-2&keywords=hobby+servo) |
| USB Cable | 10ft Type A to B | 5 | [Buy](https://smile.amazon.com/gp/product/B00NH13DV2/ref=od_aui_detailpages00?ie=UTF8&psc=1) |
| Timing belt and Pulleys | 10m GT2 belt, 2x pulleys | 10 | [Buy](https://www.amazon.com/BIQU-Meters-Timing-20Teeth-Printer/dp/B01GTGOD6U/ref=sr_1_8?ie=UTF8&qid=1510678841&sr=8-8&keywords=5mm+bore+timing) |
| Idlers | 2x Idlers| 5 | [Buy](https://www.amazon.com/BIQU-Aluminum-Toothless-Timing-Printer/dp/B01H3F8LUU/ref=sr_1_4?s=industrial&ie=UTF8&qid=1510679336&sr=1-4&keywords=6mm+belt+width+idler&dpID=419EDxynYwL&preST=_SX342_QL70_&dpSrc=srch) |
| General Screws | #6-32 1/2" (>20 count) | 3 | [Buy](https://www.mcmaster.com/#91249A148) |
| Nuts | Square #6-32 (>20 count) | 3 | † [Buy](https://www.mcmaster.com/#94855A115) |
| Washers | #6 (>20 count) | 1 | † [Buy](https://www.mcmaster.com/#92141A008) |
| Metric Screws | Two m5x30mm | 1 | † [Buy](https://www.mcmaster.com/#91502a150/=1alhs37) |
| Metric Nuts | Two m5 | 1 | † [Buy](https://www.mcmaster.com/#93187a200/=1alhrm1) |
| Long screws | Two #6-32 x 2" | 1 | † [Buy](https://www.mcmaster.com/#92949A817) |
| == | == | == | == |
| | **Total** | 90 | |

† indicates brick and mortar purchase recommended, for cheaper low-volume pricing.





Our mechanical design is [available on Onshape](https://cad.onshape.com/documents/8f08652983ca17f06e9ac67d/w/e174f06e8eb73e105045d519/e/7b27395932c9fa97ee45a030).

Our software is [available on GitHub](https://github.com/ScrumbledEggs/PoE).

## Build Instructions:

### Laser Cutting
For laser cutting fabrication, you will need:
- 12"x24" 1/8" Acrylic sheet
- Laser Cutter (Capable of cutting acrylic)

A cut sheet is available [Here](https://cad.onshape.com/documents/8f08652983ca17f06e9ac67d/v/2d1037471e8f919848eb07d1/e/9d0991215f774ad617620235):

Download sheet as whatever format is convenient for your Laser Cutting toolchain, and cut all paths.




### Stepper Mount

#### Chassis
For each stepper mount, you will need:
- 10x #6-32 1/2" screws
- 10x #6-32 square nuts
- 10x #6 washers
- 2x side panels
- Mount panel
- Top panel
- Phillips Screwdriver

Take care to reverse the chirality of the mount panel for the second stepper mount.

#### Hardware
For each stepper mount, you will need:
- NEMA 17 stepper motor
- 4x M3-8mm screws
- 4x M3 washers
- M5-30mm screw
- M5 nut
- M5-10mm spacer
- M2 hex key
- M2.5 hex key
- M4 hex key

Take care to align the direction of the wire exit from the motor with the direction of the idler pulley.


### Tool Changer

#### Chassis

For the Tool Changer, you will need:
- 7x #6-32 1/2" screws
- 15x #6-32 square nuts
- 7x #6 washers
- 2x #6-32 2" screws
- 4x #8-32 screws
- 4x #8-32 square nuts
- Base plate
- End plate
- Mid plate
- Front plate
- Top plate
- Side plate
- Whiteboard marker
- Hobby servo
- Phillips screwdriver

First, uncap the pen, insert through the mid plate and front plate, then recap.

Next, install the servo in the base plate with the #8 fasteners

Assemble the rest of the chassis, taking care that all the side plate notches are on the same side.

Run the 2" #6 screws through the sides of the tool changer, adding 4 nuts in the middle of the screw. These will serve as the adjustable contact point for the belts.

##### End Effector

For the End Effector, you will need:
- Assembled Tool Changer Chassis
- 4-way servo horn
- Servo horn screw
- 1" pin
- Marker with eraser cap
- Hot glue gun
- Cutting Tool

First, cut two of the lobes off of the servo horn.

Next, hot glue the pin and the marker cap to the remaining two lobes

Finally, install the servo horn on the Tool Changer Chassis.

### Microcontroller Mount

For the microcontroller you will need:
- Arduino Uno compatible microcontroller
- 4x #6-32 1/2" screws
- 4x #6-32 square nuts
- 4x #6 washers
- 4x #4-32 3/4" screws
- 4x #4-32 nuts
- 4x #4 washers
- 12x #4 1/8" spacers
- Base plate
- Side plate
- Side plate w/ cutout
- Phillips screwdriver

First, assemble the microcontroller mount chassis.

Then, Mount the arduino with the #4 hardware, with one spacer on top and two spacers underneath each mount hole.






