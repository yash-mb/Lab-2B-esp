# TODO:

Toggle the Qt Py's Neopixel LED when the BOOT button is pressed, using only direct register reads to access the boot button status. You may use the SDK to initialize the board and the pins, and the WS2812 example code to toggle the Neopixel.

# Registers Video

The following demonstration video shows reading from a register directly. In this program the neopixel LED blinks, if the on-board BOOT button is pressed.

https://user-images.githubusercontent.com/73771085/202279728-a92b1488-7bbe-4a02-b180-5d9fb22b9f88.mp4

Here, we are reading the register with address 0xd0000004. The bit value present at 21st location will be the reading from the boot pin. We have masked the other bits and turning the LED on when boot pin is pressed.


