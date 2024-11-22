# HALF_ADDER_SUBTRACTOR
### NAME: NAVEEN KUMAR S
### REF NO:24900140

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
![Screenshot 2024-11-15 143300 (2)](https://github.com/user-attachments/assets/a46ef337-b704-4480-81f3-96f89a36fd0b)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
*HALF SUBTRACTOR:*

module exphs(diff,borr,a,b);

input a,b;

output diff,borr;

wire w1;

xor g1(diff,a,b);

not g2(w1,a);

and g3(borr,w1,b);

endmodule 
*HALF ADDER*

module exphs(Ssum,cout,a,b);

input a,b;

output sum,cout;

xor g1(sum,a,b);

and g3(conta,b);


/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: RegisterNumber:24900140

**RTL Schematic**
![Screenshot 2024-11-15 145152 (2)](https://github.com/user-attachments/assets/c1b17ebd-1545-48d4-a45f-9ec253fddd72)

![Screenshot 2024-11-15 145152 (2)](https://github.com/user-attachments/assets/5d26bce7-440d-43ee-87ea-fbaa8615d66e)

**Output/TIMING Waveform**
![Screenshot 2024-11-15 141306 (1)](https://github.com/user-attachments/assets/4db9f431-31bc-49be-870a-68b48bd6b83b)
![Screenshot 2024-11-15 135011 (2)](https://github.com/user-attachments/assets/3a969d99-7ea9-4f04-9704-bc52364ae311)

**Result:**
To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming was successfully.
