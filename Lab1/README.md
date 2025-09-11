# Lab 1
Switches, Lights, and Multiplexers

The purpose of this exercise is to learn how to connect simple input and output devices to an FPGA chip and
implement a circuit that uses these devices. I will use the switches SW9-0 on the DE10 Lite board, with a MAX 10 (10M50DAF484C7G) chip, as inputs to the
circuit. I will use light emitting diodes (LEDs) and 7-segment displays as output devices.


## PART I
### Module that connects the SW switches to the LEDR   lights

The inputs and outputs are defined as the Switches and LEDs and I assigned directly.

<img src="IMG/Part_I.png" width="300">

Bellow can be seen a demonstration:

<img src="IMG/Part_I_Demonstration.gif" width="500">


## PART II
### Module with the funcitonality of a 2-to-1 4 bit multiplexer

Using Logisim Evolution we can simulated the functionality of both a 2-to-1 1bit and 2-to-1 8bit multimplexer to understant how it works.
<img src="IMG/Part_II_1bitMUX_Demonstration.gif" width="300">
<img src="IMG/Part_II_4bitMUX_Demonstration.gif" width="300">

As we only have ten selectors in our FPGA, we will implement a 2-to-1 4bit multimplexer. In it will be four 2-to-1 1bit multimplexers with the following logic:
<img src="IMG/Part_II_mux_2_1_1_bit.png" width="300">
<img src="IMG/Part_II_mux_2_1_4_bit.png" width="300">

And in our main file we will need to call the 2-to-1 4bit using the Selector switches and the LEDs.
<img src="IMG/Part_II_main.png" width="300">

Bellow can be seen a demonstration:

<img src="IMG/Part_II_Demonstration.gif" width="500">


## PART III
### Module with the funcitonality of a 4-to-1 2 bit multiplexer

Using Logisim Evolution we can simulated the functionality of both a 2-to-1 1bit and 2-to-1 8bit multimplexer to understant how it works.
<img src="IMG/Part_III_2bitMUX_Demonstration.gif" width="300">

As we only have ten selectors in our FPGA, we will implement a 4-to-1 2bit multimplexer. In it will be two 4-to-1 1bit multimplexers with the following logic:
<img src="IMG/Part_III_mux_4_1_1_bit.png" width="300">
<img src="IMG/Part_III_mux_4_1_2_bit.png" width="300">

And in our main file we will need to call the 4-to-1 2bit using the Selector switches and the LEDs.
<img src="IMG/Part_III_main.png" width="300">

Bellow can be seen a demonstration:

<img src="IMG/Part_III_Demonstration.gif" width="500">


## PART IV
### Module of a 7 segments decoder to print the letters "H", "E", "L" and "O"

Using Logisim Evolution we can simulated the functionality of a 7 segment decoder to understant how it works. In our case we will only use 7 bits, the "dot" (8th bit is not needed)
<img src="IMG/Part_IV_7seg_Demonstration.gif" width="300">



## PART V
Multiplexer 3-to-1 3 bits to print an static "HELLO" in five 7-segments

## PART VI
Multiplexer 3-to-1 3 bits to print an static "HELLO" in six 7-segments, creating a space at the end/begining to create the ilusion of moving

## (extra) PART VII 
Implement a counter to trigger de segments without using the selector and make de word "HELLO" move by it self. Can be adjusted in time to go faster and slower.

