# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

 
 
 
## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime


## Theory
 Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

Using AND gate: An AND gate is a fundamental digital logic gate that performs a logical conjunction on its input signals. It produces an output signal only when all of its input signals are high (logic level 1). If any of the input signals is low (logic level 0), the output of the AND gate remains low.

using NOT gate: A NOT gate, also known as an inverter, is a basic digital logic gate that performs the operation of negation on its input signal. In other words, it produces the opposite (complementary) output to its input. If the input is high (logic level 1), the output will be low (logic level 0), and if the input is low, the output will be high.

using OR gate: An OR gate is a fundamental digital logic gate that performs a logical disjunction on its input signals. It produces an output signal when at least one of its input signals is high (logic level 1). The output remains low only if all input signals are low (logic level 0).


## Procedure:

1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.

## Program:
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: REVATHI D
RegisterNumber: 212221240045
```
```
module DE2(a,b,c,d,f1);
input a,b,c,d;
output f1;
wire x1,x2,x3,x4,x5;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign f1=x1|x2|x3|x4|x5;
endmodule
```
## Output:
## RTL

![img1](https://github.com/Revathi-Dayalan/Experiment--02-Implementation-of-combinational-logic-/assets/96000574/1b388794-af60-454b-9537-206461e639f8)

## TRUTH TABLE:

![img3](https://github.com/Revathi-Dayalan/Experiment--02-Implementation-of-combinational-logic-/assets/96000574/679e0839-fc04-4651-ac7b-1264b332f4f7)

## OUTPUT WAVEFORM:

![img2](https://github.com/Revathi-Dayalan/Experiment--02-Implementation-of-combinational-logic-/assets/96000574/e52ebcb9-d9d7-428f-9e0a-c1d1264e3f26)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
