Introduction-
Xs-3 (Excess-3) code is a non-weighted BCD code obtained by adding 3 to the decimal digit. It is widely used in digital systems because it is self-complementing.
This project implements an XS-3 adder/subtractor circuit using digital ICs to perform addition and subtraction of decimal numbers represented in XS-3 format.
 

Objective-
o   Design Xs-3 Adder and Subtractor circuit using digital logics
o   Take input in decimal form
o   Show result output on 7 segment displays
 

Design Concept and Implementation-
Xs-3 Adder Subtractor circuit is based on basic algorithm of xs-3 addition and subtraction. In Xs-3 addition we convert decimal numbers into BCD adds 3 into each digit before writing; then we do simple BCD addition but if carry is generated then we add 3 (0011) into that nibble if carry is not generated then we subtract 3 (1101) from that nibble.

 In this project we have made  8-bit Adder subtractor circuit and we took a Input in decimal and converted that decimal into BCD by using IC 74LS147 then added 3(0011) into each nibble by using adder IC 7483 by this we got required Xs-3 number; then, I created 8-bit adder subtractor circuit by using IC 7483 and gates. The final results are shown on 7 segment displays by using IC 7447 driver.

To switch on the Subtractor circuit there is one logic state (K) on right side of circuit and also shown in circuit below which default state is zero that is addition mode; if we set it 1(high) then by XOR circuits the inputs, let’s say B is converted into B’ and by 2’s complement while adding one into B’ it gives final result as -B. Then by the adder circuit it becomes A+(-B) = A - B.
