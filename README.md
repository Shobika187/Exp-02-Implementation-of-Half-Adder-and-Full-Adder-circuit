# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: P Shobika
RegisterNumber:  212221230096

## Half adder
```
module HalfAdder(A,B,sum,carry);
input A,B;
output sum,carry;
xor(sum,A,B);
and(carry,A,B);
endmodule
```
## Full Adder
```
module FullAdder(a,b,c,Sum,Carry);
input a,b,c;
output Sum,Carry;
assign Sum = ((a^b)^c);
assign Carry = ((a&b) | (b&c) | (c&a));
endmodule
```
*/
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
## Half Adder
![Screenshot (46)](https://user-images.githubusercontent.com/94508142/190621478-a47a7f35-8476-432b-8545-e9ad421a8788.png)

## Full Adder
![Screenshot (49)](https://user-images.githubusercontent.com/94508142/190621551-0a65a223-9ce1-4592-8509-51e33ddc935a.png)

### TIMING DIAGRAM
## Half Adder
![Screenshot (47)](https://user-images.githubusercontent.com/94508142/190621710-5c39b43f-14df-4090-80d0-8b84b30c68d2.png)

## Full Adder
![Screenshot (50)](https://user-images.githubusercontent.com/94508142/190621753-59b3a7c2-2d93-4ec7-8102-afc31004b79c.png)

### TRUTH TABLE 
## Half Adder
![Screenshot (48)](https://user-images.githubusercontent.com/94508142/190621891-5cb78b59-b918-47b2-aa06-3c2a4a6a67c4.png)

## Full Adder
![Screenshot (51)](https://user-images.githubusercontent.com/94508142/190621948-dd737e2b-1215-4256-8d1c-b427d80ac797.png)

### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming is successfully done
