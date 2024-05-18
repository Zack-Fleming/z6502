#Z6502

This is a collection of PCBs for a 6502-based computer. The core design of the computer is based on Ben Eater's design [here](https://eater.net/6502). I will be implementing changed to the original changes in the form of version revisions. Each board revision will have its own in-depth README.md, that will go over the changes in more depth and provide other relevant information.

This project was made using the KiCAD software, that can be downloaded [here](https://www.kicad.org/download/). If you do not have KiCAD, then there is also a zip file of the Gerber and Drill files needed to order a PCB. This zip file can be uploaded to any PCB manufacturer with no problem. 

Below the use of pinheaders is mentioned on different occasions, all of these pinheaders are of the 2.54mm pitch variety, and are the same used in the Arduino or Raspberry Pi boards as well. 


## Revisions at a Glance

Revision V1:

The main changes of this version are the addition of data and control bus readouts, in the form of LEDs and pinheaders. Another change was to add PCB footprins for DIP-8 and DIP-14 type oscillators. 


## Modules

The computer features two 8-bit ports, that have their own headers for I/O modules. The silkscreen of the board will include all of the information for the design of the modules. This information includes: the position and size of the mounting holes, the length and width of the boards, and the position of the interface pin header. both I/O ports are situated next to each other, and are identical in dimensions. Now, if an I/O device needs to use both of the available ports, then one can just design a board that combines the two ports into a single board. There is not need to keep the device to only one port. 

I am currently working on a template project for KiCAD, where you can create a project from the template, instead of copy pasting the project multiple times.

Currently planed modules include:
- 1602A 16x2 character LCD screen
- 8x8 button matrix 'keyboard'
- clock switching (not an I/O module)
- LED matrix ??x??
- more.
