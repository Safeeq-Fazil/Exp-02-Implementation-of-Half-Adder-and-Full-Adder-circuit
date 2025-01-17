# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
## Date: 23/9/2023
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
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Safeeq Fazil.A
RegisterNumber: 212222240086

1. Program to design a half adder:

module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule 

2. Program to design a full adder:

module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule

```
## Logic symbol & Truthtable

## Truth Table
HALF ADDER:

![image](https://github.com/Safeeq-Fazil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118680361/9b4a71eb-8d15-4ecd-b42f-38f3636c6e1b)

FULL ADDER:

![image](https://github.com/Safeeq-Fazil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118680361/629eae2f-49e4-45c9-883a-42305ca95f2c)

## RTL
HALF ADDER

![image](https://github.com/Safeeq-Fazil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118680361/d8ac11fc-a13f-4ca7-afb5-5010992a3a99)

FULL ADDER

![image](https://github.com/Safeeq-Fazil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118680361/2f67b3a2-4ccf-4d82-94c9-39429db27018)

## OUTPUT:

HALF ADDER

![image](https://github.com/Safeeq-Fazil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118680361/5357d606-086d-4bc6-a757-2f6e15881137)

FULL ADDER

![image](https://github.com/Safeeq-Fazil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118680361/41b25b21-d2ef-4ff0-b67d-dca564172dd8)

### Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
