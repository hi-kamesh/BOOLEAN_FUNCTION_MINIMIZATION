# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean Function Minimization
Boolean function minimization simplifies digital circuits while preserving functionality. Techniques like Karnaugh Maps (K-Maps), Quine-McCluskey method, and Petrick's method eliminate redundant variables and terms. Benefits include reduced complexity, improved performance, and cost savings. Applications include digital circuit design, computer networks, and embedded systems. Key concepts include minterms, maxterms, and K-Maps. By minimizing Boolean functions, designers create more efficient, reliable, and cost-effective digital systems. This technique is essential in digital electronics and computer science, enabling complex digital system development with reduced complexity and improved performance, leading to better designs.

**Logic Diagram**
![image](https://github.com/user-attachments/assets/812ce8fb-2378-41d8-9dac-768039180603)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
```

module func(a,b,c,d,f1); 
input a,b,c,d; 
output f1; 
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c)); 
endmodule

module func1(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(w&y)|(x&y));
endmodule
```

Developed by:S.KAMESH RegisterNumber:212224230113



**Output:**
![image](https://github.com/user-attachments/assets/88d0074c-b446-461c-a1e6-6c089ce49a4a)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

