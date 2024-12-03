# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

F1:
```

module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```



F2:
```


module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Shyam Gideon 

RegisterNumber:24900637*/


**RTL realization**
F1:

![6ff32893-65c5-49e8-927b-59bca58f9ffb](https://github.com/user-attachments/assets/890e5ce1-28f3-4413-90f4-3ca61996c5ae)

F2:

![bd89d118-f8a3-4e66-85b9-9a3be323caa1](https://github.com/user-attachments/assets/327be48a-b85f-4703-b3ab-5add4a011b69)

**Output:**


**RTL**

**Timing Diagram**

![265878cc-04ce-4bc5-b70b-8c90f74f29dc](https://github.com/user-attachments/assets/fbf683e1-db85-4db9-9d68-5bfc567e196f)

![c68ba7ee-d0be-4152-aa83-94bf218cec31](https://github.com/user-attachments/assets/f4481398-b342-4bfc-9ca1-294a124a2ae8)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

