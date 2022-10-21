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
### Program:
~~~
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:Manoj M
RegisterNumber:  212221240027

## Half adder program:

module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

## Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
  
~~~
### output
### Logic symbol & Truthtable

![a](https://user-images.githubusercontent.com/94588708/197108132-5ed554b6-799f-4ac5-bdc1-b81370ac18ea.png)
![b](https://user-images.githubusercontent.com/94588708/197108152-7622191a-8790-4b0c-9a67-bdce07037fb1.png)

### RTL:
#### HALF ADDER:
![e](https://user-images.githubusercontent.com/94588708/197108841-25c71136-1401-4f80-8db1-f405ae174c5a.png)
#### FULL ADDER:
![f](https://user-images.githubusercontent.com/94588708/197108916-989afbc7-cc39-43e2-8f1a-d82503dc4b94.png)


### TIMING DIAGRAM:
#### HALF ADDER:
![c](https://user-images.githubusercontent.com/94588708/197108490-83b92230-d8f3-45fe-9f1f-4c7497bd82f2.png)

#### FULL ADDER:
![d](https://user-images.githubusercontent.com/94588708/197108516-6157b23e-963c-4652-835f-c34f966fa0d7.png)


### TRUTH TABLE :
#### HALF ADDER:
![g](https://user-images.githubusercontent.com/94588708/197109143-7c882df8-f268-4fd1-afa4-f5ad7cceb66d.png)


#### FULL ADDER:
![h](https://user-images.githubusercontent.com/94588708/197109154-2b43618b-8b96-4eac-881b-9ec30e59949c.png)




### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
