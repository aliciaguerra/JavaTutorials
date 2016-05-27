Java provides a rich set of operators to manipulate variables. We can divide all the Java operators into the following groups:
- arithmetic operators
- relational operators
- bitwise operator
- logical operator
- assignment operator
- misc operators

#The Arithmetic Operators
Arithmetic operators are used in mathematical expressions in the same way that they are used in algebra.  The following
table lists the arithmetic operators:

Assume integer variable A holds 10 and variable B holds 20, then:

- +(Addition)
  Adds values on either side of the operator
  A+B will give 30
- -(Subtraction)
  Subtracts right hand operand from left hand operand
  A-B will give -10
- *(Multiplication)
  Multiplies values on either side of the operator
  Example: A * B will give 200
- /(Division)
  Divides left hand operand by right hand operand
  B/A will give 2
- %(Modulus)
  Divides left hand operand by right hand operand and returns remainder.
  B%A will give 0
- ++(Increment)
  Increases the value of operand by 1
  B++ gives 21
- --(Decrement)
  Decreases the value of operand by 1
  B-- gives 19
  
#The Relational Operands
- ==(equal to)
  Checks if the values of two operands are equal or not, if yes than the condition becomes true.
  A==B is not true
- !=(not equal to)
  Checks if the values of two operands are equal or not, if values are not equal than the condition becomes true
  (A!=B) is true
- >(greater than)
  Checks if the value of the left operand is greater than the value of the right operand, if yes the condition becomes true
  A>B is not true
- <(less than)
  Checks if the value of left operand is greater than the value of right operand, if yrs the condition becomes true
  A<B
- >=(greater than or equal to)
  Checks if the value of the left operand is greater than the right operand, if yes then condition becomes true
  A>=B is not true
- <=(less than or equal to)
  Checks if the value of left operand is less than or equal to the value of the right operand, if yes condition becomes
  true. 
  A<=B is true
  
#The BitWise Operators
Java defines several bitwise operators, which can be applied to the integer types, long, int, short, char, and byte.

Bitwise operator works on bits and performs bit-by-bit operation. Assume if a=60 and b=13; now in binary format they
will be as follows. Assume if a=60 and b=13, now in binary format they will be as follows:

a=0011 1100
b=0000 1101

a&b=0000 1100
a|b=0011 1101
a^b=0011 0001
~a=1100 0011

The following table lists the bitwise operators. The variable A holds 60 and variable B holds 13.

- &(bitwise AND)
  Binary AND operator copies a bit to the result if it exists in both operands
  (A&B) will give 12 which is 0000 11000
- |(bitwise OR)
  Binary OR operator copies a bit if it exists in either operand
  (A|B) will give 61 which is 0011 1101
- ^(BitWise XOR)
  Binary XOR operator copies the bit if it is set in one operand but not both. 
  Example: (A^B) will give 49 which is 0011 0001
- ~(bitwise complement)
  Binary ones complement operator is unary and has the effect of flipping bits.
  Example: (~A) will give -61 which is 1100 0011 in 2's complement form due to a signed binary number.
- <<(left shift)
  Binary left shift operator. The left operand value is moved left by the number of bits specified by the right operand.
  Example: A<<2 will give 240 which is 1111 0000
- >>(right shift)
  Binary right shift operator. The left operand's value is moved right by the number of bits specified by the right 
  operand.
  Example: A>>2 will give 15 which 1111
- >>>(zero right fill shift)
  Shift right zero fill operator. The left operands value is moved right by the number of bits specified by the right 
  operand and shifted values are filled with zeros.
  Example: A>>>2 will give 15 which is 0000 1111

#The Logical Operators
Asssuming boolean variable A holds true and variable B holds false

- &&(logical AND)
  Called AND operator. If both the operands are non-zero, then the condition becomes true.
  Example: A&&B becomes false
- ||(logical OR)
  Called logical or operator. If any of the two operands are non-zero, then the condition becomes true. 
  (A||B) is true
- !(logical not)
  Called logical NOT operator. Uses to reverse the logical state of the operand. If a condition is true, then logical
  operand not will make it false.
  !(A&&B) is true

#The Assignment Operators

- =
  Simple assignment operator, assigns values from right side operands to left side operands. 
  C=A+B will assign value of A+B into C
- +=
  Add AND assignment operator, it adds right operand to the left operand and assign the result to the left operand.
  C+=A is equivalent to C=C+A
- -=
  Subtract and assignmnet operator , it subtracts right operand from left nd assign the result to the left operand.
- *=
  Multiply and assignment operator, it multiplies right operand with the left operand and assigns the result to the
  left operand.
  C*=A and is equivalent to C=C*A
- /=
  Divide and assignment operator, it divides left operand with right operand and assign the result to the left operand.
  C/=A is equivalent to C=C/A
  

