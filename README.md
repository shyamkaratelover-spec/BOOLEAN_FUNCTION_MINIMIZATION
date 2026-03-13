AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

F2=xy’z+x’y’z+w’xy+wx’y+wxy

Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

Theory

Logic Diagram:

<img width="730" height="896" alt="Screenshot 2026-03-12 161218" src="https://github.com/user-attachments/assets/2b46e2de-7589-4a4e-98cd-7bdc61049d40" />


Procedure

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

Program:

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
~~~
Developed by: SHYAM .M
RegisterNumber: 212225220096
~~~
~~~
module exp2(
input A,B,C,D,
output F
);
assign F=(~A & ~B & ~C & ~D) | 
			( A & ~C & ~D)		  |
			(~B &  C & ~D)      |
			(~A &  B &  C &  D) |
			( B & ~C &  D);
endmodule
~~~
RTL realization

Output:

RTL

<img width="1920" height="1080" alt="Screenshot (153)" src="https://github.com/user-attachments/assets/f86fa097-efbd-482b-8e2a-5aa9e0c97875" />\

Timing Diagram

<img width="1920" height="1080" alt="Screenshot (151)" src="https://github.com/user-attachments/assets/16cab7bd-6bad-401e-850f-c96b2f008ea2" />

Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
