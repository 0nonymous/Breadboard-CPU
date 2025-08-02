This repository contains files and scripts that are used to program and flash data to my breadboard CPU--and other stuff

This is the block diagram for the CPU
diagrams/CPU Block Diagram.jpg

Videos and photos of the project will be added soon
This is an 8-Bit CPU made using primarily 74LS series chips. It has a complex instruction set and 64 kilobytes of addressable memory. In addition to the CPU, the breadboards contain the "computer" itself (ie: memory and peripheral interface)
For peripheral interface it has two 6522 VIA that give it 32 GPIO pins
Various peripherals have been connected like LCD character displays, keypads, and LED matrix. Some programs include a fibonacci sequence, adder calculator, keypad reader, name printer, and the most complex program so far, Snake.

This project is the 3rd iteration of my breadboard CPU. This iteration has started in July 2023 and was completed in around December/January of that year but it had various issues that took most of 2024 to fix. Programs were written for it in 2024 before more problems being discovered led to the temporary pause of writing programs to refocus on fixing it. I've written more programs in 2025 such as Snake.

Where this project is going: I am trying to connect the CPU to a VGA monitor and later a keyboard to enable new possibilities for it. The VGA circuit is currently being built.

IMPORTANT: the assembly language files are in .txt files
IMPORTANT: I don't really know how to use GitHub properly yet (learning)
IMPORTANT: see the credits.txt file because things credit were important for the project

This repository has recently been organized into folders to make it easier to find things:
assembler tests = files to test if the assembler works properly
assemblers (breadboard CPU) = contains the assembler (assembler_3.py) for assembling the text file into a "binary" text file; write.py turns the "binary" text file into a bin that can be flashed onto the ROM
clock = the CPU uses an Arudino to provide clock pulses so that is the code for it
diagrams = contains the design diagrams and other important materials
hardware test programs = breadboard CPU programs to check if various instructions are working
keypad projects = projects that use a keypad
lcd char projects = projects that use an LCD character display (some of these programs use a keypad)
led matrix projects = projects that use an LED matrix display (some of these programs use a keypad)
microinstruction = contains microinstructions (steps to run each instruction) that were flashed onto the instruction decoding ROMs
Test KiCad = the KiCad project for my VGA driver (unfinished)

Let me know if you have any questions or what else I should put on this,
Thanks :)