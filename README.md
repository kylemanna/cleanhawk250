# CleanHawk 250 Power Distribution Board

This document outlines the basic tasks to get the CleanHawk 250 Power Distribution Board (PDB) up and flying.


## Overview

The goal of the CleanHawk 250 PDB is to simplify wiring and imporve integration and reliability.  The printed circuit board replaces the bottom carbon fiber frame support on the Emax 250 / Nighthawk 250.

### Buy It Now

* [MassiveRC](http://bit.ly/1aG1E3O)
* Tindie

### Features

* 3-4S compatible
* Designed for KISS 18A ESCs, ReadyToFly/Witespy's BearHug should fit just fine, and have pads for traditional ESCs. Hoping that the new Emax BLHeli Oneshot ESCs fit.
* 3A @ 5V for flight computer, OSD, and LEDs (i.e. WS2812), telemetry/BT, etc. (85%+ efficient).
* 3A @ 9V for FPV camera, vtx, and LEDs. (92%+ efficient),
* (6) RGB LEDs. 4 on bottom, 2 on top (not sure if top will be useful). Testing waters here. User configurable color by changing resistors. Plan is to do red on the rear and white up front.
* FPV LC filter that can select between 9V or 5V for feeding cameras and FPV transmittter,
* Multiple soldering points for accessories on the VBAT, 9V, and 5V rail. Helps to contain the wiring mess.
* Battery voltage divider for dividing the voltage down to something manageable for the Frsky D4R-II.
* Optional bulk capacitance near the ESCs to help smooth out ripples.
* Centralized battery input pads to keep the high current paths through the board as short as possible
* 2oz copper for efficiency
* Sufficient copper keep out area surrounding the mounting holes
* Shielded inductors to reduce switching power supply noise.

### What's Included

* (1) CleanHawk 250 Power Distribution Board with all surface mount components installed.
* (1) 1x4 pin header for the auxilliary port
* (1) 1x6 pin header for the ESC and flight controller port
* (3) 2x2 pin header for respective power supply outputs (5V, 9V, Filtered)

### Recommended Additional Components

#### Wire Extension Cables

It is recommended to use Dupont female to female cable connectors to wire the PDB to the receiver and flight controller. Available on [Amazon](http://amzn.com/B00KOL5BCC) in 10cm length. ![Dupont cables](http://i.imgur.com/sG2cDaPm.jpg)  An alternative to these are male to male servo extension headers such as [these from Amazon](http://amzn.com/B00FGLSTY2).  ![Servo extension](http://i.imgur.com/mOOl1RLm.jpg)

#### Angled Pin Headers

Consider picking up 90 degree angled pin headers if mounting KISS ESCs or if the front/rear pin headers for LEDs are more useful angled.

#### Electrical Tape

Electrical tape is a critical requirement to insulate parts mounted on the PCB (i.e. KISS ESCs) to prevent wearing through the solder mask.

#### Cable Ties

Who doesn't have these?  Strap down wires or ESCs to secure them.


## Quick Start Guide

### Step 1 -- Install Pin Headers

### Step 2 -- Configure LC Filter and FPV Gear

### Step 3 -- Install ESCs

### Step 4 -- Install on Quadcopter


## Known Issues

* 5V and GND silkscreen labels flipped on first build, but copper traces are correct. Refer to images or verify with multipmeter before powering flight controller.
* QR code placement is a little off and leads to now [defunct bit.ly bundle](http://bitly.is/1aG0YLU).  Thanks bit.ly!  I'd be nice if I could change the destination URL to the Github page instead.


## Additional Reading

* [RC Groups Forum Thread](http://bit.ly/1aFZpxj)
* [Hackaday Project Page and Build Log](http://bit.ly/1aG09m9)
* [Imgur Image Gallery](http://bit.ly/1aG00z3)
