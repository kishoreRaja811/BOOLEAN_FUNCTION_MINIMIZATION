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

Developed by:kishore.r RegisterNumber:*/24900772

i)function 1



    module funct1(a,b,c,d,f1);
    input a,b,c,d;
    output f1;
    assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
    endmodule



ii)function 2


    module funct2(w,x,y,z,f2);
    input w,x,y,z;
    output f2;
    assign f2=((~y & z)|( w & y )|(x & y));
    endmodule



**Truthtable**


![Screenshot 2024-12-09 140517](https://github.com/user-attachments/assets/c6823dbb-2dc7-4882-8c2e-d2f35479f259)


**RTL**


![Screenshot 2024-12-09 140601](https://github.com/user-attachments/assets/c374688f-f9d8-4604-bf81-906ec1a0ce9c)


**output**


![Screenshot 2024-12-09 140643](https://github.com/user-attachments/assets/85b6a3a5-5b55-4d4c-a84b-8755e910ebd6)

**Timingdaigram**


![Screenshot 2024-12-09 140724](https://github.com/user-attachments/assets/b0a00119-e7a7-457e-9009-602b934552e4)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

