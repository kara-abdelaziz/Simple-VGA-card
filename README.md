# Simple-VGA-card
This project involves a replicate implementation of the World Worst Video Card, the educational VGA video card designed by Ben Eater in his [website](https://eater.net/) and [YouTube](https://www.youtube.com/c/beneater) channel. A simple educational digital logic simulation called [Logisim](http://www.cburch.com/logisim/) was used to implement the Simple VGA Card. Actually, two identical implementations are deposited in this repository, one constructed from the ground using only logic gates and single memory cells (flipflops) placed in the file [SimpleVGACard.circ](https://github.com/kara-abdelaziz/Simple-VGA-card/blob/main/SimpleVGACard.circ), and the second using only TTL [74xx](https://en.wikipedia.org/wiki/List_of_7400-series_integrated_circuits) chip series, it is placed in the file [SimpleVGACard-TTL.circ](https://github.com/kara-abdelaziz/Simple-VGA-card/blob/main/SimpleVGACard-TTL.circ). The schematics of the two circuits are depicted just below.

# Simple-VGA-card schematics in Logisim (ground-up version)

![Simple VGA Card image](https://github.com/kara-abdelaziz/Simple-VGA-card/blob/main/SimpleVGACard.PNG)

# Simple-VGA-card schematics in Logisim (TTL-74xx version)

![Simple VGA Card TTL image](https://github.com/kara-abdelaziz/Simple-VGA-card/blob/main/SimpleVGACard-TTL.PNG)

# Files description

1. SimpleVGACard.circ : The circuit of the card containing a ground up version constructed using primitive logic gates and memory cells.
2. SimpleVGACard-TTL.circ : The circuit of the card version designed using the TTL 74xx chip series.
3. 74xx Libary-v1.0.circ : The library used by logisim to call the TTL 74xx circuit used in SimpleVGACard-TTL.circ
4. SimpleVGACard.png : A schematic of the ground up version of the video card.
5. SimpleVGACard-TTL.png : A schematic of the TTL 74xx version of the video card.
6. README : This text file.

# Bill of Materials (BoM)

The list of all the parts used in this project are as follow :
1. 1 x 10MHz crystal oscillator.
2. 3 x 7400 chips (Quad NAND gates).
3. 4 x 7404 chips (Hex Inverters).
4. 8 x 7430 chips (NAND8 gate).
5. 6 x 74161 chips (4-bits counters).
6. 1 x 28C256 chip (32 KB EEPROM).
7. 3 x 680 Ω resistors.
8. 3 x 1.5 KΩ resistors.
9. 1 x VGA port.

# Notes

1. Logisim could not simulate analog circuits, thus the risistor ladder responsible for the RGB different voltages could not be replicated in the simulation.
2. In circuit _SimpleVGACard-TTL_, 27C512 EPROM was used instead of the 28C256 due its absence from the 74xx library, normally there is no difference using either of the two in the circumstance where the ROM is used in this circuit.
3. No VGA display was implemented in this simulation considering the screen a part outside the circuit.
4. The ROM is not loaded with any image data to display, because there is no device to display to.
5. The two seven segment displays are not part of the project, they are used for debugging puposes, mainely used to indicate the pixel and line number.

# Website:
- [www.el-kalam.com](https://www.el-kalam.com/): my personal website for more details, contains this project and others.

