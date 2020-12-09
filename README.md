# python-basics

## Hello World!

* Print
in Python 2, the "print" statement is not a function,therefore invoked without ()
in Python 3, it is a function, and must be invoked with parentheses.

print("Hello, Python!")
O/P: Hello, Python!

Python uses indentation(use four spaces) for blocks, instead of curly braces.
x = 1
if x == 1:
    # indented four spaces
    print("x is 1.")

O/P: x is 1.	

* Comments
used to explain code and to make the code more readable.
used to prevent execution when testing the code.
Single line Comments starts with a #
# Single line comment used 

Multi-line comment starts with """ and span across lines end with """.
""" Multi-line comment used 
print("Python Comments") """

## Variables and Types
Python is completely object oriented. 
No not need to declare variables nor their type before using them.
Every variable in Python is an object

* Numbers

Python supports integers and floating point numbers (also supports complex numbers)

n1=1
print(n1)
O/P: 1 

For floating point number, you may use one of the following notations
n1=1.11
print(n1)
O/P: 1.11

myfloat = float(7)
print(myfloat)
O/P: 7.0

* Strings

Strings are defined either with a single quote or a double quotes. The difference between the two is using double quotes makes it easy to include apostrophes (whereas these would terminate the string if using single quotes). Additional variations on defining strings are covered in the Python documentation.
https://docs.python.org/3/tutorial/introduction.html#strings

mystring = 'hello'
print(mystring)
O/P: hello

mystring = "hello"
print(mystring)
O/P: hello

mystring = "Don't worry python is easy"
print(mystring)
O/P: Don't worry python is easy

mystring = 'Don't worry python is easy'
print(mystring)
O/P: SyntaxError: invalid syntax

var1 = 1
var2 = 2
output = var1 + var2
print(output)
O/P: 3

string1 = "hello"
string2 = "world"
output = string1 + " " + string2
print(output)
O/P: hello world

Mixing operators between numbers and strings is not supported
var1 = 1
var2 = 2
string1 = "hello"

print(var1 + var2 + string1)
O/P: TypeError: unsupported operand type(s) for +: 'int' and 'str'

## Lists
Lists are very similar to arrays, can contain as many variables as you wish and any type of variable.

mylist = [1,2,3,"hello"]
print(mylist)		# O/P: [1, 2, 3, 'hello']
mylist.append(2)	# Add element in list
print(mylist)		# O/P: [1, 2, 3, 'hello', 2]
mylist.remove(2)	# Removes the first matching element
print(mylist)		# O/P: [1, 3, 'hello', 2]

Iterating lists in a very simple manner. 
mylist = [1,2,3]
# prints out 1,2,3
for x in mylist:
    print(x)
	
Accessing List elements
print(mylist[0])  # O/P: 1 		
print(mylist[10]) # an index which does not exist generates an error. 
O/P: IndexError: list index out of range

## Basic Operators

* Arithmetic Operators
Just as any other programming languages, the addition, subtraction, multiplication, division and modulo operators can be used with numbers
number = 1 + 2 * 3 / 4.0 % 2
print(number)	#O/P : 2.5

Using two multiplication symbols makes a power relationship
cube = 2**3
print(cube)	# O/P: 8

Using Operators with Strings
'+' is used for concatenating strings
output = "hello" + " " + "world"
print(output)		# O/P: hello world
 
'*' is used for repeating sequence
output = "Hello" 
print(output*5) #O/P: HelloHelloHelloHelloHello

Using Operators with Lists
'+' is used for joining lists
list1 = [2,4,6,8]
list2 = [1,3,5,7]
output = list1 + list2
print(output)		#O/P: [2, 4, 6, 8, 1, 3, 5, 7]
