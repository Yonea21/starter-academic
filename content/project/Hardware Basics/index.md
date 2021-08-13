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

2. How many bits are in a Mebibyte? ​
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

> Creating a sequence in the Johnny simulator that takes 2 numbers from any 2 registers, multiplies them and writes the result to another register.

*Optional:*
> Creating a macro-command to multiply (like ADD)  
> Creating a sequence to calculate the KGV or GGT  
> Making a division or modulo sequence

<br>

Boolean algebra
=================

> Documentation about `transistors` and `logic gates`

