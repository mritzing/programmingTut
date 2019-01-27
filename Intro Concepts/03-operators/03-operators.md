## Operators

In programming operators are special symbols that manipulate the values of operands
```
1 and 4 are the operands and + is the operator
1 + 4 = 5
```

### Operator Types
For getting started these are some of the operator types you should be aware of: 
* Arithmetic 
* Assignment
* Comparison
* Logical

#### Arithmetic

| Operator | Name           | Example | Result                                                       |
|----------|----------------|---------|--------------------------------------------------------------|
| +        | Addition       | x+y     | Sum of x and y                                               |
| -        | Subtraction    | x-y     | Difference of x and y                                        |
| *        | Multiplication | x*y     | Product of x and y                                           |
| /        | Division       | x/y     | Quotient of x and y                                          |
| %        | Modulus        | x%y     | Remainder of x divided by y                                  |
| **       | Exponent       | x**y    | x to the power y                                             |
| //       | Floor division | x//y    | Quotient of x and y rounded down to the nearest whole number |

#### Assignment
Assignment variables are shorthand for preforming other operations

| Operator | Example | Description                                                                          | Expression |
|----------|---------|--------------------------------------------------------------------------------------|------------|
| +=       | x+=y    | Assigns the left value (x) to itself plus the right value (y)                        | x = x + y  |
| -=       | x-=y    | Subtracts the two numbers and assigns the result to the left operand                 | x = x - y  |
| *=       | x*=y    | Multiplies the two numbers and assigns the result to the left operand                | x = x * y  |
| /=       | x/=y    | Divides the two numbers and assigns the result to the left operand                   | x = x / y  |
| %=       | x%=y    | Calculates the modulus of the two numbers and assigns the result to the left operand | x = x % y  |
| **=      | x**=y   | Evaluates x to the y power and assigns the result to the left operand                | x = x ** y |

#### Comparison
Comparison operators are boolean expressions meaning that they will return either True or False

| Operator | Example | Description                                                                          | Expression |
|----------|---------|--------------------------------------------------------------------------------------|------------|
| +=       | x+=y    | Assigns the left value (x) to itself plus the right value (y)                        | x = x + y  |
| -=       | x-=y    | Subtracts the two numbers and assigns the result to the left operand                 | x = x - y  |
| *=       | x*=y    | Multiplies the two numbers and assigns the result to the left operand                | x = x * y  |
| /=       | x/=y    | Divides the two numbers and assigns the result to the left operand                   | x = x / y  |
| %=       | x%=y    | Calculates the modulus of the two numbers and assigns the result to the left operand | x = x % y  |
| **=      | x**=y   | Evaluates x to the y power and assigns the result to the left operand                | x = x ** y |

#### Logical
Logical operators are also boolean expressions, but logical operators preform comparisons on boolean values.  
If you want to learn more about how these operators evaluate you can look up their truth tables (Google image search "and truth table").  

| Operator | Example   | Result                        |
|----------|-----------|-------------------------------|
| and      | (x and y) | True if both x and y are true |
| or       | (x or y)  | True if either x or y is true |
| not      | not(x)    | Returns the opposite of x     |

#### Example Code:
````python
# You can save and run this code as a .py file or run it in the python terminal 
x = 1
y = 2
print(x == y) # this will print false
print(x <= y) # this will print true
# Because these expressions evaluate to booleans (True/False) you can use them with the logical operators 
print((x <= y) and (x == y)) # this will print false because the second operand is not true
print((x <= y) or (x == y)) # this will print true because or is looking for at least one operand to be True
````
