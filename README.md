# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: NIVETHA K 
RegisterNumber: 212222230102
```
half adder:

module halfadder(a,b,s,c);
input a,b;
output s,c;
xor (s,a,b);
and (c,a,b);
endmodule
```
```
full adder:

module fulladder(a,b,ci,s,co);
input a,b,ci;
output s,co;
wire d,e,f;
xor (d,a,b);
xor (s,d,ci);
and (f,a,b);
or (co,e,f);
endmodule
```

Logic symbol & Truthtable

RTL realization

half adder:

![HAD](https://user-images.githubusercontent.com/119559844/231478947-e4607ba6-ff2e-4410-9df6-315e45f2d356.png)

full adder:

![FAD](https://user-images.githubusercontent.com/119559844/231479034-c56d3d00-f48b-49ca-b0bd-fe558d075fed.png)

TIMING DIAGRAM:

half adder:

![HA ](https://user-images.githubusercontent.com/119559844/231479724-a4500f47-c569-424b-8b2d-cbd526ec6415.png)

full adder:

![FA ](https://user-images.githubusercontent.com/119559844/231479778-b868f13b-b57d-4c56-ab82-90a703444d8f.png)

TRUTH TABLE:

half adder:

![PODA](https://user-images.githubusercontent.com/119559844/231479181-c4710442-6410-4524-a518-0624b5683646.png)

full adder:

![TTF ](https://user-images.githubusercontent.com/119559844/231479228-a58847cc-11d8-4463-8648-07a98ab13319.png)

### Result:

Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified
