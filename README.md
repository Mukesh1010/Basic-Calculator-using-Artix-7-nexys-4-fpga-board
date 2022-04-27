# Basic-Calculator-using-Artix-7-nexys-4-fpga-board
This is a basic calculator verilog program which uses artix 7 nexys 4 fpga board for performing the operations

1.As soon as the FPGA is connected to the PC, one can see the displays showing 00000000.If reset switch is high (1) the number becomes 00000000.
2.In order to give the first number as input, M should be low (0) and BCD input is given through switches from 2 to 9 and the same switches are used to give the second number as input. After the first input is given, make M high (1) so that the second number can be given.   
3.To perform the Arithmetic operations a,b,c are used to select the operations 
         abc
000 - xxxx.
001 - Addition
010 - Difference
011 - Multiplication
100 - Division
101 - Remainder
110 - Remainder
111 - Remainder
4.After all the operations are performed the result is displayed on the last four seven segment displays and input number1 on the first two seven segments and second number on the next two seven segment displays.

Sw[0] - reset
Sw[1] - M
Sw[10] - c
Sw[11] - b
Sw[12] - a  
Sw[5:2]  are multiplexed to give the number1 and number2 with M acting as a select line.
Sw[9:6]  are multiplexed to give the number1 and number2 with M acting as a select line.
An[7:0]-anode(8-bit)
Seg[6:0]-cathode(7-bit)
Clock-clk

https://www.youtube.com/shorts/G9L7EtFmp0c
