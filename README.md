# The [BOSS DS-1](https://www.thomann.de/ro/boss_ds1_distortion.htm)
![image](https://bdbo2.thomann.de/thumb/bdb3000/pics/bdbo/7536188.jpg)
Maybe the most popular distortion pedal to ever hit the market. It's harsh attack and heavy distortion make it the perfect choice for genres like thrash and heavy metal.

# The DST-1
![isometric](https://github.com/user-attachments/assets/fcb0ee38-672f-449a-bfc0-e2adf3bfc920)

The DST-1 is a copy of the DS-1's schematic, but modified in certain ways.
The original DS-1 used some relatively hard to find components, so i've swapped those out with some common components like the 2N3904 and the TL072.

This distorion pedal is intended to set the standard to me as to what "a good distortion pedal" sounds like. Usually distortion pedals are quite cheap and easy to build, but their sound comes down to the components used. Thus, I might swap out the TL072 for other op-amps aswell as the transistors. Good components make good pedals, but sometimes their cheapness and imperfections make the pedal unique. 

# The Schematic
![DST-1_Schematic](https://github.com/user-attachments/assets/2cee1d8d-a1e5-451e-9762-bd3f3e70fbaf)
The schematic is quite cramped since I wanted it to fit all in a single unbroken signal line, from the input to the output. The +Vcc and -Vcc are supplied using a voltage divider between the positive and negative terminals of a 9v battery, also forming a vitual ground. To make sure I make the disctinction between the Gnd of the battery and the Gnd of the signal, I decided to rename signal's ground to +4,5v since it's the midway point between the +9v and the 0v of the battery.

The 3PDT switch didn't had any symbol in KiCAD's library so I made them myself, aswell as the footprint, using the datasheet for the switch. Feel free to copy use and share since resources should not be kept behind paywalls and such and anybody should have the right to use resources to create / recreate things.

# The PCB
I've yet to test the circuit, but the PCB is on it's way and will soonly arrive.

The PCB is made to fit in a Hammond 1590B aluminium enclosure, thus it's rather strict dimensions. I'm not quite sure if it'll fit tho since I've been too lazy to make the board's outline match the enclosure's lid, but I plan to do it... sometime in the future I hope ...

Here is the datasheet for the enclosure tho!

![image](https://github.com/user-attachments/assets/0b2e4468-79c0-4179-9b62-bffd1439946f)

I also added some (4 to be precise) M3 mounting holes that are connected directly to 0v, thus being capable to ground the whole PCB if the user so desires.
The LED can be anything from red to UV, I used a 220 ohm resistor but it can be replaced with any kind of THT resistor to match the desired brightness/current need of an LED, if so desired.

I plan to power up the pedal using a 9v battery connected via a barrel jack, at the back of the board. 

To do:
- [x] Schematic
- [x] PCB design
- [ ] Integrate the pedal in an enclosure
