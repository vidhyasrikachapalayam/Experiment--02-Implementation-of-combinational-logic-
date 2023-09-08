# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output. F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

1.AND gate The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB Y= A.B

2.OR gate The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation. Y= A+B


 

## Logic Diagram
## Procedure
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.****


## Program:
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: vidhyasri.k
RegisterNumber:  212222230170
```
module f1(A,B,C,D,F1);

input A,B,C,D;

output F1;

wire p,q,r,s,t;

assign p = (~A & ~B & ~C & ~D);

assign q = (A & ~C & ~D);

assign r = (~B & C & ~D);

assign s = (~A & B & C & D);

assign t = (B & ~C & D);

assign F1 = p | q | r | s | t;

endmodule


## RTL realization
![image](https://github.com/vidhyasrikachapalayam/Experiment--02-Implementation-of-combinational-logic-/assets/119477817/b1549e08-28e4-43b3-a9dc-93c474033808)


## Output:

![image](https://github.com/vidhyasrikachapalayam/Experiment--02-Implementation-of-combinational-logic-/assets/119477817/ce059c22-ab38-435a-bdef-f3c4018ff9c2)

##Truthtable:

![image](https://github.com/vidhyasrikachapalayam/Experiment--02-Implementation-of-combinational-logic-/assets/119477817/6d91327d-e406-4bba-8dee-c7a5b03459f1)


Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
