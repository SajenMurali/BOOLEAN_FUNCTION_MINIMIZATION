# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

Logic symbol & Truthtable:
![image](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/164154502/6419b712-eb82-4b57-9ffa-5b83f88da36f)
![image](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/164154502/5e4711ba-8a74-45c0-aa6e-32799e57682e)

**RTL realization**
![image](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/164154502/786fd7d5-e479-436c-a6ba-7d8a38f4f412)


**Output:**
![image](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/164154502/12c0d5a6-938a-4631-be7a-7b853e9fb0b0)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

