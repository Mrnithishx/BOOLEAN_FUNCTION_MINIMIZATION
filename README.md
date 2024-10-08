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
```
Developed by:Nithish D M 
RegisterNumber: 212223230144*/

// Verilog model:Circuit with boolean expressions
module ex02 (E,F,A,B,C,D);
input A, B, C, D;
output E,F;
assign E = A || (B && C) || ((!B) && D);
assign F=((!B) && C) || ( B && (!C) && (!D));
endmodule
```


**RTL realization**
![image](https://github.com/user-attachments/assets/7ce3bebe-a18d-4381-854c-e892e8c2fd58)

**Timing Diagram**
![image](https://github.com/user-attachments/assets/f91a350d-34ba-407c-b38f-49d3d55ac3b5)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

