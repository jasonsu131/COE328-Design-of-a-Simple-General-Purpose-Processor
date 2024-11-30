  The Simple Central-Processor-Unit (CPU) designed consists of 2 latches, 4 seven segment displays, an arithmetic logic unit, a FSM, and a 4x16 decoder. 
Each latch processes an 8-bit input (A and B) which represents the last four digits of our student number. 
If the reset is not on, the 8-bit input is sent to the ALU through a positive edge clock input. The FSM is a moore machine that determines and switches to the next depending on the previous state.
There are a total of 9 states that switch through chronologically when data_in is on and the clock has a positive edge.
Each state has a corresponding student number digit which is sent to a seven segment display while the current state is passed onto the 4x16 decoder.
The 4x16 decoder is comprised of two 3x8 decoders and converts the 4-bit state inputs into 16-bit while the enable is on. 
The ALU receives inputs A and B from the two latches, the state in 16-bit from the decoder, and a clock signal which is synchronous throughout the whole system. 
The ALU performs a different calculation of A and B depending on the state, with the sign and upper and lower four bit results sent and displayed on a seven segment display. 

Further component discriptions, waveforms, and truth tables are included in the lab report.
