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

/*
//Program to compute the function f1=a'b'c'd'+ac'd'+b'cd'+a'bcd+bc'd
//f2=xy'z+x'y'z+w'xy+wx'y+wxy

Developed by: RegisterNumber:212223230032
```
module ex02 (A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(~A)&(~C)&(~D);
assign x3=(~B)&(~C)&(~D);
assign x4=(~A)&(~B)&(~C)&(~D);
assign x5=(~B)&(~C)&(~D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```

![code](https://github.com/bhavatharanisiva7418/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473922/7829e8e5-30f1-495a-97bd-c29602e8bf3e)


**RTL relization**

![output 2](https://github.com/bhavatharanisiva7418/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473922/ee875524-f9f5-417f-aba4-fccf504c7b97)


**Output**

![ex02output](https://github.com/bhavatharanisiva7418/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473922/13debc59-5971-4445-9347-2f1496b28072)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

