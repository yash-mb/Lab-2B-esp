# TODO:

Create a 'sequencer' that allows you to record BOOT button presses and play them on the Neopixel, and also play a sequence of read/write commands. You should be able to:

record at a least a few seconds of button input to your RP2040 (in RAM)

replay a recorded sequence on your NeoPixel

loop a recording

save a recording to your laptop (the Python Serial library is one way to do this)

play a recording from your laptop

record 'macros' (a sequence of console commands) based on keystrokes in your serial console

hand-edit a list of register read/write commands on your laptop, and play them on the RP2040

include multiple I/O sources in a recording, and remap among the following:

inputs: BOOT button, console commands, register read/write commands

outputs: neopixel color, neopixel brightness, data over serial, register read/write commands


## Sequencer Video

https://user-images.githubusercontent.com/73771085/202282888-2cb7f6b7-0417-4733-afcc-d50153e2119d.mp4

This program works when the c program present on the QT Py is integrated with a Python program that takes input from the user and writes data into a TXT file. The c program is unable to access a file on the computer.

A C program contains 2 functions to read and replay the data sequence, which are called when it gets "r" and "p" as input, respectively.

A Python program reads serial input from the microcontroller (button press sequence) and saves it to a text file. Depending upon the input, the python program write "r" and "p" onto the com port to select read and replay the data sequence option.
