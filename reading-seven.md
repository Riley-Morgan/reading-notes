# Operators and Loops
## Operators
-JS has binary and unary operators, and one ternary op (conditional op)
-binary needs two operands, one before and one after, ex: operand1 operator operand2 (3+4)
-unary needs one operand, can be before or after, ex: operator operand (x++)
### Assignment operators 
-assigns a value to left operand based on the value of the right operand
-simple assignment operand is '='. ex: x = y assigns value of y to x.
### Return value and chaining
-assignments have return values, they can be retreived by assing the expression or
logging it (x = y) 
	- const z = (x = y); or const z = x = y
	- console.log(z); // Log the return value of the assignment x = y.
- the return value matches the expression to the right operand
	-x = y returns y
	-x += y returns x + y
	-x /= y returns x / y
	-x ^= y returns x ^ y
-for logical assignments, the return value is that of the logical operation w/o the assignment
	-x &&= y returns x && y
	-x ||=y returns x || y
	-x ??=y returns x ?? y
-return values are always based on the operands' value before the operation
-when changing expressions the assignment is evaluated *right-to-left*
	-w = z = x = y is the same as w = (z = (x = y)) or x = y; z = y; w = y
	-z += x *= y is the same as z += (x *= y)
### Destructuring
-Use this for more complex assignments like arrays
### Comparison Operators
-compares operands and returns a logical value based on if the comparison is true
-operands can be a number, string, logical value, or objective value
-if operands are not the same type, JS will attempt to convert them to an appropriate type
for the comparison
-only exception to type conversion within comparisons involve === and !== ops,
- => is not an operator, its notation for arrow functions
### Arithmetic operators
-takes numerical values as their operands and returns a single numerical value
-standard operators are addition, subtraction, multiplication, and division (+, -, *, /)