## Conditional Statements

So far all code has executed sequentially, the top line is evaluated then the next, etc.  Control structures let you change the order of how your code executes (often refered to as the program's control flow).  The first control structures you will learn are conditional statements which allows for the conditional executotion of a block of code based on the value of a variable or expression.

#### The If Statement
The if statement checks the condition it is given and if it is true it evaluates the code inside of it (the code that is tabbed over) and if it is not it moves on.
```` python
if condition: 
    print("Condition is true")
    
if (1 < 3): 
    print("1 is less than 3")
````
Syntax matters here, python uses whitespace (tabs) to determine what is contained by the if statement.  Also be aware that the end of the if statement is denoted by a colon.  While not required surrounding your condition in parenthesis will help to reduce errors in your code.

#### Else / Elif
Else and elif can be used to extend the if statement to give you a choice between several statements:
elif allows you to specify other conditions to check and else is evaluated if none of the above if/elif conditions are true 
````python 
hour = 21
if hour <= 11: 
    print("It is morning")
elif hour == 12:
    print("It is noon")
elif hour < 20: 
    print("It is evening")
else:
    print("It is night")
````
##### Grouping Statements
Python allows you to place if statements within if statements to further control the flow of your code, this is called nesting.  When doing nested conditionals your indentation is very important.
````python
x = 1
y = -5
if (x != y):
    print("X and Y are not equal")# This line will print
    if(x < y):
        print("X is less than Y") 
    else: 
        print("X is greater than Y") #This line will print
else:
    print("X and Y are equal")
````

