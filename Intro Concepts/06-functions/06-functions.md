## Functions

A function is a block of code that runs when it is called.  Data, called parameters, can be passed into functions.  Functions can also return values.

Functions are useful when you are doing the same operation repeatedly because you only need to write the function once and then call it as many times as you need.  Writing code with functions also helps because if you need to change the function you change it in one place vs if you didn't use a function for your operation you would need to change it everywhere it appeared.
##### Creating a function
The following function consists of its name "first_function" , this function does not take in any parameters so the parenthesis are empty "()" , then print("Hello world!") is the code that is run every time that function is called.
````python
def first_function():
    print("Hello world!")
# to call the function write the name followed by ()
first_function();  #Prints hello world
````
##### Parameters
Parameters are specified after the function name inside the parenthesis.  You can add as many parameters as you want seperated by commas.  
The following function has one paremeter named "name" that is used to form the print statement.
````python 
def hello_function(name):
    print("Hello " + name)

hello_function("Matt") # prints   "Hello Matt"
hello_function("Zoey") # prints   "Hello Zoey"
````
You can also specify a default parameter, if the function is called without passing a parameter it uses the default value.
````python 
def hello_function(name = "Dave"):
    print("Hello " + name)

hello_function("Matt") # prints   "Hello Matt"
hello_function() # prints   "Hello Dave"
hello_function("Zoey") # prints   "Hello Zoey"
````

##### Return Values
One of the main ways you will be using functions is to preform operations on a parameter and then return a result.  In the example below the thing that is printed is the return value of the function called, so three times the parameter.
Note: A return statement in a function will break you out of the function completely, meaning it will return you back to where you were when you called the function.  If there is code past your return keyword in your function it will not be evaluated.
````python
def timesthree(x):
  return 3 * x
  
print(timesthree(3)) # will print 9
print(timesthree(5)) # will print 15
# because it returns a number the function can be treated as a number
print(timesthree(timesthree(3))) # will print 27
````