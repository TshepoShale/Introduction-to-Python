# Introduction to Python:  

## Week 1:  

## Day 1:  

### What is Python?: 

Python is an interpreted language. This means that a new executable file is created when you run your code. The next time that you execute your code, this new executable file is run instead of the original file. 

It is a relatively simple language that includes a standard library that provides modules for a large number of processes that programs deal with. This approach keeps Python simple yet reliable programming language. Python has an easy-to-use syntax that is focused on the programmer who must type in the program, read what was typed, and provide formal documentation for the program. Python strikes a good balance between fast compilations and readability, and it is easier to write applications. 

Python is implemented in C and relies on the extensive, well understood, portable C libraries. It fits seamlessly with UNIX, Linux, and POSIX environments. Since these standard C libraries are widely available for the various MS-Windows variants, and other non-POSIX operating systems, Python runs similarly in all environments. The Python programming language was created based on lessons learned during language and operating system support. Python is built from concepts in the ABC and Modula-3 languages. 

### Comments in Python:  

Comments are added to make the source code easier to understand. Comments in Python start with the hash character, #, and extend to the end of the physical line. A comment may appear at the start of a line or following whitespace or code, but not within a string literal.  

### Creating Applications using Python:  

Indentation in Python identifies what code belongs to what section of code. 

### Escape Sequences:  

* Backslash character (\):  e.g \\ 

* New line feed: \n 

* Tab: \t 

* Vertical tab: \v 

* Backspace: \b 

* Carriage return: \r 

* Single quote (useful in strings enclosed in single quotes: ‘hello \ ‘World’): \\' 

* Double quote (useful in strings enclosed in single quotes: “hello \ “World”): \\" 

  

  

### Reserved words in Python: 

NB: Cannot be used as ordinary identifiers, must be spelled *EXACTLY* as wriiten here: 

False      class      finally    is         return 

None       continue   for        lambda     try 

True       def        from       nonlocal   while 

and        del        global     not        with 

as         elif       if         or         yield 

assert     else       import     pass 

  

# Python 3.5 keywords (added 'async', 'await', 'asynchronous', 'contextlib', 'async for', 'async with') 

async      await      async def  async for  async with 

asynchronous contextlib 

  

# Python 3.6 keywords (added 'f' for formatted string literals) 

f          False      async      await      True 

  

# Python 3.7 keywords (added 'async' and 'await' as non-keyword identifiers, 'contextvars', 'nonlocal', 'dataclasses') 

async      await      contextvars dataclasses nonlocal 

  

# Python 3.8 keywords (added 'walrus' operator ':=') 

:= 

  

# Python 3.9 keywords (added 'match' statement) 

match 

  

### Anaconda Navigator:  

Anaconda is a popular open-source distribution of Python and other data science-related packages. It simplifies the process of installing, managing, and updating Python libraries for data science, machine learning, and scientific computing. Anaconda includes tools such as conda, a powerful package manager, and provides an environment management system, allowing users to create isolated Python environments for different projects, making it easier to manage dependencies and avoid conflicts between packages. 

  

## Day 2:  

## Variables:  

Variables in programming act as temporary storage spaces in a computer's memory, holding various data values. When a variable's value changes, it affects the program's current state. They serve as containers for different data items, and understanding them is essential for programming. Variables are crucial in all programming languages, allowing data transfer between functions and making programming tasks more manageable. 

Each variable is created with an initial value. A value can be in *THREE* states:  

1. Variable creation (Declaration) 

2. Variable assignment (Initialization) 

3. Variable changed (Execution) 

  

NB: Once the code which created the variable has finished executing, the variable is destroyed. 

  

NB: In Python, variables are defined in a standard way, by using the assignment character (=). This changes the value of the variable. Naming conventions specify the way in which variables should be named. This standard is used to make code more readable, and thus easier to understand. 

  

The rules include the start and continuation characters. Variable names may contain any upper or lower case letter (A–Z, a–z), a number, or the underscore character. They may not begin with a number or contain spaces. Continuation characters are any characters except whitespace characters like tab and space. 

  

Here are a few examples of valid variable names: 

  

* c 

* ref_number 

* admin 

* aVeryLongName 

  

   

Here are a few examples of invalid variable names: 

  

* True 

* $name 

* 12Graph 

  

NB: *In Python identifiers are case sensitive!!!* 

  

NB: *Variables cannot have the same name as Python’s keywords!!!* 

  

We can find out what keywords are in Python, by using the function called dir(). If this function is called with the __builtins__ attribute, it returns a list of Python’s built-in attributes. 

  

The __builtins__ module contains all Python’s built-in attributes, which can be used with the dir()function. 

  

The ones that are returned are identified with the following characteristics: 

  

* Python’s built-in exceptions start with a capital letter. 

* The rest are either functions or data type names. 

* Identifiers that start and end with one or two underscores are special methods. 

  

  NB: *All of the methods, exceptions, and functions contained in   

dir(__builtins__), dir(__doc__), dir(__name__), and dir(__package__) cannot be used as variable names.* 

  

### Using Variables:  

* All variables are assigned to a data type, be it a STRING, or an INTEGER.  

* Values of the same type can be manipulated together. 

* In Python, automatic type conversion, also known as implicit casting, allows the interpreter to automatically convert compatible data types, such as integers to floats or floats to strings, as needed during operations or assignments, simplifying code and enhancing flexibility. 

  

### Casting:  

  

#### Implicit Casting:  

In Python, automatic type conversion, also known as implicit casting, allows the interpreter to automatically convert compatible data types, such as integers to floats or floats to strings, as needed during operations or assignments, simplifying code and enhancing flexibility. Also ensures that no data is lost when these conversions occur.  

  

#### Explicit Casting:  

A value cannot be automatically cast from one data type to another if it will result in data loss. Extra code has to be written to ensure that the value stays the same and only the data type changes; like when casting from a floating-point value to an integer value.  

  

The rules to convert a string to a float are: 

* The string should only contain numbers. 

* Other than numbers the following are allowed: 

* Only one dot (.) character. Indicates the decimal starts after the dot (.) character. 

A ‘+’ or ‘−‘ character at the beginning of the string. This indicates that the number is either positive or negative. 

### Day 3: 
### Lambda Expressions: 
In Python, a lambda function is a small, anonymous (unnamed) function defined using the lambda keyword. Lambda functions are often used for short, simple operations where a full function definition is not necessary. They can take any number of arguments, but they can only have one expression.
Syntax: 
lambda arguments: expression

Example: 
# Using a lambda function to square a number
square = lambda x: x ** 2

# Call the lambda function
result = square(5)
print(result)  # Output: 25

Example 2: 
# Using a lambda function to add two numbers
addition = lambda a, b: a + b

# Call the lambda function
result = addition(3, 7)
print(result)  # Output: 10

### Booleans: 
>>>>The Boolean data type is like a switch that can be either on (1, or True) or off (0, or False). When you write it as words, it's always 'True' or 'False,' not '1' or '0.' In Python, 'True' and 'False' are written with exact capitalization. Booleans help check if things are true or not. There are three ways to do this:

1.The 'and' operator
2.The 'or' operator
3.The 'not' operator"
>>>>Operators and built-in functions that have a Boolean result always return (False or 0) or (True or 1). The Boolean or and and operations always return only one of the options, either True or False.
	Floating point numbers=are decimal values or fraction numbers
	Complex numbers= A complex number consists of a real part and an imaginary part, and it is often written in the form a + bj, where a is the real part and b is the imaginary part. In Python, the imaginary unit is denoted by j.
	Strings=represents a sequence of characters
>>>>
## Day 4: 
### Operators: 

#### Arithmetic Operators:

+ (Addition): Adds two values.
- (Subtraction): Subtracts the right operand from the left operand.
* (Multiplication): Multiplies two values.
/ (Division): Divides the left operand by the right operand (results in a float).
// (Floor Division): Divides the left operand by the right operand and rounds down to the nearest whole number.
% (Modulus): Returns the remainder of the division.

#### Comparison Operators:
== (Equal to): Checks if two values are equal.
!= (Not equal to): Checks if two values are not equal.
< (Less than): Checks if the left operand is less than the right operand.
> (Greater than): Checks if the left operand is greater than the right operand.
<= (Less than or equal to): Checks if the left operand is less than or equal to the right operand.
>= (Greater than or equal to): Checks if the left operand is greater than or equal to the right operand.

#### Logical Operators:
and: Returns True if both operands are True.
or: Returns True if at least one of the operands is True.
not: Returns True if the operand is False and False if the operand is True.
Assignment Operators:

= (Assignment): Assigns the value on the right to the variable on the left.
+=, -=, *=, /=, %=, //=: Perform the operation and assign the result to the variable.

#### Other Operators:
** (Exponentiation): Raises the left operand to the power of the right operand.
in: Returns True if a value exists in a sequence (e.g., list, tuple, string).
is: Returns True if two variables refer to the same object.
not in: Returns True if a value does not exist in a sequence.

## Week 2: 
## Day 1: 

### Control Flows: 

#### Sequencial: 
This flow happens by default. Meaning from the top,downwards. 

#### Selection/ Decision Control: 
eg. else-if statements, if statements, this means testing values or conditions, before executing the instructions. 

#### Repetition: 
eg. while loops. Executes code multiple times. 

## Day 2: 

### Python Functions: 
#### What are needed in Functions?:
* Function name
* List of zero, or more parameters
* Optional piece of code, with return statements.
  NB: A function can return nothing. We normally store functions in script files, because we do not want to type them more than once.
  #### Types of Functions:
  ##### Ordinary Functions:
  These follow mathematical procedures.
  ##### Procedure Functions:
  These are called, to exectue a procedure.
  ##### Factory Functions:
  Do not take parameters, these generate values.
  #### Argument VS. Parameter:
  * Arguments are objects in an application of a function. Can also be referenced by other variables.
  * Parameters are are variable names, that are part of the function, and is a local variable. 
### Random module: 
Generates random floating point numbers as outputs.

#### Examples of random module functions: 

* In Python, the randint() function is part of the random module, which provides functions for generating pseudo-random numbers. Specifically, randint(a, b) generates a random integer between a and b, inclusive.
  Example:
  random.randint(a, b)
  
*  In Python, the sample() function is part of the random module, and it allows you to generate a random sample of unique elements from a given population sequence without replacement.
   Example:
   import random
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
 Generate a random sample of 3 unique numbers from the list
random_sample = random.sample(numbers, 3)
print(random_sample)

* In Python, the choice() function is part of the random module, and it allows you to randomly select an item from a sequence (such as a list, tuple, or string). Choose a random element from a non-empty sequence.
Example:
import random
fruits = ["apple", "banana", "cherry", "orange"]
Choose a random fruit from the list
random_fruit = random.choice(fruits)
print(random_fruit)

* The randrange() function in Python, part of the random module, generates a random number from the specified range.
Example: 
import random
Generate a random number between 1 and 10
random_number = random.randrange(1, 11)
print(random_number)

## Day 3:
### Python Modules: 
These are libraries that contain code, that gives classess, methods, and functions, their functionality. 
NB: The moment a module is imported, the Python interpreter then fetches it from the either the program directory, or in the PYTHONPATH variable. 
NB: You can check module lists using help("modules"). 

## Day 4: 
### Regular Expressions: 
Regular expressions (regex) in Python are a powerful tool for pattern matching and searching in strings. The re module in Python provides support for regular expressions. Regular expressions are used to specify a search pattern, which can be a string or a complex expression, and then this pattern can be used to find matches within strings, replace substrings, or split strings based on the specified pattern.
NB: Use the import re module to utilize RegEx. 

## Week 3: 
## Day 1: 
### List Data-type methods: 

### * list.append(x):
Adds an item to the end of the list. 

### * list.extend(iterable):
Extends list by appending all items from the iterable. 

### * list.insert(i,x): 
Inserts items at a given position. 1st arguments is index of element, before which to insert. Insert, adds it at the front of the list. 

### * list.remove(x):
Returns first item from the list, whose value is equal to x. 

### * list.pop([i]):
Remove item, at a given position, and return it. If no index is specified, a pop() removes and returns the last item in the list. Square brackets mean that the parameter is optional, so you don't need to type square brackets, in that position. 

### * list.clear():
Removes all items from the list. 

### * list.index(x[, start[ end]]):
Returns zero-based in the list of the first item, whose value is equal to x. Optional parameters START and END, are interpreted as the slice notation, and are used to limit the search, to a list. 

### * list.count(x):
Returns the number of times x appears on the list. 

### * list.sort(key = None, reverse = False):
Sorts the items of the list, in place. 

### * list.reverse():
Reverse the elements of the list in place. 

### * list.copy():
Returns shallow copy of the list. 

## Day 3: 
## Errors and Exceptions: 
#### Try-Block: A Safety Net for Your Code

Imagine you're doing a tricky task, like juggling. You might drop the balls, right? In programming, sometimes things can go wrong, too. The try block is like your safety net—it catches the errors and prevents your program from crashing.
How It Works:
1. You put the risky code inside the try block.
2. If everything goes well, Python continues without any problems.
3. If an error happens inside the try block, Python doesn't stop. Instead, it jumps to the except block.
4. In the except block, you can handle the error. Maybe you print a message or do something else to manage the problem.

Example: 
try:
    result = 10 / 0  # Risky code! Dividing by zero causes an error
except ZeroDivisionError:
    print("Oops! Can't divide by zero.")
#### * TypeError: 
Occurs when you try to do something with a data type, that is not allowed. 
#### * SyntaxError: 
When syntax is incorrect. 
#### * NameError: 
When you try to access a function, or variable that has not been defined in the scope. 
#### * AssertationError:
Here you use the 'assert' statement. Raiases an alarm for your code. Maybe your assumption for a condition in your code, probably did not hold. 
Example: 

age = 15
assert >= 18, "Too Young!"
Error Message here would be: 
AssertationError: "Too Young!" 

## Day 4: 
## Classes: 
Classes can have methods, for modifying its state. Creating a new class, creates a new type of instance to be made. 
Methods: Functions assosciatd in a class. 
NB: Instance variables contain data unique to each instance. 
We use the 'pass' statement to create an empty class. The 'pass' keyword can be placed under the class declaration, to let the compiler know that more code, or logic will come underneath there. 

Example: 
class Employee: 
def_ _ init _ _ (self, first, last, pay):
self.first = first
self.last = last 
self.pay = pay 
emp_1 = Employee('Tshepo', 'Shale', 41000) ---> This is an instance of a class. 

 _ _ init _ _ : This is a constructor. It is called when a new instance of a variable is created. 

 * Classes are like blueprints.
 * Attributes within a class, are characteristics.
 * Methods of a class, are actions.
 * Objects, are instances of a class. eg. like a specific car, is an object of a 'Car' class.
 * Encapsulation: classes help you keep related attributes and methods together; making code easier to manage, and understand. 

#### Scopes: 
These are textual regions of a python programme, where a namespace is directly accessible. Basically is a set of rules where you can access, or modify a variable. 
##### * Global Scope: 
Variables defined outside of the function. Can be accessed anywhere in the code. 
##### * Local Scope: 
Variables that exist within the function itself. Cannot be acessed anywhere else, other that inside that function. 

#### Namespaces: 
Mapping from names, to objects. In other words,namespace is like a box where you keep all your variables (names of things), and funcitons (the actions that you do). Same with creating a class; when you create a class, it has its own namespace, to store it's own stuff. eg. Your ID number. 







  

  

  

 

 
