---
title: Hardware Basics
summary: Following Jim's module 
tags:
- PiBS
date: 27-06-2020

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by Lorenzo Herrera on Unsplash
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

> To build your own computer, you need to be aware of following components and their functions.

**Computer housing:**  
   protects all the connected components – maybe even in a stylish way  

**Motherboard:**  
   Also known as Mainboard, is the main component that connects every other component with eachother  

**CPU (central processing unit):**  
   Similar to the human brain, it calculates every command made on a PC  

**RAM (random access memory):**  
   Mostly 8 or 16 GB enables the CPU to work faster whilst using it as a temporary storage  

**Hard Disk:**  
   SSD = solid state drive  
   HDD = hard disk drive  
   SSD and HHD both enable physical, long term storage  

**PSU (power supply unit):**  
   This component fuels the PC with electricity  

**GPU (graphics processing unit):**  
   Enables 2D and 3D graphic programs to work as flawless as possible  

**Cooling:**  
   internal or external air cooling for avoiding overheated hardware  

<br>

> Advanced questions: (My device is a Surface Book 2)

 1.	How fast (in GHz) is the CPU you are using right now?  
   i5-7300U 2.60 GHz

 2.   What chipset is on the motherboard? Could there be more options?  
   Windows 10 Pro Creators Update 64 Bit  
   For this product there's just 64 Bit available 

 3.	How many gigabytes of RAM are in the PC you’re using?  
   8.00 GB  Ram

 4.	What is/are the storage medium/media in your PC?  
   PCIe (:= Peripheral Component Interconnect Express)  
   Solid-State-Laufwerk (SSD) 256 GB, local hard disk C:

 5.	Where is the PSU in your PC? What about a laptop?  
   PC trhough motherboard  
   Laptop externally

 6.	Do you have a GPU?  
   HD-Grafik 620-GPU

 7.   How does the cooling work in your device? What about a smartphone?  
   My device: (Air) highly developed air conduction system inside; cooling is provided by a fan similar in design to an aircraft turbine  
   Smartphone: (Heatpipe) small pipe that transmits heat to the outside

<br>

Hypothetical machine
=====================

![Hypothetical machine](hypotet.jpg "<b>Hypothetical machine</b> (Unsplash: Christian Wiediger)")

Here's a list of parts i would choose to build my own pc:
[What do you think?](https://www.digitec.ch/de/shopList/show/3D5728899D9C9AB362CA0C9DD0376E73)

You may ask yourself why i chose those parts. Let me explain.
A way to choose computer parts in an online shop or anything actually, is to use filters and selections. For example I sort the Items based on ratings and reviews of buyers. Then I compare popularity, price and functionality. Is it a good investment? You want to make sure that it is. The most important thing to consider is if the parts are compatible. If you choose a product, mostly the site recommends compatible ones. If not, check the interfaces for compatibility.

There's also an intresting [Website](https://www.logicalincrements.com/), which helps you compare components.

<br>

CPU - in - depth
=================

**Wich one of the shown CPUs will perform best?**

| CPU 1         | CPU 2         | CPU 3 |
| ------------- |:-------------:| -----:|
| i9            | AMD           | i5    |
| 64-Bit        | 64-Bit        | 64-Bit |
| 3.50-5.30 GHz | 3.40-4.90 GHz | 2.7-4.6 GHz |
| 8 Cores       | 16 Cores      | 6 Cores   |
| 16 MB Cache   | 64 MB Cache   | 12 MB Cache  |

> I would say CPU 1 will perform best because it has the best base clock and boost clock speed. Although CPU 2 is a good competator as it improves in high core and cache.

A chip is made of a very simple raw material. Sand. 

<br>

Bits and bytes
===============

1. Say you have a gigabit internet connection (downstream). How many kilobytes can you download per second?​  
`1'000'000 KB`  
​

2. How many bits are in a Mebibyte?  
`1'048'576 / 8 = 131'072`  
​

3. You buy an HDD advertised with 1TB. How much usable space will the Windows operating system report you and why?  
`953 GB`  
`1024 GB would be usable in theory. 1 TB on "Base 10"  equals 1'099'511'627'776 (=:2^40) bits on "Base 2". The PC shows usable space in gigabyte. So we make the calculation {(2^40)TiB / (2^30)GiB = 1024 GB} 1024 := 1 kibibyte`  

<br>

Binary number system
=====================

> Decoding the following binary sequences to text. 

`01000001011011010110000101101110011011110111100000100000010101000110010101100001`

>  Each character uses 8-bits. Let's divide for more perspective. [Using ASCII table](https://www.rapidtables.com/code/text/ascii-table.html)

`01000001 01101101 01100001 01101110 01101111 01111000 00100000 01010100 01100101 01100001`

> A  m  a  n  o  x   `space (=: 001000000)`   T  e  a

<br>

##### Let's write my name in a binary sequence!

`0101100101101111011011100110010101100001`

`:= Yonea`

<br>

Johnny Simulator
================

[Youtoube tutorial](https://www.youtube.com/watch?v=CcZbqOHWyQY)

**Legend**
```
Asm   := Assembly
Type of language - Replace micro commands with macro commands  

Opnd  := Operand
Tells Johnny on what adress he should operate
``` 
<br>

> + Creating a sequence in the Johnny simulator that takes 2 numbers from any 2 registers, multiplies them and writes the result to another register.

+ Open RAM (on Macro Code)
+ Use the file *"multiplikation.ram"* (comes with the installation)
+ Make sure there are no errors
+ Click through *"one makro step"* until the numbers 4 and 6 multiplied and the accumulator shows the result 24.

> While continuously clicking the "play" button, it saves the numbers until you reached your result

**The Ram on your Johnny Simulator should look like this:**

> Make sure it's in the right order
![RAM on Johnny Simulator](Jonny.jpg "<b>RAM on Johnny Simulator</b> (Screenshot)")
> scroll down
![RAM on Johnny Simulator](Jonny2.jpg "<b>RAM on Johnny Simulator</b> (Screenshot)")

<br>

*Optional:*
> + Creating a macro-command to multiply (like ADD) 

+ Activate the *"Ctrl"* in the navigation bar
+ dfsadf

> + Creating a sequence to calculate the KGV or GGT  

+ dfsadf

> + Making a division or modulo sequence

+ dfsadf

<br>

Boolean algebra
=================
**How Logic Gates Work in Digital Electronics**  
To control the flow in a computer we use a gate and achieve an end goal. This flow is an electric current operating on a circuit. In the digital language we name these gates transistors. A transistor is either on or off. 
```
on  := electric current flows
off := electric current does not flow
```
Chaining transistors together leads to a `logic gate`, which enables adding, subtracting, multiplying and dividing by binary numbers `(1s & 0s)`.
> **Input:**    Voltage  
> **Output:**   decides wether it switches on or stays switched off

Some decades ago, a collection of transistors was put together and led to:
```
Integrated circuit := IC
```
Nowdays we speak about very large scale integrated ICs `(:=VLSI)`. Those contain up to billions of transistors into one tiny package.

![Microchip](microchip.jpg "<b>Microchip</b> (Unsplash: Laura Ockel)")

> Logic Gates:
```
AND; OR; NOT; XOR; NAND; NOR
```
Each logic gate has its specific way of coping. Disregarding therof, the in- and outputs will break everything down to two binary numbers. 

**AND:**
requiers two inputs for there to be an output  

**OR:**
requiers one input for there to be an output  

**NOT:**
requiers one input; always produces an opposite output  

**XOR:**
requiers one diffrent input; either/or situation  

**XNOR:**
requiers two same inputs; opposite of `XOR`  

**NAND:**
opposite output of `AND`; `NOT` logic applied to `AND`  

**NOR:**
opposite output of `OR`; `NOT` logic applied to `OR`  


> + Documentation about `transistors` and `logic gates`

<br>

Manipulating program CookieClicker with CheatEngine
===================================================

+ Download Cheatengine
+ Finish tutorial until step 6
+ Download Cookie Clicker from MS store
+ Open CookieClicer.exe on processes from cheatengine
+ Do as in the tutorial to find your value
+ And then just manipulate the value on cheatengine by overwriting it
+ enjoy the ridiculous score on your cookie

![Cookies](cookie.jpg "<b>Cookies</b> (Unsplash: The Creative Exchange)")

<br>

More on HDDs and SSDs
=========================
There are different types of HDDs like `consumer-grade`, `enterprise-grade`, `NAS-grade` and `server-grade`.  

> What are the differences between those grades?
+ Consumer-grade HDDs are more affordable and therefor easy-consumer-friendly.  
+ If a company risks coming to a stop if the server or dataase goes down, due to a drive failure, an enterpise-grade is considerable.  
+ A NAS-grade HDD is compareable to a private Cloud in an office. It's connected to a network, cheaper and enables comprehensive control.  
+ Server-grade HDDs have higher standards and requirements compared to regulare home usage HDDs.  

> Are there grades/tiers for SSDs?  
+ Yes there are so called tiers which stagger the SDDs in kategories as price and performance.  

> My whishlist  
+ [For building my own PC i would use these](https://www.digitec.ch/de/shopList/show/7D11285C0C277E21F637857D8BE90DEF)

<br>

GPU in depth
=============
+ Latest GPU from NVIDIA has 10'496 cores and 24 GB of GDDR6X memory.  
+ Two major GPU manufacturers: AMD & NVIDIA  
+ ASIC := Application-specific integrated circuit := Processor designed to do one thing; ASIC is high in efficency but low when it comes to being flexible.
+ CPU := Central Processing Unit on the other hand, ist low in efficency but high in flexibility.
+ GPU := Graphics Processing Unit multiplicates huge amounts of matrix (3D) in parallel.

<br>

Desired interfaces
==================
> What are my desired interfaces in a consumer PC or laptop?
+ [Please check my whishlist](https://www.digitec.ch/de/shopList/show/FB59BE98A43084CCBFD002196628C81D)
+ Ethernet for fast internet connection
+ Several USB C - USB A for connecting peripheral devices
+ Several Micro USB - USB A for connecting peripheral devices
+ HDMI for video and sound

> What would I change for in a server?
+ 
+ 
+ 
+ 

<br>

**Table**

| Name         | Use Case         | Release | Bandwidth | Wires | Clock | Signaltype | Distance | Power |
| ------------- |:-------------:| ----------:|---------:|-------:|-----:|------------:|--------:|-------:|
| RCA       | Video, Audio       | 1940      | 10 MHz   | 1     | 768 kHz  |   Analog   | 3m           |  x         |
| VGA     | Video Trans.        | 1987 | 3 MBit/s  |  14   |  60 MHz    | Digital          |  4m       |  x         |
| DVI       | Video Trans.      | 1999 | 7.44 GBit/s  |  29   |  165 MHz    |     Digital     |  4.5m  |     x      |
| PS/2        | Periphery       | 1990 |   350 MHz     |   4 |   16 kHz   |     Digital      |   5m    |     x      | 
| RJ45       | Network          | 1970  |   10 GBit/s   |   8 |   160 MHz   |   Digital    |    3m     |   x        |
| USB-1.0      | Power, Data Trans.  | 1996  |   1.5 MBit/s  | 4 |   1 kHz   |   Digital   |    5m     |   2.5 Watt |
| USB-2.0       | Power, Data Trans.  | 2000  |   480 MBit/s |  4 |   24 kHz   |   Digital    |    5m  |   x        |
| USB-3.0      | Power, Data Trans.  | 2008 |   5 GBit/s |     4 |   33 kHz   |   Digital  |    5m     |   x        |
| USB-C       | Power, Video, Audio, Network | 2015 |   40 GBit/s | 4 |   240 Hz  | Digital |    2m    |   x        |
| DP       | Video, Audio   |    2006  |   77 GBit/s |     20 |   225 MHz   |   Digital   |    1.8m    |   x        | 
| HDMI       | Video und Audio|    2002  |   43 Gbit/s   |   19 |   150 MHz   |   Digital  |    25m    |   x        |

<br>

Periphery
==========
Those are the discontinued displays:  
+ `CRT := Cathode ray tubes`  
+ `Plasma`  

Those are the most common Displays:  
+ `LCD := Liquid Crystal Display`  
+ `OLED := Organic Light Emitting Diode` 

> How much bandwidth is needed to stream a typical 2 hour Netflix 1080p movie (~6 GB)?
+ 48 Gbit/s

> What bandwidth (upload/download) do I have at home and on my mobile phone?
+ 

<br>

Setting up VR headset
======================

<br>

Sound
======
> What interfaces are used to play surround sound?

> What are common codecs?
