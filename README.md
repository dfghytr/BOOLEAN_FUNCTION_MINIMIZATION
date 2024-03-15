# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

module combinationalcircuit(A,B,C,D,F1);

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

Developed by:Abdul kalaam k m

RegisterNumber:212223230003

**RTL realization**
![Screenshot 2024-03-15 053028](https://github.com/dfghytr/BOOLEAN_FUNCTION_MINIMIZATION/assets/138970628/ebab94af-6712-4414-a15c-6aca1e69f1b8)





**Truth Table**

![Screenshot 2024-03-15 053040](https://github.com/dfghytr/BOOLEAN_FUNCTION_MINIMIZATION/assets/138970628/7b648fd8-918b-4f9b-b712-72421b45667a)


**Timing Diagram**

![Screenshot 2024-03-15 053054](https://github.com/dfghytr/BOOLEAN_FUNCTION_MINIMIZATION/assets/138970628/5c123af8-65eb-4ca2-844f-53d8eb7af06a)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

