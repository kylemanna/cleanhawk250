# RGB LEDs

The CleanHawk 250 PDB comes with 6 standard brightness RGB LEDs to help the pilot determine orientation in flight.  By default the front LEDs are near white (some variance is observed due to 1% resistor manufacturing tolerance) and the rear LEDs are red.

## Additional LEDs

The LEDs are not high brightness and pilots are encouraged to use the P1-P4 headers to install brigher LEDs if desired and mount them a more visible location.

## Changing the LED Color

The 3 LEDs on each end of the board are wired in series and color can be changed by modifying the appropriate resistors.  To change the color, modify the resistor values to create any color in the rainbow.

The resisor size is `0603` and different resistor values can be purchased from places like Digi-Key.  Choosing a resistor value is matter of obtaining the target current as it relates to the other colors to obtain the desired overall color.

The LEDs are powered by the 9V regulator and each color is wired in with three LEDs in series.

### Front LEDs

Id | LED Color | Default Resistor Value
---|-----------|------------
R1 | Blue      | 68 ohms
R2 | Red       | 120 ohms
R3 | Green     | 68 ohms

### Rear LEDs

Id | LED Color | Default Resistor Value
---|-----------|------------
R4 | Blue      | not installed
R5 | Red       | 120 ohms
R6 | Green     | not installed
