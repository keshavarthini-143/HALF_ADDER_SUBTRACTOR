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

HALF ADDER

![Screenshot 2024-12-03 183051](https://github.com/user-attachments/assets/337bb328-81e8-4bcb-a97a-016322028ea1)

HALF  SUBTRACTOR

![Screenshot 2024-12-03 182834](https://github.com/user-attachments/assets/8cf0f4cd-a67a-431b-b3b9-1655bac910d4)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: KESHAVARTHINI B RegisterNumber:*/ 24900033

HALF ADDER

module half_adder(a,b,s,ca);

input a,b;

output s,ca;

assign s=a^b;

assign ca=a&b;

endmodule



HALFSUBTRACTOR

module halfsubtractor(a,b,dif,bor);

input a,b;

output dif,bor;

assign dif=a^b;

assign x=~a;

assign bor=b&x;

endmodule

**RTL Schematic**

HALF ADDER

![Screenshot (32)](https://github.com/user-attachments/assets/3b83b690-8af6-4a66-9d5e-85f02a9ca8ee)

HALF SUBTRACTOR

![Screenshot (36)](https://github.com/user-attachments/assets/564feaeb-0722-459b-a293-fcf70f96e189)


**Output/TIMING Waveform**

![Screenshot (31)](https://github.com/user-attachments/assets/59f7b3c8-14e7-4a1f-85a6-2ba71cc0dfbb)

![Screenshot (37)](https://github.com/user-attachments/assets/80dd7022-df22-4886-b4ff-3bb7a689f7ee)



**Result:**

Thus the Half Adder and Half Subtractor circuits are designed and the truth tables is verified using Quartus software.
