#python #basic_syntax 
## Table of Contents
- [[#Comments]]
	- [[#Single-Line Comments]]
	- [[#Multi-Line Comments]]
- [[#Print Command]]
- [[#Variables and Operators]]
	- [[#Creating and Defining Variables]]
	- [[#The Assignment Operator]]
## Comments

```
#prints the words "Hello World"
print('Hello World')
```
### Single-Line Comments
In python, comments are created by using the `#` symbol. Comments are used to explain the code and make it easier to understand. Comments are ignored by the python interpreter and are not executed. The # is used to create a single line comment.

```
#this is a comment
#this is also a comment
#single-line comments are good for brief notes
```
### Multi-Line Comments
 To create a multi-line comment, you can use triple quotes `'''` or `"""`. This is useful when you want to write a comment that spans multiple lines, such as a detailed explanation of a function or a block of code. Multi-line comments are also known as docstrings, which are used to document functions, classes, and modules in Python.

```
'''This is a multi-line comment. It can span multiple lines and is typically used to create docstrings, which are used to provide detailed explanations of functions, classes, and modules in Python.'''
```
## Print Command
In Python, the "print" command is used to output to the console or terminal. The print command can be used to display text, numbers, variables, and expressions. The syntax for the print command is as follows:

```
print('Hello World')
```

Note that in order to print text, which is known as a string, text must be enclosed in either single quotes ' ' or double quotes " ". Printing numbers or variables does not require quotes.

## Variables and Operators

### Creating and Defining Variables
Variables are names given to pieces of data that we want to store and manipulate in our programs. Variables can store any type of data, and unlike other programming languages, you do not usually need to declare the type of a variable in Python. Variables are created by assigning a value to a name using the `=` operator.

```
userAge = 43
userName = 'Joel'
```

Once a variable is created and a value is assigned to it, the value is stored in memory. This variable (and its value) can then be "called" by referring to it by name. The value of a variable can also be reassigned using `=`.

Multiple variables can be initialized and defined in one line by separating the variables with a comma:

```
userAge, userName = 43, 'Joel'
```

### Naming Variables
Variable names can only contain letters (lowercase or uppercase), numbers or underscores. However, the first character of a variable cannot be a number.

```
userName = 'John'
user_name = 'John'
```

`2username = "John"` is an invalid variable name because it starts with a number

Variable names are also case sensitive, so `userName` and `UserName` would be different variables. In Python, variables are usually created using camel case or underscores. Camel case is the practice of making compound words using mixed casing (`userName`), while underscores use a `_` to separate words. Sometimes these are combined, such as in `user_Name`. Which naming convention you use is not really important, so long as you are consistent. 
### The Assignment Operator
In programming, the `=` sign is called the assignment operator, because it is used to assign a value to variables. This differs from how the `=` is used in math. The `=` sign assigns the value on the right side to the variable on the left.

```
x = 5o
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

```
x = 5, y = 2

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
```

