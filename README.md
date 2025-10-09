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
module loggic_gate(a,b,c1,c2,c3,c4,c5,c6,c7);
input a,b;
output c1,c2,c3,c4,c5,c6,c7;
assign c1=~a;
assign c2=a&b;
assign c3=a|b;
assign c4=~(a&b);
assign c5=~(a|b);
assign c6=a^b;
assign c7=~(a^b);
endmodule
```

Program for logic gates and verify its truth table in quartus using Verilog programming

 Developed by:RAKISHA R
 RegisterNumber: 25008669
 
**Logic symbol & Truthtable**

![Truth table](https://github.com/user-attachments/assets/875f3fe9-9d9b-49e8-a799-85bbf3ca0663)

**RTL realization Output:** 
![Screenshot (33)](https://github.com/user-attachments/assets/eb352c3d-a1d6-4760-9de5-cc2ba17822b3)


**RTL**
<img width="1513" height="823" alt="Screenshot 2025-09-29 161644" src="https://github.com/user-attachments/assets/1da9008f-4220-44e7-a305-ebe0dca82a1d" />

**Result:**
Thus the logic gates are studied and their Truth tables are verified.

