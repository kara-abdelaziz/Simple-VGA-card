# Simple-VGA-card
This project involves a replicate implementation of the World Worst Video Card, the educational vgaVGA video card designed by Ben Eater in his [website](https://eater.net/) and [YouTube](https://www.youtube.com/c/beneater) channel. A simple educational digital logic simulation called [Logisim](http://www.cburch.com/logisim/) was used to implement the Simple VGA Card. Actually, two identical implementations are deposited in this repository, one constructed from the ground using only logic gates and single memory cells (flipflops) placed in the file [SimpleVGACard.circ](https://github.com/kara-abdelaziz/Simple-VGA-card/blob/main/SimpleVGACard.circ), and the second using only TTL [74xx](https://en.wikipedia.org/wiki/List_of_7400-series_integrated_circuits) chip series, it is placed in the file [SimpleVGACard-TTL.circ](https://github.com/kara-abdelaziz/Simple-VGA-card/blob/main/SimpleVGACard-TTL.circ). The schematics of the two circuits are depicted just below.

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
