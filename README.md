# CleanHawk 250 Power Distribution Board

This document outlines the basic tasks to get the CleanHawk 250 Power Distribution Board (PDB) up and flying.

**Documentation can be found at the [CleanHawk250 GitHub repository](https://github.com/kylemanna/cleanhawk250).**


## Overview

The goal of the CleanHawk 250 PDB is to simplify wiring and imporve integration and reliability.  The printed circuit board replaces the bottom carbon fiber frame support on the Emax 250 / Nighthawk 250.

### Buy It Now

* [MassiveRC](http://bit.ly/1aG1E3O)
* Tindie

### Features

* **3-4S compatible**
* Designed for **KISS 18A ESCs**, ReadyToFly/Witespy's BearHug should fit just fine, and have pads for traditional ESCs. Hoping that the new Emax BLHeli Oneshot ESCs fit.
* **3A @ 5V** for flight computer, OSD, and LEDs (i.e. WS2812), telemetry/BT, etc. (85%+ efficient).
* **3A @ 9V** for FPV camera, vtx, and LEDs. (92%+ efficient),
* **(6) RGB LEDs**. 4 on bottom, 2 on top (not sure if top will be useful). Testing waters here. User configurable color by changing resistors. Plan is to do red on the rear and white up front.
* **FPV LC filter** that can select between 9V or 5V for feeding cameras and FPV transmittter,
* Multiple soldering points for accessories on the VBAT, 9V, and 5V rail. Helps to contain the wiring mess.
* **Battery voltage divider** for dividing the voltage down to something manageable for the Frsky D4R-II.
* Optional bulk capacitance near the ESCs to help smooth out ripples.
* Centralized battery input pads to keep the high current paths through the board as short as possible
* **2oz copper** for efficiency and electroless nickel immersion gold plating for solderability.
* Sufficient copper keep out area surrounding the mounting holes
* Shielded inductors to reduce switching power supply noise.

### What's Included

* (1) CleanHawk 250 Power Distribution Board with all surface mount components installed.
* (1) 1x4 pin header for the auxilliary port
* (1) 1x6 pin header for the ESC and flight controller port
* (3) 2x2 pin header for respective power supply outputs (5V, 9V, Filtered)

### Recommended Additional Components

#### Wire Extension Cables

It is recommended to use Dupont female to female cable connectors to wire the PDB to the receiver and flight controller. Available on [Amazon in 10cm length](http://amzn.com/B00KOL5BCC).

![Dupont cables](http://i.imgur.com/sG2cDaPm.jpg)

An alternative to these are male to male servo extension headers such as [these from Amazon](http://amzn.com/B00FGLSTY2).

![Servo extension](http://i.imgur.com/mOOl1RLm.jpg)

#### Angled Pin Headers

Consider picking up 90 degree angled pin headers if mounting KISS ESCs or if the front/rear pin headers for LEDs are more useful angled.

#### Electrical Tape

Electrical tape is a critical requirement to insulate parts mounted on the PCB (i.e. KISS ESCs) to prevent wearing through the solder mask.  I stick to [3M Super33](http://amzn.com/B00004WCCL).

#### Cable Ties

Who doesn't have these?  Strap down wires or ESCs to secure them.


## Quick Start Guide

### Step 1 -- Install Pin Headers and Battery Cables

The `P9` header is critical for flight and should be installed first.  All other headers are optional and pilots should refer to the [pin headers documentation](PinHeaders.md) for more details.

Verify that the Dupont cables or servo extensions are available to connect `P9` to the flight controller.

Battery wires up to 12 AWG are installed to the large through hole pads in the center of the board.  Due to the massive copper area surrounding the pads to transfer large amounts of current to the ESCs, **a large amount of heat is necessary to heat this area**.  *Turn the soldering iron up, feed solder to help transfer heat, and be patient.*

### Step 2 -- Configure LC Filter and FPV Gear

The LC filter should be bridged to the 9V side for most FPV gear.  Verify this is valid for your gear and modify `JP1` if needed.  More details in the [pin headers documentation](PinHeaders.md).

### Step 3 -- Install ESCs

Mount the ESCs to the board with **some insulation such as heat shrink or 3M Super33 to avoid shorts** that could occur should they wear through the black solder mask.  More details in the [ESC documentation](ESCs.md).

### Step 4 -- Install on Quadcopter

Install the board in place of the bottom carbon fiber plate.  Verify that all screws and hardware fit in the designated area and aren't rubbing on the PDB. Note that there are recesses on the board around all mounting holes where copper has been removed to prevent issues.  **Failure to remove any objects that are touching the PDB could damage the PDB and cause a short and in extreme cases a fire.** Don't be on the news or YouTube with a flaming CleanHawk quad copter!

## Known Issues

* 5V and GND silkscreen labels flipped on first build, but copper traces are correct. Refer to images or verify with multipmeter before powering flight controller.
* QR code placement is a little off and leads to now [defunct bit.ly bundle](http://bitly.is/1aG0YLU).  Thanks bit.ly!  It'd be nice if I could change the destination URL to the GitHub page instead.


## Additional Reading

* [RC Groups Forum Thread](http://bit.ly/1aFZpxj)
* [Hackaday Project Page and Build Log](http://bit.ly/1aG09m9)
* [Imgur Image Gallery](http://bit.ly/1aG00z3)
