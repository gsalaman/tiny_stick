# Tiny Stick
Hardware design for a line of 8 surface-mount WS2812B LEDs

![tinystick](https://user-images.githubusercontent.com/43499190/78037458-d35a0680-7328-11ea-9676-655453b6d2d9.jpg)

## Project Goals
Test connections for multiple LEDs strung together.  Configurations:
- a three-pin jumper, with 5v, Din, and GND driven from an external source (uno)
- multiple boards strung together, driven by the Din and Dout Headers
- ATTINY85 driven lights.  External 5v input from Din header.  User iput from potentiometer and button.

Test power configurations:
- Can two coin cell batteries drive ATTINY85 configuration and 8 lights?  How about multiple boards (one tiny only)?
- Test AMS1117 LDO with 9v battery configuration
