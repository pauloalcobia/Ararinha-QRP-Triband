# Ararinha-QRP-Triband

This is a PCB for the Ararinha 6 project from Miguel PY2OHH, made with a 4 layer board. 

You can find the correct values of the BPF for 40/20/15m bands on the RFSim99 files in the repository.

### Already tested in the project prototype:
* IF
* Microphone Pre-Amplifier
* LM386 Audio Output
* XTAL Filter
* BPF for 40m and 15m - Tested on MiniVNA Tiny

### Note on current version of the board:

* RF Switching: I found that the MASWSS0136TR is a better RF Switch for the project than the one in the PCB, going for it. Less expensive and doesn't have the 50 ohm termination that could ruin the project impedances.  

* RF transistors: I started building the project with 2n3904 but I'm going to switch to the 2SC4915 that are in use in newer radios and have better specifications on RF. Decided on them because I wanna beat the record for Ararinha design, using it on 15m and later on 
6m band. (As 21/09/2017, testing it with the 2sc4915 looking good and no parasitic oscillation found yet)

* LM386 amplifier circuit: There is a missing electrolytic capacitor between the LM386 pin 5 and the Headphone output. Can be any capacitor from 10uf to 470uf with at least 16v.

* The 78L05's on the V1.0 board has pin 1 and pin 3 changed. Corrected on V2.0 schematic

* 4:1 xformer is inverted in both RF Mixer and RF Pre sheets. Needs to be corrected. In V1.0 you can just rotate it 180 degrees.

* R32 (2k2 resistor on RF Pre) is wrong placed, just replace it with a 0R resistor for V1.0 board

* CWKey isn't routed to any connector


### A 3D preview of the 4 layer board for the Ararinha 6 Project
![Preview](https://github.com/PY1CX/Ararinha-QRP-Triband/raw/master/ArarinhaPCB3D.png)

It's free to copy or modify and uses the Beerware License ( https://en.wikipedia.org/wiki/Beerware )


