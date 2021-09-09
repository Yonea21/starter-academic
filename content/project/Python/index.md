---
title: Python
summary: Following John's module 
tags:
- PiBS
date: 27-06-2020

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by David Clode on Unsplash
  focal_point: Smart

links:
- icon: linkedin
  icon_pack: fab
  name: 
  url: https://www.linkedin.com/in/yonea-koch-2543a0219/
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
---

> Get started

After you [download](https://www.python.org/downloads/) Python, search `IDLE` in your PC and create a new file.

<br>

> Syntax

`print("This is an example.")`
The highlighted above shows the syntax. The command `print` must be written in lower case. The printed as a text must be in quotes.

<br>

> Identation

Indentation refers to the spaces at the beginning of a code line.
Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important.
Python uses indentation to indicate a block of code.

Error:  
```
if 5 > 2:  
print("Five is greater than two!")
```

Correct:
```  
if 5 > 2:  
    print("Five is greater than two!")
```

<br>

> Comments

There are two ways to include comments, that won't be shown when ran.

Hashtag:
```  
#This is a comment  
print("XXX")  
```
 
or  
  
Quotes:  
```
"""
multiple
line
comment
"""
```

<br>

> Variables

You assign a value to the created variable. Otherwise Python has no command for detecting a variable.  

```
x = 5
y = "John"

print(x)
print(y)

run

5
John
```

Multiple values to multiple variables:  
```
x, y, z = "Guava", "Banana", "Papaya"

print(x)
print(y)
print(z)

run

Guava
Banana
Papaya
```

One value to multiple variables:  
```
x = y = z = "Strawberry"

print(x)
print(y)
print(z)

run

Strawberry
Strawberry
Strawberry
```

Extract values:
```
fruits = ["apple", "berry", "cherry"]
x, y, z = fruits

print(x)
print(y)
print(z)

run

apple
berry
cherry
```
<br>

> Output Variables

The Python print statement is often used to output variables.
To combine both text and a variable, Python uses the `+` character:

```
x = "awesome"
print("Python is " + x)

run

Python is awesome
```
```
x = "awesome"
print("Python is " + x + ".")

run

Python is awesome.
```

Combine variables:
```
x = "Python is "
y = "awesome."
z = x + y
print(z)

run

Python is awesome.
```

Instead of using String (texts) use Integer (numbers). Then the `omen` works as a mathematical operator. I played with some examples:
```x = 5
y = 10
print(x+y)

x = 5
y = 10
print(x*y)

x = 5
y = 10
print(x/y)

x = 5
y = 10
print(x-y)

x = 5
y = 10
print(x<y)

x = 5
y = 10
print(x>y)

x = 5
y = 10
print(x==y)

x = 5
y = 10
print(x<=y)

x = 5
y = 10
print(x>=y)

run

15
50
0.5
-5
True
False
False
True
False
```

Error, you cannot combine a string and a number:
```
x = 5
y = "John"
print(x+y)

run

TypeError: unsupported operand type(s) for +: 'int' and 'str'
```
<br>

> Global Variables

Variables that are created outside of a function (as in all of the examples above) are known as global variables.
Global variables can be used by everyone, both inside of functions and outside.

Create a variable outside of a function, and use it inside the function:
```
x = "awesome."

def myfunc():
    print("Python is " + x)

myfunc()

run

Python is awesome.
```

If you create a variable with the same name inside a function, this variable will be local, and can only be used inside the function. The global variavle with the same name will remain as it was, global and with the original value. 
```
x = "awesome."

def myfunc():
    x = "fantastic."
    print("Python is " + x)

myfunc()

print("Python is " + x)

run

Python is fantastic.
Python is awesome.
```

Use the global keyword:
```
x = "awesome."

def myfunc():
    global x
    x = "fantastic."
    print("Python is " + x)

myfunc()

print("Python is " + x)

run

Python is fantastic.
Python is fantastic.
```
<br>

Built-in Data Types
======================

> Text Type:
```
str
```

> Numeric Types:
```
int
float
complex
```

> Sequence Types:
```
list
tuple
range
```

> Mapping Type:
```
dict
```

> Set Types:
```
set
frozenset
```

> Boolean Type:
```
bool
```

> Binary Types:
```
bytes
bytearray
memoryview
```

Example with `type()` function:
```
x = 5
print(type(x))

run

<class 'int'>
```
(numeric type, integer)

<br>

In the following graph you see the data structure:

![Data Structure](datagraph.png "<b>Data Structure</b> (Module 2)")

Setting data type example:
```
x = {"name" : "John", "age" : 36}
print(x)

print(type(x))

run

{'name': 'John', 'age': 36}
<class 'dict'>
```

Setting specific data type example:
```
x = dict(name="John", age=36)
print(x)
print(type(x))

y = bool(5)
print(y)
print(type(y))

run

{'name': 'John', 'age': 36}
<class 'dict'>

True
<class 'bool'>
```
<br>

capitalize()
=====

In Python, the capitalize() method returns a copy of the original string and converts the first character of the string to a capital (uppercase) letter while making all other characters in the string lowercase letters.

```
name = ("yO Me LlamO...")
print(name.capitalize())

run

Yo me llamo...
```

"python for dummies" becomes "PythonForDummies":
```
name1 = "python"
name2 = "for"
name3 = "dummies"
print(name1.capitalize() + name2.capitalize()
                         + name3.capitalize())

run

PythonForDummies
```
<br>

count()
====

Shows the number of times a specified value occurs in a string.
```
Buildings = ["big", "small", "big", "small", "small", "big", "tiny", "big"]

print(Buildings.count("small"))
print(Buildings.count("big"))
print(Buildings.count("tiny"))

run

3
4
1
```
<br>

endswith()
===========
The `endswith()` method returns `true`if a string ends with the specified suffix. If not, it returns `False`.
Example:
```
anything = "Python is fun"
print(anything.endswith("fun"))

run

True
```
and
```
anything = "Python is fun"
print(anything.endswith("n"))

run

True
```
or
```
anything = "Python is fun"
print(anything.endswith("u"))

run

False
```
<br>

find()
=======
This function returns the position of the specified value as a number. For a whole word, it is the first letter in each case.
```
message = "Hello, welcome to my world."

print(message.find("Hello"))
print(message.find(","))
print(message.find("welcome"))
print(message.find("to"))
print(message.find("my"))
print(message.find("world"))
print(message.find("d"))
print(message.find("."))

run

0
5
7
15
18
21
25
26
```
<br>

lower()
=========

The `lower()` method converts all uppercase characters in a string into lowercase characters and returns it.
Example:
```
words = "PYTHON IS FUN"
print(words.lower())

run

python is fun
```
Example 2:

```
firstString = "PYTHON IS AWESOME!"
secondString = "PyThOn Is AwEsOmE!"

if(firstString.lower() == secondString.lower()):
    print("The strings are same.")
else:
    print("The strings are not same.")

run

The strings are same.
```
<br>

replace()
=========

The `replace()` method replaces a specified phrase with another specified phrase.
```
message = "I like New York."
print(message)
print(message.replace("like New York", "prefer Bern"))

run

I like New York.
I prefer Bern.
```
<br>

split()
=======

Splits a text into sperate words.
```
messagetosplit = "I want to split this phrase with python."
print(messagetosplit.split())

run

['I', 'want', 'to', 'split', 'this', 'phrase', 'with', 'python.']
```

Or eliminate unwanted factors:
```
txt = "apple@banana@cherry@orange"
print(txt.split("@"))

run

['apple', 'banana', 'cherry', 'orange']
```
<br>

startswith()
==============

The `startswith()` method returns True if the string starts with the specified value, otherwise False.
```
text = ("Hello, welcome to my world.")
print(text.startswith("He"))

run

True
```
<br>

split()
========

The `stirp()`method removes any leading spaces at the beginning and trailing characters.
![Split cup](split.jpg "<b>Split cup</b> (Photo by Tania Melnyczuk on Unsplash)")
```
myword = "    papaya    "
print("Of all fruits", myword.strip(), "is my favorite.")

or

myword = "   papaya   "
x = myword.strip()
print("Of all fruits", x, "is my favorite.")

run

Of all fruits papaya is my favorite.
```
<br>

upper()
========

The `upper` method returns a string where all characters are in upper case. Symbols and Numbers are ignored.
```
text = "Hello friendo"
print(text.upper())

run

HELLO FRIENDO
```
<br>

Implementing a List and an Array
=================================

**List**
List with an Integer, a String and a nested list:
```
thislist = [5, "banana", "[list, in a, list]"]
for x in thislist:
  print(x)

run

5
banana
[list, in a, list]
```

Merged list:
```
listone = [21,"student",11]
listtwo = ["books","read",33]
print(listone + listtwo)

run

[21, 'student', 11, 'books', 'read', 33]
```

**Array**
The sum of two lists:
```
first = [1,2,3,4,5]
second = [6,7,8,9,10]
print([x + y for x, y in zip(first, second)])

run

[7, 9, 11, 13, 15]
```

**Many usages of List**

> Simple List

```
thislist = ["apple", "banana", "cherry"]
print(thislist)
```
> Access an Item

Positive indexing means to start from the beginning:
```
thislist = ["apple", "banana", "cherry"]
print(thislist[1])

run

banana
```

Negative indexing means to start from the end:
```
thislist = ["apple", "banana", "cherry"]
print(thislist[-1])

run

cherry
```

Return the third, fourth, and fifth item:
```
papaya", "passion fruit", "mango", "star fruit", "grapefruit", "melon", "lychee"]
print(thislist[2:5])

run

['mango', 'star fruit', 'grapefruit']
```

This will return the items from index 0 to index 4.:
```
thislist = ["papaya", "passion fruit", "mango", "star fruit", "grapefruit", "melon", "lychee"]
print(thislist[:4])

run

['papaya', 'passion fruit', 'mango', 'star fruit']
```

> Change an Item





