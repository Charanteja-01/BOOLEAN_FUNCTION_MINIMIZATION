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

Developed by:Yedlapalli Charan Teja RegisterNumber:*/212223040247

```
module ex02(A,B,C,D,F1);
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

**Output:**
![319439390-a36158a1-d673-4829-b6f0-6562f939fbb0](https://github.com/Charanteja-01/BOOLEAN_FUNCTION_MINIMIZATION/assets/145693038/42436697-1ec6-4404-a76b-ed73d9f357d7)


**RTL**
![316283051-1c2e6d14-f33b-47ba-98c0-ea594d1a042d](https://github.com/Charanteja-01/BOOLEAN_FUNCTION_MINIMIZATION/assets/145693038/ebe11a2e-b5cf-4d2b-af91-2f1d9ec9b426)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

