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
<br>

**List**  
List with an Integer, a String and a nested list:
```
thislist = [5, "banana", "[list, in a, list]"] #syntax requires angular brackets
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
<br>

**Array**  
The sum of two arrays:
```
first = [1,2,3,4,5]
second = [6,7,8,9,10]
print([x + y for x, y in zip(first, second)])

run

[7, 9, 11, 13, 15]
```
<br>

**Many usages of List**  

> Simple List

```
thislist = ["apple", "banana", "cherry"]
print(thislist)
```
> Access an item

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
thislist = ["papaya", "passion fruit", "mango", "star fruit", "grapefruit", "melon", "lychee"]
print(thislist[2:5])

run

['mango', 'star fruit', 'grapefruit']
```

This will return the items from index 0 to index 4:
```
thislist = ["papaya", "passion fruit", "mango", "star fruit", "grapefruit", "melon", "lychee"]
print(thislist[:4])

run

['papaya', 'passion fruit', 'mango', 'star fruit']
```

> Change an item

Replaces the value:
```
thislist = ["pear", "apple", "cherry"]
thislist[1] = "blackcurrant"
print(thislist)

run

['pear', 'blackcurrant', 'cherry']
```

Replaces the value with two new items:
```
thislist = ["pear", "apple", "cherry"]
thislist[1:2] = "blackcurrant", "melon"
print(thislist)

run

['pear', 'blackcurrant', 'melon', 'cherry']
```

The `insert()` method inserts an item at the specified index:
```
thislist = ["pear", "apple", "cherry"]
thislist.insert(0, "meleon")
print(thislist)

run

['meleon', 'pear', 'apple', 'cherry']
```

> Add an item

Using the `append()` method to append an item:
```
thislist = ["apple", "banana", "cherry"]
thislist.append("orange")
print(thislist)

run

['apple', 'banana', 'cherry', 'orange']
```

To append elements from another list to the current list, use the `extend()` method:
```
thislist = ["apple", "banana", "cherry"]
tropical = ["mango", "pineapple", "papaya"]
thislist.extend(tropical)
print(thislist)

run

['apple', 'banana', 'cherry', 'mango', 'pineapple', 'papaya']
```

You also can add any iterable object (tuples, sets, dictionaries etc.):
```
thislist = ["apple", "banana", "cherry"]
thistuple = ("kiwi", "orange")
thislist.extend(thistuple)
print(thislist) 

run

['apple', 'banana', 'cherry', 'kiwi', 'orange']
```

> Remove an item

The `remove()` method removes the specified item:
```
thislist = ["apple", "banana", "cherry"]
thislist.remove("banana")
print(thislist)

run

['apple', 'cherry']
```

Remove specified Index with `pop()`:
```
thislist = ["apple", "banana", "cherry"]
thislist.pop(0)
print(thislist)

run

['banana', 'cherry']
```

If you don't specifiy the `pop()`method, it removes the last item:
```
thislist = ["pear", "lychee", "apple"]
thislist.pop()
print(thislist)

run

['pear', 'lychee']
```

![Fruit](apples.jpg "<b>Fruit</b> (Photo by Jocelyn Morales on Unsplash)")

The `del` keyword also removes the specified index:
```
thislist = ["pear", "lychee", "apple"]
del thislist [0]
print (thislist)

run

['lychee', 'apple']
```

You also can delete the list completely:
```
thislist = ["pear", "lychee", "apple"]
del thislist
print (thislist)

run

NameError: name 'thislist' is not defined
```

Or use `clear()`method to clear the content of the list:
```
thislist = ["pear", "lychee", "apple"]
thislist.clear()
print(thislist)

run

[]
```

> Loop lists

You can loop through the list items by using a `for` loop:
```
thislist = ["pear", "lychee", "apple"]
for x in thislist:
    print(x)

run

pear
lychee
apple
```

Loops trhrough, refering to index number. Creates a suitable iterable with `range()`and `len()`:
```
thislist = ["pear", "lychee", "apple"]
for x in range(len(thislist)):
    print(thislist[x])

run

pear
lychee
apple
```

You can loop through the list items by using a `while` loop. Use the `len()` function to determine the length of the list, then start at 0 and loop your way through the list items by refering to their indexes. Always increase the index by 1 after each iteration.
```
thislist = ["plant", "fruit", "building"]
x = 0
while x < len(thislist):
    print(thislist[x])
    x = x + 1

run

plant
fruit
building
```

> Comprehend items

Based on a list of fruits, you want a new list, containing only the fruits with the letter "a" in the name.
Without list comprehension you will have to write a for statement with a conditional test inside:
```
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
listwitha = []

for x in fruits:
    if "a" in x:
        listwitha.append(x)

print(listwitha)

run

['apple', 'banana', 'mango']
```

The same thing with only one line of code:
```
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
listwithw = [x for x in fruits if "w" in x]
print(listwithw)

run

['kiwi']
```

> Sort items

Objects in a list have a `sort()` method that sort the items alphanumerically, ascending. Alphabetically:
```
mylist = ["¿","que", "esta", "pasando", "en", "este", "mundo", "?"]
mylist.sort()
print(mylist)

run

['?', 'en', 'esta', 'este', 'mundo', 'pasando', 'que', '¿']
```

Numerically:
```
mylist = [654,56465,4312,15468,7621,5,53,2,5,8,9]
mylist.sort()
print(mylist)

run

[2, 5, 5, 8, 9, 53, 654, 4312, 7621, 15468, 56465]
```

With the keyword argument `reverse = True` you can manipulate the sort into descending:
```
mylist = [654,56465,4312,15468,7621,5,53,2,5,8,9]
mylist.sort(reverse = True)
print(mylist)

run

[56465, 15468, 7621, 4312, 654, 53, 9, 8, 5, 5, 2]
```

Keyword argument `key = function` sorts the list based on how close the number is to 15468:
```
def myfunc(n):
    return abs(n - 15468)

mylist = [654,56465,4312,15468,7621,5,53,2,5,8,9]
mylist.sort(key = myfunc)
print(mylist)

run

[15468, 7621, 4312, 654, 53, 9, 8, 5, 5, 2, 56465]
```

> Copy items
Using method `copy()`:
```
mylist = ["mouse","keyboard","monitor"]
copy = mylist.copy()
print(copy)

run

['mouse', 'keyboard', 'monitor']
```

Using method `list()`:
```
mylist = ["mouse","keyboard","monitor"]
copy = list(mylist)
print(copy)

run

['mouse', 'keyboard', 'monitor']
```

> Join two lists

```
list1 = ["a", "b", "c"]
list2 = [1, 2, 3]

list3 = list1 + list2
print(list3)

run

['a', 'b', 'c', 1, 2, 3]
```
<br>

Tuples
========
<br>

> Implement a tuple with 3 elements
```
mytuple = ("amanox", "is", "good") #syntax requires standard brackets
print(mytuple)

run

('amanox', 'is', 'good')
```
<br>

> Add an element to `mytuple`:

The method `append()`does **not** work with tuples. Convert it into a list instead:
```
thistuple = ("origami", "nagasaki", "kyoto") #first you write your tuple
y = list(thistuple)                          #then you define your tuple as a list, you convert
y.append("hiroshima")                        #use method append() to add an item in your converted tuple
thistuple = tuple(y)                         #you define your converted tuple (your list) as the uptdated tuple(y)
print(thistuple)                             #you want to see the output

run

('origami', 'nagasaki', 'kyoto', 'hiroshima')
```
<br>

> Join two tuples

Use operator `+`:
```
tuple1 = ("x", "y", "z")
tuple2 = (3,6,9)

tuple3 = tuple1 + tuple2
print(tuple3)

run

('x', 'y', 'z', 3, 6, 9)
```

You also can multiply tuples:
```
brands = ("nike", "puma", "adidas")*2
print(brands)

run

('nike', 'puma', 'adidas', 'nike', 'puma', 'adidas')
```
<br>

> Why are tuples better than lists?

Tuples contain less memory than lists and therefore are faster.

<br>

> All existing methods for tuples

Method `count()` counts the amount a specified item appears in a tuple:
```
brands = ("nike", "puma", "adidas", "nike")
x = brands.count("nike")
print(x)

run

2
```

Method `index()` shows the position of the specified item as a number:
```
brands = ("nike", "puma", "adidas", "nike")
x = brands.index("puma")
print(x)

run

1
```
![tuple](tuple.jpg "<b>Tuple</b> (Photo by Jan Huber on Unsplash)")

<br>

Set
===

> Implement a set with 3 elements

```
myset = {"notebook", "desk", "office"} #syntax requires curly brackets
print(myset)

run

{'desk', 'notebook', 'office'}
```
<br>

> Duplicates are not allowed

Items or values that occur several times, are ignored:
```
myset = {"notebook", "desk", "office", "notebook"} #the word "notebook" appears twice
print(myset) #commands output

run

{'notebook', 'office', 'desk'} #as you can see, the duplicate was ignored
```
<br>

> Join two sets

The `union()` method returns a new set with all items from both sets:
```
set1 = {"x", "y", "z"}
set2 = {3,6,9}
set3 = set1.union(set2)
print(set3)

run

{'y', 'x', 'z', 3, 6, 9}
```
<br>

> Why are sets better than lists?

They are very useful to eliminate duplicates, since duplicate elements are not allowed. Therefore, sets are best for implementing mathematical operations such as unions and intersections.

<br>

> All existing methods for sets

Method `add()` adds an element to the set:
```
brands = {"nike", "puma", "adidas"} #the brackets indicate that it is a set
brands.add("yonex")
print(brands)

run

{'nike', 'adidas', 'yonex', 'puma'}
```

Method `clear()`removes the sets content between the brackets:
```
brands = {"nike", "puma", "adidas"}
brands.clear()
print(brands)

run

set() #output returns standard brackets
```

Method `copy()` returns your sets copy:
```
brands = {"nike", "puma", "adidas"}
x = brands.copy()
print(x)

run

{'puma', 'nike', 'adidas'}
```

Method `difference()` returns a set that contains items that only exists in set x, and not in set y:
```
x = {"apple", "banana", "cherry"}
y = {"google", "microsoft", "apple"}
z = x.difference(y)
print(z)

run

{'banana', 'cherry'}
```

Method `difference_update()` removes the unwanted items form the origianl set. The parameter value `set` is required:
```
x = {"nagasaki", "heroshima", "kyoto"}
y = {"tokyo", "osaka", "nagasaki"}
x.difference_update(y) #in this case, "x" is the required "set"
print(x)

run

{'kyoto', 'heroshima'}
```

Method `discard()` removes the specified item from the set. The value as a parameter is required:
```
fruits = {"mexico", "canada", "panama"}
fruits.discard("canada")
print(fruits)

run

{'mexico', 'panama'}
```

Method `intersection()` returns a set that contains the item that extists in both sets x and y. At least one value as a parameter is required. You can search for as many equal items you like:
```
x = {"mexico", "canada", "panama"}
y = {"germany", "namibia", "canada"}
z = x.intersection(y)
print(z)

run

{'canada'}
```

Method `interseciton_update()` removes the unwanted items from the original set:
```
x = {"mexico", "canada", "panama"}
y = {"germany", "namibia", "canada"}
z = {"cuba", "india", "canada"}
x.intersection_update(y, z)
print(x)

run

{'canada'}
```

Method `isdisjoint()` returns `True` if no items are present in the amount of compared sets, therwise `False`. The value as a parameter is required:
```
x = {"mexico", "canada", "panama"}
y = {"germany", "namibia", "canada"}
print(x.isdisjoint(y))

run

False
```

or

```
x = {"mexico", "canada", "panama"}
y = {"germany", "namibia", "honduras"}
print(x.isdisjoint(y))

run

True
```

Method `issubset()` returns `True` if all items in the set exit in the specified set, otherwise `False`. The value as a parameter is required:
```
x = {"a", "b", "c"}
y = {"f", "e", "d", "c", "b", "a"}
print(x.issubset(y))

run

True
```

or

```
x = {"a", "b", "c"}
y = {"f", "e", "d", "c", "b", "a"}
print(y.issubset(x))

run

False
```

Method `issuperset()` returns True if all items in the specified set exists in the oiginal set, otherwise `False`. The value as a parameter is required:
```
x = {"a", "b", "c"}
y = {"f", "e", "d", "c", "b", "a"}
print(x.issuperset(y))

run

False
```

or

```
x = {"a", "b", "c"}
y = {"f", "e", "d", "c", "b", "a"}
print(y.issuperset(x))

run

True
```

Method `pop()` removes a random item from the set:
```
brands = {"nike", "puma", "adidas"}
brands.pop()
print(brands)

run

{'puma', 'nike'}
```

Method `remove()` removes a specified item and therefore requires a value as a parameter:
```
brands = {"nike", "puma", "adidas"}
brands.remove("puma")
print(brands)

run

{'adidas', 'nike'}
```

Method `symmetric_difference()` returns a set that contains all items from both sets, but not the items that are present in both sets. The parameter `set` is required. `set.symmetric_difference(set)`:
```
x = {"nike", "puma", "adidas"}
y = {"puma", "cheetah","tiger"}
z = x.symmetric_difference(y)
print(z)

run

{'tiger', 'nike', 'cheetah', 'adidas'} #logically it removed the symmetric diffrence that would be "puma" in this case
```

Method `symmetric_difference_update()` updates the original set by removing identical items. This method also requires the parameter `set`:
```
x = {"nike", "puma", "adidas"}
y = {"puma", "cheetah","tiger"}
x.symmetric_difference_update(y)
print(x)

run

{'adidas', 'nike', 'tiger', 'cheetah'}
```

Method `union()` returns a set that contains all items from the original set influding items from the specifed set(s). The specification can be any iterable object. If an item is present in more than one set, the output will show only one appearance of this item:
```
x = {"a", "b", "c"}
y = {"f", "d", "a"}
z = {"c", "d", "e"}
result = x.union(y, z)
print(result)

run

{'d', 'f', 'c', 'b', 'e', 'a'}
```

Method `update()` updates the current set, by adding items from another set or any other iterable. `set`is required as a parameter:
```
x = {"nike", "puma", "adidas"}
y = {"puma", "cheetah","tiger"}
x.update(y)
print(x)

run

{'tiger', 'nike', 'adidas', 'puma', 'cheetah'}
```

<br>

Dictionary
==========

![Dictionary](dictionary.jpg "<b>Dictionary</b> (Photo by Pisit Heng on Unsplash)")

Dictionaries are written with curly brackets, have keys and values. Dictionaries are used to store date values in key. Dict items are structured, chagneable, and do not wllow duplicates. They are presented in key:value paris and are being referred to by using the key name.

<br>

> Empty list

```
people = {'list':[]}
print(people)

run

{'list': []}
```
```
people = {'list':[]}
list = people.pop('list')
print(list)

run

[]
```

<br>

> Editing the list

```
people = {'Name': 'Koch', 'First name':'Yonea', 'Age':21, 'list':[]}
print(people)

run

{'Name': 'Koch', 'First name': 'Yonea', 'Age': 21, 'list': []}
```

<br>

> Joining two dicts

```
people = {'Name': 'Koch', 'First name':'Yonea', 'Age':21, 'list':[]}
people['Class'] = ['Math', 'JavaF']
print(people)

run

{'Name': 'Koch', 'First name': 'Yonea', 'Age': 21, 'list': [], 'Class': ['Math', 'JavaF']}
```

<br>

> Why are dicts better than lists?

So, dictionary is faster because you used a better algorithm. The reason is because a dictionary is a lookup, while a list is an iteration. Dictionary uses a hash lookup, while your list requires walking through the list until it finds the result from beginning to the result each time.

<br>

> Dicts methods

Method `clear()` removes all the elements from the dictionary. There are no parameters required:
```
thisdict = {"name": "Laura", "brand": "nike", "year": 1997}
thisdict.clear()
print(thisdict)

run

{}
```

Method `copy()` returns a copy of the dictionary. There are no parameters required:
```
thisdict = {"name": "Laura", "brand": "nike", "year": 1997}
thisdict.copy()
print(thisdict)

run

{'name': 'Laura', 'brand': 'nike', 'year': 1997}
```

Method `fromkeys()` returns a dictionary with the specified keys and values. Parameters such as key and value are required:
```
x = ('key1', 'key2', 'key3')
y = 0
thisdict = dict.fromkeys(x,y)
print(thisdict)

run

{'key1': 0, 'key2': 0, 'key3': 0}
```

Method `get()` returns the value of the specified key. (To access an item.) Parameters such as keyname and value are required:
```
thisdict = {'name':'Yonea', 'food':'Arepa', 'movie':'Star Wars'}
print(thisdict.get('food'))

run

Arepa
```

Method `items()` returns a list containing a tuple for each key value pair. There are no parameters required:
```
thisdict = {'name':'Yonea', 'food':'Arepa', 'movie':'Star Wars'}
print(thisdict.items())

run

dict_items([('name', 'Yonea'), ('food', 'Arepa'), ('movie', 'Star Wars')])
```

Method `keys()` returns a list containing the dictionary's keys. There are no parameters required:
```
thisdict = {'name':'Yonea', 'food':'Arepa', 'movie':'Star Wars'}
print(thisdict.keys())

run

dict_keys(['name', 'food', 'movie'])
```

Method `pop()` removes the element with the specified key. Parameter keyname is required:
```
thisdict = {'name':'Yonea', 'food':'Arepa', 'movie':'Star Wars'}
thisdict.pop('food')
print(thisdict)

run

{'name': 'Yonea', 'movie': 'Star Wars'} #either shows your dict with the removed pop
```
```
thisdict = {'name':'Yonea', 'food':'Arepa', 'movie':'Star Wars'}
print(thisdict.pop('food'))

run

Arepa #or shwos the specified pop
```

Method `popitem()` removes the last inserted key-value pair. There are no parameters required:
```
thisdict = {'name':'Yonea', 'food':'Arepa', 'movie':'Star Wars'}
print(thisdict.popitem())

run

('movie', 'Star Wars')
```

Method `setdefault()` Returns the value of the specified key. If the key doesn't exist, insert the key, with the specified value. Parameter keyname is required:
```
#Get the value of the "color" item, if the "color" item does not exist, insert "color" with the value "white"
thisdict = {'name':'Yonea', 'food':'Arepa', 'movie':'Star Wars'}
x = thisdict.setdefault('color','White')
print(x)

run

White
```

Method `update()` updates the dictionary with the specified key-value pairs. An iterable as a parameter value is required:
```
thisdict = {'name':'Yonea', 'food':'Arepa', 'movie':'Star Wars'}
thisdict.update({'color':'Fuchsia'})
print(thisdict)

run

{'name': 'Yonea', 'food': 'Arepa', 'movie': 'Star Wars', 'color': 'Fuchsia'}
```

![Fuchsia](fuchsia.jpg "<b>Fuchsia</b> (Photo by Kseniya Lapteva on Unsplash)")

Method `values()` returns a list of all values in the dicitonary. There are no parameters required:
```
thisdict = {'name':'Yonea', 'food':'Arepa', 'movie':'Star Wars'}
x = thisdict.values()
thisdict['movie'] = 'Grease'
print(x)

run

dict_values(['Yonea', 'Arepa', 'Grease'])
```
<br>

File
=====







