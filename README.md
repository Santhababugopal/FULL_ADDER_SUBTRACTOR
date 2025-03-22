

Implementation-of-Full-Adder-and-Full-subtractor-circuit

NAME:  SANTHABABU G

REGISTER NUMBER : 212224040292

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

FULL ADDER:

![full-adder2](https://github.com/user-attachments/assets/c3382a58-a6e5-4686-98da-edb27cf4ce8b)


FULL SUBTRACTOR:

![full subtractor](https://github.com/user-attachments/assets/df9316c9-6162-42f1-b118-0f955f705af6)


**Procedure**
 Write the detailed procedure here

**Program:**

```
module EXP4 (a,b,c,x,y,z,sum,dif,car,bor);
 input a,b,c,x,y,z;
 output sum,dif,car,bor;
assign sum = a^b^c;
 assign car = a&b | a&c | b&c;
 assign dif = x^y^z;
 assign bor = ~x&z | ~x&y | y&z;
 endmodule

```

**RTL Schematic**

![Screenshot 2025-03-22 200920](https://github.com/user-attachments/assets/0ea929ba-9464-42cd-b9e9-ae770bedd30f)

**Output Timing Waveform**

![Screenshot 2025-03-22 201839](https://github.com/user-attachments/assets/b8ce2730-0573-4191-ae30-db362ff379d2)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



