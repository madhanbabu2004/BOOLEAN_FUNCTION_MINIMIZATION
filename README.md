# EX NO:2 BOOLEAN_FUNCTION_MINIMIZATION

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

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

```
module Exp2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule

```

**RTL realization**


![Screenshot 2024-10-03 110649](https://github.com/user-attachments/assets/6d471a06-c677-489c-8011-094c96b6e9d9)


**Truth Table**

![image](https://github.com/premalatha-sureshbabu/BOOLEAN_FUNCTION_MINIMIZATION/assets/120620842/a903ec9e-14cc-4fef-8203-65a27c73363a)

**Timing Diagram**


![Screenshot 2024-10-03 110353](https://github.com/user-attachments/assets/a882a214-c28d-433b-846f-7655f9d9635d)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
