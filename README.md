# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit
# BY: VIGNESH.V
# REGISTER NUMBER : 23004027

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
### Program:
# Half Adder:

```
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule
```
# Full Adder

```
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule
```
### TRUTH TABLE: 
Half Adder Circuit:
![Screenshot 2023-12-18 161643](https://github.com/23004027/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138956447/c1e52f63-54d0-439d-b7e2-c9c5984310fc)

Full Adder Circuit:
![Screenshot 2023-12-18 161651](https://github.com/23004027/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138956447/5eae28dc-f9ce-4cc0-aad0-4587e8b84a02)

### RTL:
Half Adder Circuit:
![Screenshot 2023-12-18 161713](https://github.com/23004027/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138956447/5b869572-a565-4f69-ae87-b13c296720cb)

Full Adder Circuit:
![Screenshot 2023-12-18 161727](https://github.com/23004027/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138956447/f88f6d90-d31e-4c45-a636-729a3e0c7b8c)

### Output:
Half Adder Circuit:
![Screenshot 2023-12-18 161801](https://github.com/23004027/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138956447/808e2fca-fc78-48f2-8e81-fa4be872aca6)


Full Adder Circuit:
![Screenshot 2023-12-18 161816](https://github.com/23004027/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138956447/674ce8ea-ad23-4789-be42-23101210ba95)


### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
