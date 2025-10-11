# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus II**

**Theory**

 Boolean function minimization is the process of simplifying Boolean algebraic
 expressions to reduce the number of logic gates and complexity in a digital circuit,
 leading to more efficient, faster, and less costly hardware
 For minimizing Boolean expressions,we can use a set of rules and laws (like distributive,
 associative, and complement laws) to simplify Boolean expressions. This method
 focuses on applying algebraic manipulations to reduce the complexity of the expression
 by eliminating redundant terms.
 
 Identity Law A ⋅ 1 = A, A + 0 = A
 
 Null Law A ⋅ 0 = 0, A + 1 = 1
 
 Idempotent Law A ⋅ A = A, A + A = A
 
 Complement Law A ⋅ A′ = 0, A + A' = 1
 
 Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C
 
 De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′
 
 Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A

 Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C
 
 Commutative law A B = B A,A + B = B + A
 
**Logic Diagram**

![WhatsApp](https://github.com/user-attachments/assets/451cd0bb-df44-4482-a7d9-73157f43832c)

![WhatsApp](https://github.com/user-attachments/assets/040f3828-dcd2-4a30-8ca0-9fcb927f3e0e)

![WhatsApp](https://github.com/user-attachments/assets/01468d6a-5082-44d8-ada2-e5e3b7d6263b)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to implement the given logic function and to verify its operations in quartus
 using Verilog programming.
 
 i)
 
 module funct1(a,b,c,d,f1);
 
 input a,b,c,d;
 
 output f1;
 
 assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
 
 endmodule
 
 ii)
 
 module funct2(w,x,y,z,f2);
 
 input w,x,y,z;
 
 output f2;
 
 assign f2=((~y & z)|( w & y )|(x & y));
 
 endmodule
 

**RTL realization**

**Output:**

i)

![UDHAYA](https://github.com/user-attachments/assets/6608910d-bfa1-46da-8053-4ce3ec40a91d)

ii)

![nila](https://github.com/user-attachments/assets/744f5693-9ce0-4b0c-84b1-c167f4eb31e8)

**RTL**

**Timing Diagram**

i)

![wave](https://github.com/user-attachments/assets/6e055b83-030e-4620-a715-40f95ecb4076)

ii)

![form](https://github.com/user-attachments/assets/d9801c4a-d477-4ff1-be8c-4af395f36ac8)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

