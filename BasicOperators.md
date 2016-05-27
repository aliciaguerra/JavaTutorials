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

