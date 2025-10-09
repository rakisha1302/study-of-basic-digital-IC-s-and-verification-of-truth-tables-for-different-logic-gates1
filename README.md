### study-of-basic-gates

**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.

**Equipments Required:**

Software – Quartus prime 

**Theory**

Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate

**AND gate**

The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B

**OR gate** 

The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B

**NOT gate**

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'

**NAND gate**

This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’

**NOR gate**

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’

**Ex-OR gate**

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B

**Ex-NOR gate**

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B

**Procedure** 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**PROGRAM**
```
module EXP1 (
    input  wire a,     // Input A
    input  wire b,     // Input B
    output wire and_out,
    output wire or_out,
    output wire not_out,   // only on A
    output wire nand_out,
    output wire nor_out,
    output wire xor_out,
    output wire xnor_out
);

    assign and_out  = a & b;      // AND gate
    assign or_out   = a | b;      // OR gate
    assign not_out  = ~a;         // NOT gate (on input A)
    assign nand_out = ~(a & b);   // NAND gate
    assign nor_out  = ~(a | b);   // NOR gate
    assign xor_out  = a ^ b;      // XOR gate
    assign xnor_out = ~(a ^ b);   // XNOR gate

endmodule


```

Program for logic gates and verify its truth table in quartus using Verilog programming

 Developed by:RAKISHA R
 RegisterNumber: 25008669
 
**Logic symbol & Truthtable**

![Truth table](https://github.com/user-attachments/assets/875f3fe9-9d9b-49e8-a799-85bbf3ca0663)

**RTL realization Output:** 

<img width="1300" height="696" alt="image" src="https://github.com/user-attachments/assets/16c549c1-5fb6-463f-b2e8-c6f3c20f08d7" />

**RTL**
<img width="1513" height="823" alt="Screenshot 2025-09-29 161644" src="https://github.com/user-attachments/assets/1da9008f-4220-44e7-a305-ebe0dca82a1d" />

**Result:**
Thus the logic gates are studied and their Truth tables are verified.

