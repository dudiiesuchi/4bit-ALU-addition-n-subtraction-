# 4bit-ALU-addition-n-subtraction-

Objective:
To design and implement a 4-bit ALU capable of performing addition and subtraction operations using the following components:

IC7483: 4-bit Binary Adder.
IC7486: XOR Gate.
Basic components like logic switches, resistors, and LEDs.

Addition mode(M=0)
In IC7483 we can add and we gave input A and B and output is collected at 15,2,6,9 pins and the output carry is at 14 pin.
Since the mode (M) is 0, the XOR gates (IC7486) pass the B inputs unaltered to the IC7483.
Normal addition takes place as S=A+B.
Subtraction mode(M=1)
The binary number A is fed directly into the IC7483, while the binary number B is processed through XOR gates.The XOR gates invert each bit of B (producing B' when M = 1.)
the carry-in of IC7483 is 1, then adding 1 to the inverted B.
this process forms the 2's complement of B.then performs addition A+(B'+1)=A-B

​
 
​
 
