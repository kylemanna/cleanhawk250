# Bulk Capacitance

The board has provisions for 4 additional tantalum capacitors to help improve throttle response or smooth out ripple depending on battery and ESC combinations.  The parts aren't included as they are cost prohibitive and not needed by most people.

## Capacitor Selection

The pads are an industry standard `EIA 7343 metric` size.  Capacitors installed here **must be ultra low ESR** to have their desired effect. I also highly recommend following industry standard techniques for voltage derating capacitors to avoid failure.

That said, I recommend starting with AVX `TCJY336M025R0060`.  These capacitors can be purchased from [Digi-Key](http://bit.ly/1CZ7seG) in the US and likely many other places.

Consider using [findchips.com](http://bit.ly/1CZ8GXm) and the part number listed above to search for a better price.

## Installation

The unpopulated bulk capacitors are labeled with identfiers: `C1`, `C2`, `C3`, `C4`.

The line or bar on the capcitor marks the anode and should be orientated in the direction that places that anode nearest the `+` symbol on the PCB silkscreen.

These components are easily soldered with a traditional soldering iron and leaded or lead-free solder with flux.
