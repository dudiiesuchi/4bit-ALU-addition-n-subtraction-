# 4bit-ALU-addition-n-subtraction-

# Overview:
This Multisim design and implementation of a 4-bit ALU capable of performing addition and subtraction operations 
# components:
IC7483: 4-bit Binary Adder.
https://i0.wp.com/circuitdiagrams.in/wp-content/uploads/2022/04/IC-7483-Pinout.png?resize=840%2C665&ssl=1
IC7486: XOR Gate.https://www.futurlec.com/IC7486.gif

Basic components like logic switches, resistors, and probes.

# Addition mode(M=0)
We can add to IC7483, We gave inputs A and B, and the output is collected at 15,2,6,9 pins. The output carry is at 14 pins.
Since the mode (M) is 0, the XOR gates (IC7486) pass the B inputs unaltered to the IC7483.
Normal addition takes place as S=A+B.
# Subtraction mode(M=1)
The binary number A is fed directly into the IC7483, while the binary number B is processed through XOR gates. The XOR gates invert each bit of B (producing B' when M = 1.)
the carry-in of IC7483 is 1, then adding 1 to the inverted B.
this process forms the 2's complement and then performs addition A+(B'+1)=A-B
![image](https://github.com/user-attachments/assets/7ea09b56-cd59-4d54-9b0a-4fd1ab1d2533)
![image](https://github.com/user-attachments/assets/9a844d65-7f27-4ccf-a0dd-3e193058e3c3)

# simulation results :

# addition of two numbers:
keeping M=0, the addition of two numbers can be done. 
![image](https://github.com/user-attachments/assets/6d4362a7-76c4-4e17-8e7e-4091edd7fe7d)
# subtraction of two numbers :
keeping M=1, subtraction can be done by making 2's complement method. 
![image](https://github.com/user-attachments/assets/dd4f9e42-7e01-4311-a1cc-162abc97102a)

 
​
 
