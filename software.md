---
title: Software
permalink: "/tech/software/"
layout: page
---

## SVG Parsing
To parse SVGs we use the svgpathtools python library and the xlm library to get the SVG data our of .svg files. With these libraries we go through each path defined in an svg file and break it into points. For straight lines we grab just the end points and for curves we grab a few points (8) along it. We scale each point from the scale of the svg file to our board size (soon to be a variable scale) and send it to the Arduino. Each path is passed in a handshake (Python sends the point one way, Arduino sends them back to confirm everything worked) and we wait for Arduino to finish a path before we send the next one.