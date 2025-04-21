# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
![318401808-c06bba9c-9c1e-4e92-a1e3-869583ce44c7](https://github.com/user-attachments/assets/280d62be-9d74-45fa-9059-e435a913f80a)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: G P HARIESH RegisterNumber:*/ 212224040100
HALF-ADDER
module exp3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= ( a ^ b);
assign carry =(a & b);
endmodule


HALF-SUBTRACTOR 
module exp31(a,b,diff,borr);
input a,b;
output diff,borr;
assign diff= (a^b);
assign borr= (~a&b);
endmodule
```
**RTL Schematic**
![Screenshot (107)](https://github.com/user-attachments/assets/c310ec50-4938-455c-829b-289758adba66)
![Screenshot (109)](https://github.com/user-attachments/assets/274c99b6-b462-4e4c-b6b2-22fc1a10494f)


**Output/TIMING Waveform**
![Screenshot (108)](https://github.com/user-attachments/assets/d32b08dc-6b46-43a5-835c-f1d1815b6fff)
![Screenshot (110)](https://github.com/user-attachments/assets/19f344f9-03ae-41fb-91ea-8060a47923bc)


**Result:**
Thus the program has been verified successfully.
