## Loops

Loops are another kind of control statement very similar to conditional statements, but are more focused on executing the code repeatedly until its condition is met.

#### While Loop
The while loop is syntactically very similar to the if statement we looked at before, but the code inside the while-loop will loop until the condition becomes false.
So for example this code will print "Condition is true" forever because there is nothing to change the value of the condition variable
````python
condition = True;
while condition:
    print("Condition is true")
print("Out of the loop") # will never print
````
So unless you need an infinite loop for something, the inside of your while loop should operate on the value of the condition it is given
````python
x = 1;
while x < 10: 
    x = x * 2
    print(x)
print("X is greater than 10")
````
The code above would print the following
````
2
4
8
16
X is greater than 10
````
#### For Loop 
The other loop we will look at is the for-loop which is used for iterating over a sequence.
A common use of for loops is to iterate over items in a list (a list is a collection of variables which will be covered more later)
````python
fruits = ['banana', 'apple', 'orange']
for x in fruits:
    print(x)
````
Will print
````
banana
apple
orange
````
The for loop will iterate through every item in the 'fruits' list, x is set to each individual item in order and the code contained is evaluated.  This can be combined with the conditional statements we learned before.
````python
fruits = ['banana', 'apple', 'orange']
for x in fruits:
    if x == 'orange':  
        print("We have oranges") # Will print 
    if x == 'strawberry':
        print("We have strawberries") # Will not print
````
The above code would print "We have oranges".  Below is an example of how you would not want to put if statements inside your for loops.
````python
fruits = ['banana', 'apple', 'orange']
for x in fruits:
    if x == 'orange':  
        print("We have oranges") # Will print 
    else: 
        print("We do not have oranges") # Will print x2
````
The above code would print "We do not have oranges" for every item in the list that isn't an orange, so 'banana' and 'apple'.

For loops can also iterate through a range of numbers.  By default the number inside the range() function starts at zero and increments by one until it reaches the parameter (number inside the parenthesis) specified (note that range(5) will not be the numbers 0-5, but instead 0-4).  You can add a second parameter to change the range to range(startNumber, endNumber), and you can add a third parameter to specific the increment value 
````python 
for x in range(5):
    print(x) # will print 0 1 2 3 4
for x in range(1,4):
    print(x) # will print 1 2 3
for x in range(20, 10, -2):
    print (x) #will print 20 18 16 14 12
````
More on for-loops: https://www.w3schools.com/python/python_for_loops.asp
