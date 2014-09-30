nyan-pirate
===========

Bus Pirate + Nyan Cat

This has more extensive changes than the original nyan pirate

* the cat is on the 'bottom' of the pcb to have minimal change to the Bus Pirate design and have the rainbow cables come out from behind the cat.
* a different nyan cat bitmap was used to print a little better
* image and outline are changed in the dp_pcbs.lbr file
* in the process of adjusting everything to fit into the new board, a couple text labes are out of place (oops)
* i added two 1x1 .1" header points 20mm apart to hold a cr2032 battery holder. It's on a separate supply but shared ground
* i added 6 2x3 pin headers for LEDs:
  * pins 1 and 5 are ground
  * pin 3 connects to the battery
  * pins 2-4-6 are connected
  * In order to drive LEDs at full voltage, attach them from pin 3 to pin 1
  * in order to drive LEDs with a current limiting resistor, put the resistor from 3 to 4 and LEDs from 1-2 and 5-6
* i moved the USB connector to the edge of the board
* The Bsides Logo in silk/soldermask is in the nyan-pirate.lbr file. It's on layers 200 and 201
* the .cam file will put the 200 and 201 layers into the soldermask and silkscreen gerbers.
