# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

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
FULL ADDER

![Screenshot 2025-05-10 211718](https://github.com/user-attachments/assets/d6359252-8f37-4f92-9dd9-c762b61ad1bd)



FULL SUBTRACTOR

![Screenshot 2025-05-10 211824](https://github.com/user-attachments/assets/47be13e3-58eb-4e3e-9807-ae3412cd73a4)






**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
```
     i)FULL ADDER
  
  module fa(a,b,cin,sum,carry);
  input a,b,cin;
  output sum,carry;
  assign sum=( (a ^ b)^cin);
  assign carry= ( (a & b)| ( cin &(a ^ b )));
  endmodule
  
  ii)FULL SUBTRACTOR
  
  module fs(a,b,bin,difference,borrow);
  input a,b,bin;
  output difference,borrow;
  assign difference= ( (a ^ b)^bin);
  assign borrow= ( ( a & b)| ( bin & ((a ^ b ))));
  endmodule
```
```
Developed by:SINDHUJA K
RegisterNumber:212224040320
```
*/

**RTL Schematic**
FULL ADDER
![Screenshot 2025-05-10 211924](https://github.com/user-attachments/assets/fe89aa6c-98f8-4806-bb6a-02bff1d584ca)

FULL SUBTRACTOR
![Screenshot 2025-05-10 212053](https://github.com/user-attachments/assets/e906ea83-a7c7-493a-9128-e7400f4233ea)



**Output Timing Waveform**
FULL ADDER
![Screenshot 2025-05-10 212224](https://github.com/user-attachments/assets/2156c248-0181-43d8-a023-e7dba5af3e9e)


FULL SUBTRACTOR
![Screenshot 2025-05-10 212349](https://github.com/user-attachments/assets/92d376e9-a4a5-4658-b679-99760c9146be)




**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



