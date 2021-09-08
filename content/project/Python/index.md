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

`Error:`  
if 5 > 2:  
print("Five is greater than two!")

`Correct:`  
if 5 > 2:  
    print("Five is greater than two!")

<br>

> Comments

There are two ways to include comments, that won't be shown when ran.

`Hashtag:`  
#This is a comment  
print("XXX")  
  
or  
  
`Quotes:`  
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
```

Multiple values to multiple variables:  
```
x, y, z = "Guava", "Banana", "Papaya"

print(x)
print(y)
print(z)
```
One value to multiple variables:  
```
x = y = z = "Strawberry"

print(x)
print(y)
print(z)
```
