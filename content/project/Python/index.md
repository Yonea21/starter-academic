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

In the following graph you see the different data types:

![Graph 2](graph2.jpg "<b>Graph 2</b> (Module 1.5)")

sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!


