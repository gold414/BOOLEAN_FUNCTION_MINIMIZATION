
# BOOLEAN_FUNCTION_MINIMIZATION
```
Developed by:   THANGAPAZHAM P

RegisterNumber: 25017581
```

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
module logic_functions(
    input  a, b, c, d,
    input  w, x, y, z,
    output f1, f2
);

assign f1 = (~b & ~d) |
            (a & b & ~c) |
            (~a & b & d);

assign f2 = (~y & z) |
            (w & y);

endmodule


```
## Logic symbol & Truthtable:

<img width="805" height="442" alt="table1" src="https://github.com/user-attachments/assets/275d33e2-793e-4bce-aec0-f5b77aaf4929" />

<img width="797" height="421" alt="table2" src="https://github.com/user-attachments/assets/8e19e8ae-4627-4eb6-ba04-18341acd948e" />


**RTL realization**

<img width="996" height="683" alt="Screenshot 2025-11-20 130542" src="https://github.com/user-attachments/assets/f14559d9-d69c-42ab-bf1c-2a0ba5476cd3" />


**Output:**

<img width="1920" height="1080" alt="Screenshot (143)" src="https://github.com/user-attachments/assets/5feaa4b2-850c-462f-a4e0-f9ce306747a5" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
