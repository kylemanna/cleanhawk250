# CleanHawk 250 Pin Header Description

Most pin headers are labeled on the silkscreen.  When in doubt, verify with this document and a multimeter.

Only the P9 header is required to fly.

**Pin 1 is marked by a square pad.**

## P9 - Primary ESC Header

Provides +5V power and ground to the flight controller and serves as a connection for ESC control signals.

**Note**: The first batch *v1.0* of boards has the silkscreen incorrectly labeled, but the electrical wires are correct.  These boards are marked with white paint over the silkscreen to avoid confusion. 

Pin | Function
----|---------
1   | GND
2   | +5V
3   | ESC1
4   | ESC2
5   | ESC3
6   | ESC4

## P6 - Auxiliary Receiver Header

Provides signals commonly used for telemetry on RC Receivers such as the FrSky D4R-II.

Pin | Function
----|---------
1   | +BATT
2   | GND
3   | AD2
4   | GND

The `AD2` pin can be directly connected to a FrSky receiver and usedin place of existing voltage dividers.  It works with up to 4S lipos. `AD2 = +BATT * 2.32 / (10 + 2.32)`.  The telmetry gain will need to be adjusted appropriately, **verify with a multimeter before flying**.

## P7 - 5V Header

Provides access to 5V regulator output.  Use for auxiliary flight systems.

Pin | Function
----|---------
1   | +5V
2   | GND
3   | +5V
4   | GND

## P8 - 9V Header

Provides access to 9V regulator output.  Use for auxiliary flight systems.

Pin | Function
----|---------
1   | +9V
2   | GND
3   | +9V
4   | GND


## P5 - LC Filter Header

Provides access to LC filtered regulator output.  The source of the filter is selectable with the `JP1` Filter Sel solder pads.  Bridge the pads to select desired output voltage.  Most people power FPV gear will want 9V bridged to the center pad of `JP1` and power the video transmitter (VTX) and the FPV camera.

Pin | Function
----|---------
1   | +FLT
2   | GND
3   | +FLT
4   | GND

## P1 and P2 - Front and Rear Auxiliary Power

Intended to power LEDs or other accessories.

Pin | Function
----|---------
1   | +9V
2   | GND
3   | +5V
4   | GND

## P3 and P4 - Front and Rear Auxiliary Power

Intended to power LEDs or other accessories.

Pin | Function
----|---------
1   | +BATT
2   | GND
3   | +5V
4   | GND
