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
Developed by: Balamurugan p
RegisterNumber:  212222230017

HALF ADDER
```
module Adder(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule
```
FULL ADDER
```
module fulladder (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```
*/
Logic symbol & Truthtable
RTL realization

### Output

### RTL
HALFADDER

![halfadder](https://user-images.githubusercontent.com/118680410/231664739-6f473afd-76ae-4a1e-911b-9de1deeae2f9.png)

FULL ADDER

![fulladder](https://user-images.githubusercontent.com/118680410/231664768-bb706bc4-b42e-4f46-a244-4a76b9d06da0.png)

### TIMING DIAGRAM
half adder

![halfadderwave](https://user-images.githubusercontent.com/118680410/231665233-60861d5a-524a-4ab9-8344-83a2fb64057a.png)

full adder
![fullwave](https://user-images.githubusercontent.com/118680410/231665382-53f05756-7ad3-45de-8a97-7b409799860d.png)

truth table

half adder

![hadd](https://user-images.githubusercontent.com/118680410/231664330-9096ad07-e77f-486f-b7fe-cc9de2b7e8f8.png)

full adder

![fadd](https://user-images.githubusercontent.com/118680410/231664352-78185c7f-9475-49d6-bd74-6c52a496aadb.png)

### Result:
Thus,the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
