# Frequently Asked Questions

## What are R12 and R13?  Why aren't they populated?

These two resistors would set the input cut out voltage to shut the 5V and 9V regulators off.  This would protect the lipo batteries from over discharging.  The reality is that even if the primarily regulators shut off, the ESCs would continue draining the batteries (i.e. left overnight).

To avoid surprises such as loss of control, these resistors are not populated and the regulators operate as low as they can go.  With 3S and above, the regulators will continue to operate long after the craft falls out of the sky. 
