# Electronic Speed Controllers

The board is designed in such a way that it allows for ultra minature ESCs such as Flyduino's KISS 18A ESCs as well as traditional ESCs.

## Wiring

The ESC wires are routed to the flight controller via the `P9` pin header.  The traces on the board run to the corresponding pads where the ESCs are to be mounted.  Power is provided via 2oz copper and very short distance from the battery solder pads for optimum efficiency.

### KISS 18A ESCs

These ESCs can be mounted directly to 90° pin headers and soldered to the ESC boards.  This results in an ultra clean look.  Ensure the ESCs are secured with an additional mechanism (not just pin headers) to prevent them from vibrating in flight.

### Other ESCs

The holes on the board will accomodate up to 20AWG wire to power any variety of ESCs that exist.  Ideally the ESC would be small enough to mount in the space created for the KISS ESCs.

## Mounting

**Always provide isolation between ESCs mounted directly to the PCB with some sort of insulator such as 3M Super33 electrical tape or heatshrink.**  Failure to do this could result in a short and likely a crash that would follow the instant after.

The recommend mounting procedure is to place Super33 electrical tape on the PDB to insulate the ESC from the PDB.  A cable tie can then be used to wrap around the PDB to strap the ESC down to some of the existing holes or around the board itself.

**Ensure ESCs are secure before flight!**

## Future

It would be nice if the RC community could agree on a standard pinout and spacing of the ESC inputs so that pin headers could be utilized in the future.
