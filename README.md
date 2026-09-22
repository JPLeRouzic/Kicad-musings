# This is a folder where are stored various Kicad retrocomputing projects.

## PDP-11 hack
The first project is a (tentative) Kicad schematic of the famous PDP-11 hack. It was a project by Len Bayles to build a minimal PDP-11 around the J-11, a PDP-11 microprocessor, on a breadboard. 
https://www.chronworks.com/J11/
Several people have since produced various versions of this PDP-11 hack. Each has some additional features.
My version is inspired by Brent Hilpert with a few differences, notably I put buffers on the data bus (not sure my implementation is valid). Beware the component types are a bit inhomogeneous (mix of TTL LS, ACT, etc...) as I am a Kicad noob!
http://madrona.ca/e/pdp11hack/index.html
Later I will probably take inspiration from the work of Peter Schranz:
https://www.5volts.ch/pages/pdp11hack/

## SYM-1 65C816
This is a tentative to use the 16-bit version of the famous 6502 microprocessor in a sort of SYM-1 clone.
It must be visually very similar to the SYM-1, but internally it's quite different.
- It uses a 65C816
- The address bus is 24 bits
- The 816 placement is where U27 was instead of being in upper right corner to shorter tracks length. Visually there is no impact as both U5 and U27 are DIP 40 plastic,
- As the address space is 16M now the upper 32K in address space is dedicated to ROMs and IO. I still have to design how it works when the 816 is in 6502 mode.
- The U5 (old U27) 6532 is replaced with a 6522, because of availability.
- No ROM content is written at the moment.
- The TTL logic families choice is a bit hectic and result from multiple constraint in Kicad. I don't expect to respect that when implanting real components.

## UKNC
I have a UKNC computer, unfortunately non-functional. My goals are either:
- To reuse the two PDP-11 clone CPUs and make a little board in the spirit of the PDP-11/Hack
- Or to make a PCB that would replace the faulty one and use Western components
