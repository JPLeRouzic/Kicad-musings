# PDP-11 hack
This project is a (tentative) Kicad schematics of the famous PDP-11 hack. If I am correct, it was a project by Brent Hilpert. 
http://madrona.ca/e/pdp11hack/index.html

Then Len Bayles also built a minimal PDP-11 around the J-11, a PDP-11 microprocessor, on a breadboard. 
https://www.chronworks.com/J11/

Several people have since produced various versions of this PDP-11 hack, including for S-100 bus!
Each has some variation, improvement, and/or additional features.

I took a lot of inspiration from the work of Peter Schranz:
https://www.5volts.ch/pages/pdp11hack/

This version stems from Brent Hilpert original work, but has some extensions:
- Much more RAM, 512KW
- I/O is fully decoded
- The data bus is buffered
- It has a GPIO (65C22)
- It can write into the upper byte
- The UART is the 6402 as in Brent Hilpert schematics, but the address is fully decoded
- It has 5 switches to test/learn to single-step the memory accesses, the HALT, interrupts, or make a reset
-The boot configuration could be set up with micro-switches


Beware I am an electronic, DEC and Kicad noob. Lots of dragons inside!

