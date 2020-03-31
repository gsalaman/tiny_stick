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
