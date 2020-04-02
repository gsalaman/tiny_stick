# Tiny Stick
Hardware design for a line of 8 surface-mount WS2812C LEDs

![tinystick](https://user-images.githubusercontent.com/43499190/78037458-d35a0680-7328-11ea-9676-655453b6d2d9.jpg)

# Configurations
## UNO (or other external processor)
You can use the 8 RGB LEDs with any Arduino capable processor.  Supply 5v, Gnd, and your Data Input via the "external input" ports on the bottom-left of the board.

You can chain together multiple sticks by using the "external output" port on the bottom-right.
## Tiny85
The board can also be populated with a tiny85.  Recommended configuration is to put a socket on U1 (top left) as to allow for the processor to be removed and programmed.  This processor connects to the data input line via Ardiuno Data pin 3 (physical pin 2 on the tiny).

There is also space on the board for a potentiometer.  The two sides are connected to power and ground, and the middle is connected to arduino pin 2 (physical pin 7).

Finally, there is a push-button, connected to Arduino pin 0 (phyical pin 5).  This input is pulled-up.

## Using External 5v Power with Tiny85
You can connect +5v and GND to the "external input" pins on the bottom left of the board to power the Tiny and LEDs.  This input is *not* gated by the power swiitch.

## Using Coin Cell
The back of the board has a spot for a coin cell holder, which can provide power to the Tiny and LEDs.  To enable this:
* connect the middle and bottom pins of the "input power select" block, either via a jumper or solder blob.
* populate the "internal power" switch on the bottom of the board (for switch control), or, if you want it "always on", put a solder jumper between the left and middle pins.

## Using the 9v (vin) input)
You can connect a 9v battery (or anything greather than 6v) to the Vin jumpers on the bottom left of the board.  This input goes through a voltage regulator to provide 5v.  To enable this:
* connect the top and middle pins of the "input power select" block, either via a jumper or solder blob.
* populate the "internal power" switch on the bottom of the board (for switch control), or, if you want it "always on", put a solder jumper between the left and middle pins.

One note:  since the switch is after the voltage regulator, the 9v battery will *always* be powering on the voltage regulator...not an ideal design.
