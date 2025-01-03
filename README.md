# 10-Step Electronic Sequencer

This is a simple sequencer project based on one CD4017 and three 555 timers. In 4th grade, I was learning about the 4017 and 555 timers and I had the inspiration to create a form of musical instrument by combining them togther. My first prototype was made on a breadboard and I remember that it was the most complicated circuit I had made up until that point in time. A few years later in 2021, I was learning about how to use Eagle PCB and decided to make this circuit into a PCB. And the Pocket Sequencer was born!

## Circuit

The schematic is fairly straightforward. The first 555 timer (U2) is running in astable mode and is used to drive the 4017 with a clock pulse. The 4017, which is a decade counter activates each output and moves on to the next with each clock pulse.
The pot R2 controls the speed of the counter which controls how fast each step in the sequencer is.
Each output of the 4017 is then connected to a pot (R5 - R14) which controls each individual tone in the sequencer by changing the astable operation of U2 which is the second 555 timer. By varying the value of each of the pots and the value of R3, the freqency of the timer is varied, changing the tone at the output.
The output of U3 is then connected to the trigger pin of U4. The third 555 timer is running in monostable mode which means that each pulse on the trigger pin creates a pulse on the output pin for a set length of time controlled by the value of R4.
In addition to the tones, the row of led's will light up at each corresponding step in the sequence.
The values of R3 and R4 can change the overall tone of the sequencer and when adjusted in conjuction with each other some very interesting tones can be created!
The recommended power source is a 9V battery, but anything 5V to 16V should work fine.

Connect a battery and a speaker to the pin connectors and have fun playing with the trimmers and make some music!
