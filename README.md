# CleanHawk 250 Quadcopter Power Distribution Board for Emax 250

This document outlines the basic tasks to get the CleanHawk 250 Power Distribution Board (PDB) up and flying.

**Documentation can be found at the [CleanHawk250 GitHub repository](https://github.com/kylemanna/cleanhawk250).**


## Overview

The goal of the CleanHawk 250 PDB is to simplify wiring and imporve integration and reliability.  The printed circuit board replaces the bottom carbon fiber frame support on the Emax 250 / Nighthawk 250 quadcopters.

### Buy It Now

* [Tindie](http://bit.ly/1HMsioh)
* [Amazon](http://amzn.to/2fEIMti)

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
* (1) 1x4 pin header for the auxiliary port
* (1) 1x6 pin header for the ESC and flight controller port
* (3) 2x2 pin header for respective power supply outputs (5V, 9V, Filtered)

### Recommended Additional Components

#### Wire Extension Cables

It is recommended to use Dupont female to female cable connectors to wire the PDB to the receiver and flight controller. Available on [Amazon in 10cm length](http://amzn.com/B00KOL5BCC).

![Dupont cables](http://i.imgur.com/sG2cDaPm.jpg)

An alternative to these are male to male servo extension headers such as [these from Amazon](http://amzn.com/B00FGLSTY2).

![Servo extension](http://i.imgur.com/mOOl1RLm.jpg)

#### Angled Pin Headers

Consider picking up 90° 0.1" angled pin headers. Single row pin headers aid in mounting KISS ESCs.  Double row pin headers are very useful if the front/rear pin P1-P4 headers for LED connections.

#### XT60 Battery Connector and Pigtail

An XT60 connector is the most popular battery connector and a pigtail easily connects to the center battery pads.

![XT60 Pigtail](http://i.imgur.com/YXXkkKYm.jpg)

[MassiveRC carries XT60 connectors](http://bit.ly/1OBGKkD) and are perfect compliment for your PDB order.

#### Electrical Tape

Electrical tape is a critical requirement to insulate parts mounted on the PCB (i.e. KISS ESCs) to prevent wearing through the solder mask.  I stick to [3M Super33](http://amzn.com/B00004WCCL).  I recommend sticking some to the part of the PDB immediately below any mounted components such as ESCs.

#### Cable Ties

Strap down wires or ESCs to secure them.  Things will vibrate or rattle and eventually fail unless secured.


## Quick Start Guide

### Step 1 — Install Battery Wires

Battery wires up to 12 AWG are installed to the large through hole pads in the center of the board.  Due to the massive copper area surrounding the pads to transfer large amounts of current to the ESCs, **a large amount of heat is necessary to solder to this pad**.  *Turn the soldering iron temperature up, feed solder to help transfer heat from the tip to the pad, and be patient.*

### Step 2 — Install Pin Headers

The `P9` header is critical for flight and should be installed first.  All other headers are *optiona*l and pilots should refer to the [pin headers documentation](PinHeaders.md) for more details.

Verify that the Dupont cables or servo extensions are available to connect `P9` to the flight controller.

### Step 3 — Configure LC Filter and FPV Gear

The LC filter should be bridged to the 9V side for most FPV gear.  Verify this is valid for your gear and modify `JP1` if needed.  More details in the [pin headers documentation](PinHeaders.md).

### Step 4 — Install ESCs

Mount the ESCs to the board with **some insulation such as heat shrink or 3M Super33 to avoid shorts** that could occur should they wear through the black solder mask.  More details in the [ESC documentation](ESCs.md).

### Step 5 — Install on Quadcopter

Install the board in place of the bottom carbon fiber plate.  Verify that all screws and hardware fit in the designated area and aren't rubbing on the PDB. Note that there are recesses on the board around all mounting holes where copper has been removed to prevent issues.  **Failure to remove any objects that are touching the PDB could damage the PDB and cause a short and in extreme cases a fire.** Don't be on the news or YouTube with a flaming CleanHawk quad copter!

## Known Issues

Review the [Change Log](http://bit.ly/1GxYUxc) for more details.

### v1.0
* 5V and GND silkscreen labels flipped on first build, but copper traces are correct. Refer to images or verify with multipmeter before powering flight controller.
* QR code placement is a little off and leads to now [defunct bit.ly bundle](http://bitly.is/1aG0YLU).  Thanks bit.ly!  It'd be nice if I could change the destination URL to the GitHub page instead.
* `JP1` / `FILTER_SEL`'s +5V pad isn't hooked upto `+5V` and won't work as expected.  Instead jump the center pad of `JP1` / `FILTER_SEL` to the `+5V` pin of `P2` or `P3`.

### v1.1

* None

## Additional Reading

* [RC Groups Forum Thread](http://bit.ly/1aFZpxj)
* [Hackaday Project Page and Build Log](http://bit.ly/1aG09m9)
* [Imgur Image Gallery](http://bit.ly/1aG00z3)
* [Change Log](http://bit.ly/1GxYUxc)

## License

This work is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
