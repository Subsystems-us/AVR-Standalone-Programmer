# AVR-Standalone-Programmer
Program an AVR with the program loaded on an SD card.

This software is based on the work of Nick Gammon. I have removed some of the routines and added a function to change the fuse settings.

To change the fuse settings, add a line to the beginning of the HEX file for each fuse with the following format:

FXhh

- Where F tells the software that this line changes a Fuse
- X is the fuse to change (L = low, H = high, E = extended, B = Lock Byte)
- hh is the hex value to change the fuse to.

Ex:  FL7F will change the Low fuse to 7F
