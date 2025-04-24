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

Developed by: SANJAY C

RegisterNumber:212224050040

module exp_2(A,B,C,D,F1);
 
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

*/



**RTL realization**

![screenshot(1)](https://github.com/user-attachments/assets/69050508-57ce-4e1a-82aa-c7864c26e4bc)


**Output:**

![screenshot(2)](https://github.com/user-attachments/assets/43304971-04b9-409f-9834-2bdcf6a98bf6)


**RTL**

**Timing Diagram**

![screenshot(3)](https://github.com/user-attachments/assets/f2b69ab2-bb9d-4716-b9f3-3192dec5ac52)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

