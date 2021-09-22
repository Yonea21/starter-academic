---
title: Emma
summary: Following Yonea's instructions 
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
Trying out formatting with Markdown
======
#### Heading 4
## Heading 2
Hallo := normal  
**Hallo** := fettgedruckt  
*Hallo* := kursiv  

Hallo := normal <br>
**Hallo** := fettgedruckt <br>
*Hallo* := kursiv <br>

Hallo := normal

<br>

**Hallo** := fettgedruckt

<br>

*Hallo* := kursiv

<br>

Form
=====
<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="utf-8">
  <meta name="description" content="Übung aus PVA1">
  <meta name="keywords" content="FFHS, BestTeacher">
  <title>Übung Forms - PVA1</title>
</head>
<body>
<form action=”yonea.koch@amanox.ch”>
  <label>
    Vorname <br>
    <input id="fname" placeholder="Vorname" pattern="[a-zA-zäöüÄÖÜ]{2,}" required/><br>
  </label> <br>
  <label>
    Nachname <br>
    <input id="lname" placeholder="Nachname" pattern="[a-zA-zäöüÄÖÜ]{2,}" required/><br>
  </label> <br>
  <label>  
    E-Mail <br>
    <input type="email" id="mail" placeholder="E-Mail-Adresse" pattern="\{@}" required/> <br>
  </label> <br>
  <label>
    Buchungsdatum <br>
    <input type="date" id="orderdate" required/><br>
  </label> <br>
  <label>
    Telefonnummer <br>
    <input type="tel" id="tel" placeholder="Telefonnummer"/><br>
  </label> <br>
  <label>
    Postleitzahl <br>
    <input id="plz" placeholder="Postleitzahl" pattern="\d{4}" required/><br>
  </label> <br>
  <input type="submit" id="submit" pattern="yonea.koch@amanox.ch"/>
</form>
</body>
</html>

Mock up
===
I created my first Mock up. Here is an example of my feedback page.
![Mock up](mockup.jpg "<b>Mock up</b> (Screenshot)")
