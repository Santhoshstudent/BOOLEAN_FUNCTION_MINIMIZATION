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

Developed by: santhosh kumar B

RegisterNumber:212223230193

```
module boolean_function_minimization(a, b, c, d, w, x, y, z, f1, f2);
 input a, b, c, d, w, x, y, z;
 output f1, f2;
 wire x1, x2, x3, x4, x5, x6, x7, x8, x9, x10;
 assign x1 = (~a) & (~b) & (~c) & (~d);
 assign x2 = (a) & (~c) & (~d);
 assign x3 = (~b) & (c) & (~d);
 assign x4 = (~a) & (b) & (c) & (d);
 assign x5 = (b) & (~c) & (d);
 assign f1 = x1 | x2 | x3 | x4 | x5;
 assign x6 = (x) & (~y) & (z);
 assign x7 = (~x) & (~y) & (z);
 assign x8 = (~w) & (x) & (y);
 assign x9 = (w) & (~x) & (y);
 assign x10 = (w) & (x) & (y);
 assign f2 = x6 | x7 | x8 | x9 | x10;
 endmodule
```


**RTL realization**

![437749264-2b39f061-05be-4cbd-93cd-8b0b49d6d7af](https://github.com/user-attachments/assets/1e8ec21f-4fcf-4607-8756-a2baeacb4d41)

**Output:**

**RTL**

**Timing Diagram**
![437749301-bca58575-fe61-4810-9882-4d5b2ac76e62](https://github.com/user-attachments/assets/796a36b3-c0a1-4f12-a4b1-14092acbcf24)

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

