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

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

i)HALF ADDER
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry

i)HALF SUBTRACTOR
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule

Developed by: Sreejaa RegisterNumber: 25015302

**RTL Schematic**
#HALF ADDER
<img width="272" height="135" alt="502803706-7da00ae5-4c9f-4d44-bca2-6b4087e4afca" src="https://github.com/user-attachments/assets/a32b04f6-7a65-4d15-9729-0b6f274d4414" />

#HALF SUBTRACTOR
<img width="309" height="123" alt="502803719-2b761cab-b9f2-4fbe-b15d-e571bbdc4657" src="https://github.com/user-attachments/assets/88bf2319-f1d9-4536-9dad-fc1b16d9ff59" />

**Output/TIMING Waveform**
#HALF ADDER
<img width="823" height="176" alt="502803854-557813dd-ceeb-4b0c-9bc2-07016bda539d" src="https://github.com/user-attachments/assets/862b5ab0-cdcf-4c3b-ad7e-a63b2a8825f0" />

#HALF SUBTRACTOR
<img width="819" height="256" alt="502803902-5283d38e-fe67-4ac0-924c-7d371e3cf759" src="https://github.com/user-attachments/assets/6a6cbf6d-c2bb-4040-a5c3-0524c42f1a75" />

**Result:**
Thus the OUTPUT's of Encoder and Decoder are verified by synthesizing and simulating the VERILOG code.

