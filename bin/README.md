Binary (executable) files
=========================
This directory is for the binary files, as simulators, assembler and test files.
These are binaries, compiled under Ubuntu 16.04

Y86asEMPA
---------

This assembler program assembles files given in EMPA/Y86 format to the corresponding object format.
Usage:
Y86asEMPA <file>.Eys
The output is <file>.Eyo
The assembler compiles originale .ys sources as well

simEMPAtext
-----------
This text version simulator executes program given in the Eyo files.
Usage:
simEMPAtext <file>.Eyo <No of cores>

simEMPAGUI
----------
This GUI based simulator executes program given in the Eyo files.
Usage:
simEMPAGUI
then use the GUI controls.
