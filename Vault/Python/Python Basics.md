#python #basic_syntax 
## Table of Contents
- [[#Comments]]
	- [[#Single-Line Comments]]
	- [[#Multi-Line Comments]]
- [[#Print Command]]
- [[#Variables and Operators]]
	- [[#Creating and Defining Variables]]
	- [[#The Assignment Operator]]
	- [[#Basic Operators]]
	- [[#Shorthand Operators]]
	- [[#Comparison Operators]]
	- [[#Logical Operators]]
- [[#Data Types]]
## Comments

```python
#prints the words "Hello World"
print('Hello World')
```
### Single-Line Comments
In python, comments are created by using the `#` symbol. Comments are used to explain the code and make it easier to understand. Comments are ignored by the python interpreter and are not executed. The # is used to create a single line comment.

```python
#this is a comment
#this is also a comment
#single-line comments are good for brief notes
```
### Multi-Line Comments
 To create a multi-line comment, you can use triple quotes `'''` or `"""`. This is useful when you want to write a comment that spans multiple lines, such as a detailed explanation of a function or a block of code. Multi-line comments are also known as docstrings, which are used to document functions, classes, and modules in Python.

```python
'''This is a multi-line comment. It can span multiple lines and is typically used to create docstrings, which are used to provide detailed explanations of functions, classes, and modules in Python.'''
```
## Print Command
In Python, the "print" command is used to output to the console or terminal. The print command can be used to display text, numbers, variables, and expressions. The syntax for the print command is as follows:

```python
print('Hello World')
```

Note that in order to print text, which is known as a string, text must be enclosed in either single quotes ' ' or double quotes " ". Printing numbers or variables does not require quotes.

## Variables and Operators

### Creating and Defining Variables
Variables are names given to pieces of data that we want to store and manipulate in our programs. Variables can store any type of data, and unlike other programming languages, you do not usually need to declare the type of a variable in Python. Variables are created by assigning a value to a name using the `=` operator.

```python
userAge = 43
userName = 'Joel'
print(userAge, userName)
```

Once a variable is created and a value is assigned to it, the value is stored in memory. This variable (and its value) can then be "called" by referring to it by name. The value of a variable can also be reassigned using `=`.

Multiple variables can be initialized and defined in one line by separating the variables with a comma:

```python
userAge, userName = 43, 'Joel'
print(userAge, userName)
```
### Naming Variables
Variable names can only contain letters (lowercase or uppercase), numbers or underscores. However, the first character of a variable cannot be a number.

```python
userName = 'John'
user_name = 'John'
print(userName, user_name)
```

`2username = "John"` is an invalid variable name because it starts with a number

Variable names are also case sensitive, so `userName` and `UserName` would be different variables. In Python, variables are usually created using camel case or underscores. Camel case is the practice of making compound words using mixed casing (`userName`), while underscores use a `_` to separate words. Sometimes these are combined, such as in `user_Name`. Which naming convention you use is not really important, so long as you are consistent. 
### The Assignment Operator
In programming, the `=` sign is called the assignment operator, because it is used to assign a value to variables. This differs from how the `=` is used in math. The `=` sign assigns the value on the right side to the variable on the left.

```python
x = 5
y = 10
x = y
print('x =', x)
print('y =', y)
```
This code will output:
x = 10
y = 10 

Although x has an initial value of 5 and y has an initial value of 10, the third line assigns the value of y to x, making x = 10, while y remains unchanged.
### Basic Operators
Besides the assignment operator, Python also uses the basic mathematical operators `+`,`-`,`*`, `/`, `//`, `%`, and `**`, which represent addition, subtraction, multiplication, division, floor division, modulus, and exponent.

```python
x = 5
y = 2

#Addition
print(x + y) #prints 7

#Subtraction
print(x - y) #prints 3

#Multiplication
print(x * y) #prints 10

#Division
print(x / y) #prints 2.5

#Floor Division (rounds down to the nearest whole number)
print(x // y) #prints 2

#Modulus (returns the remainder of the division)
print(x % y) #prints 1

#Exponent (raises the first number to the power of the second number)
print(x ** y) #prints 25 (5^2 or 5*5)
```
### Shorthand Operators
In addition to the basic math operators, Python (and other programming languages) also use shorthand operators, which combine a math operator with the assignment operator. For example, `+=` is a shorthand operator that adds the value on the right to the variable on the left. This is equivalent to `x = x + y`.

```python 
x = 5
y = 2

x += y
print(x) 
#This will print 7, because x += y is equivalent to x = x + y

x -= y
print(x)
#This will print 5, because x -= y is equivalent to x = x - y

x *= y
print(x)
#This will print 10, because x *= y is equivalent to x = x * y

x /= y
print(x)
#This will print 5.0, because x /= y is equivalent to x = x / y

```
### Comparison Operators
In addition to math operators, Python also uses comparison operators, such as `==`, `!=`, `>`, `<`, `>=`, and `<=`. These operators are used to compare two values and return a boolean value (True or False) based on the comparison.

```python
x = 5
y = 2

#Equality operator (checks if two values are equal)
print(x == y) #prints False

#Inequality operator (checks if two values are not equal)
print(x != y) #prints True

#Greater than operator (checks if the first value is greater than the second)
print(x > y) #prints True

#Less than operator (checks if the first value is less than the second)
print(x < y) #prints False

#Greater than or equal to operator (checks if the first value is greater than OR equal to the second)
print(x >= y) #prints True

#Less than or equal to operator (checks if the first value is less than OR equal to the second)
print(x <= y) #prints False
```
### Logical Operators
Python also uses logical operators, such as `and`, `or`, and `not`, to combine multiple conditions and return a boolean value based on the result. 

```Python
x = 5
y = 2
z = 7

#And operator (returns True if both conditions are True)
print(x > y and x < z) #prints True

#Or operator (returns True if at least one condition is True)
print(x > y or x > z) #prints True

#Not operator (returns True if the condition is False)
print(not x > y) #prints False
```
## Data Types
In Python, every variable has a data type, which determines what kind of value it is and how it can be used. Python has several built-in data types, including integers, floats, strings, lists, tuples, dictionaries, and booleans.
### Integers
Integers are whole numbers, such as -1, 0, 1, 2, 3, etc. Integers can be positive or negative, but they cannot have decimal points. The Python interpreter automatically interprets numbers without decimal points as integers, so you do not need to specify the data type in most cases. However, you can explicitly define an integer by using the `int()` function. This is useful for certain use cases, such as converting a string to an integer.
```python
x = 5
y = -10
z = str(20) #here z is a string
z = int(z) #now z is an integer)
print(x, y, z)
```
### Floats
Floats are numbers that have decimal points, such as 2.5, 3.14, etc. Floats can be positive or negative. Like integers, floats are automatically interpreted by the Python interpreter, but you can explicitly define a float using the `float()` function.
```python
x = 3.14
y = -2.5
z = 5.5
print(x, y, z)
```
### Characters and Strings
Characters and strings are used to represent text in Python. Characters are single letters or symbols, while strings are sequences of characters. Strings are enclosed in either single quotes ' ' or double quotes " ". Strings can contain letters, numbers, symbols, and spaces. 
```python
char = 'a'
string = "Hello, World!"
print(char, string)
```

Strings can be joined together using the `+` operator, which is known as concatenation. 
```python
string1 = 'Hello, '
string2 = 'World!'
string3 = string1 + string2
print(string3)
```

Although concatenation is useful, it can be cumbersome and make code difficult to read, especially when working with long strings or multiple  variables of different types. For this reason, Python also supports string interpolation, or formatted strings (f-strings), which allows you to insert variables directly into a string using the `f` prefix and curly braces `{}`. 
```python
name = 'Alice'
age = 25
print(f'My name is {name} and I am {age} years old.')
```
#### String Manipulation
There are many ways to manipulate strings in Python. Some common string operations include:
- `len()`: Returns the length of a string
- `lower()`: Converts a string to lowercase
- `upper()`: Converts a string to uppercase
- `strip()`: Removes whitespace from the beginning and end of a string
- `replace()`: Replaces a substring with another substring
- `split()`: Splits a string into a list of substrings based on a delimiter
- `join()`: Joins a list of strings into a single string
```python
string = ' Hello, World! '
print(len(string)) #prints 15
print(string.lower()) #prints ' hello, world! '
print(string.upper()) #prints ' HELLO, WORLD! '
print(string.strip()) #prints 'Hello, World!'
print(string.replace('World', 'Alice')) #prints ' Hello, Alice! '
print(string.split(',')) #prints [' Hello', ' World! ']
print(','.join(['Hello', 'World'])) #prints 'Hello,World'
```
	
