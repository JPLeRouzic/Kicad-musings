# PDP-11 hack
This is a folder where are stored various Kicad projects loosely related to PDP-11.

The first project is a (tentative) Kicad schematic of the famous PDP-11 hack. It was a project by Len Bayles to build a minimal PDP-11 around the J-11, a PDP-11 microprocessor, on a breadboard. 
https://www.chronworks.com/J11/
Several people have since produced various versions of this PDP-11 hack. Each has some additional features.
My version is inspired by Brent Hilpert with a few differences, notably I put buffers on the data bus (not sure my implementation is valid). Beware the component types are a bit inhomogeneous (mix of TTL LS, ACT, etc...) as I am a Kicad noob!
http://madrona.ca/e/pdp11hack/index.html
Later I will probably take inspiration from the work of Peter Schranz:
https://www.5volts.ch/pages/pdp11hack/

# Kim 65C816
This is a tentative to use the 16-bit version of the famous 6502 microprocessor in a sort of KIM board similar to the SYM-1.
Needless to say, I reused the famous work of Eduardo Casino
https://github.com/eduardocasino/kim-1
But I didn't finish this project.

# UKNC
I have a UKNC computer, unfortunately non-functional. My goals are either:
- To reuse the two PDP-11 clone CPUs and make a little boad in the spirit of the PDP-11/Hack
- Or to make a PCB that would replace the faulty one and use Western components
