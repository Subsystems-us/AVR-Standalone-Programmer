# AVR-Standalone-Programmer
Program an AVR with the program loaded on an SD card. Load your HEX file onto an sd card, rename it to firmware.hex, insert it into the sd card board, select the jumper position to power the target board or not, connect your target board (be careful as there is no protection for poor connections) and press the Program button. The lights will let you know if everything went ok or if there was an error.

This software is based on the work of Nick Gammon. I have removed some of the routines (like the Crossroads code) and added a function to change the fuse settings.

To change the fuse settings, add a line to the beginning of the HEX file for each fuse with the following format:

FXhh

- Where F tells the software that this line changes a Fuse
- X is the fuse to change (L = low, H = high, E = extended, B = Lock Byte)
- hh is the hex value to change the fuse to.

Ex:  FL7F will change the Low fuse to 7F

![AVR_prog01](https://github.com/Subsystems-us/AVR-Standalone-Programmer/assets/78771234/080683f7-d271-44d3-af26-90e06632041a)
