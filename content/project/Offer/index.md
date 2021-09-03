---
title: Offers and GitHub
summary: Following Jim's module 
tags:
- PiBS
date: 27-06-2020

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by Roman Synkevych on Unsplash
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
**Module Part 1**

How to build an offer for a PC or a server
===========================================
If a client of yours submits an order, you submit an offer in return. This enables having an overview. The bigger or complexer an order is, the more sense it makes to even create an offer. (In IT it is often the case, that submiting an offer already is chargeable. This should be communicated clearly!)

> First you need to know what an offer usually contains. 
+ provider, date, location, validity, services/material, customer, reciver, contact person, invoice address, reference numbers, offer number

> You then create the offer based on the requirements given by your client. 
+ Oftentimes you'll see that your clients needs not always are clear. That's where you as a provider find suitable solutions. 

> Send the offer or maybe two offers to consult your client.
+ Sometimes it is an advantage to be prepared and offer different kind of solutions to maintain flexibility. 

<br>

**Module Part 2**

Working with GitHub
=====================
GitHub is a wonderful tool for creating projects. To be precise it's a software versioning tool or VCS (:= Version Control System). It also turns out to be an absolut necessity, when several programmers work on the same project. It was orginally made by Linus Torvalds, the founder of Linux. 

You can envision VCS like a graph:

![Graph 1](graph1.jpg "<b>Graph 1</b> (Module 1.5)")

Let's take the image above as an example. The green part is the master branch, whereas the blue and orange ones are additional branches, enabling programmers to work on their own copy of the project/code or change the content. Those changes include bugfixes, new features or updates. To realize the work, they merge the edited on to the master branch.

> The main rule is to never work on the master branch. Processes should always be done on a developing branch.

![Graph 2](graph2.jpg "<b>Graph 2</b> (Module 1.5)")

The repository is a remote location. To work on a project you need to clone the repo locally. You can use a programm like Visual Stuido Code, pull your branch, and edit your changes there. If you commit and push your changes will be transmitted to the remote location. 

It's meant to be a transparent tool. The project participants can see who did what, when and why. Team members can work on different tasks without conflicting others. Don't upload temporary date used only for testing purposes or stuff that your specific IDE (:= Integrated Development Environment) uses.

CHeckout the GitHub [GIT CHEAT SHEET](https://education.github.com/git-cheat-sheet-education.pdf) 

```Some git commands visualised by a DAG (:= Directed Acyclic Graph):```
![Graph 3](graph3.jpg "<b>Graph 3</b> (Module 1.5)")

`git commit -m "your commit message"`
`git merge <branch>`
`git rebase -i <base>`

A DAG never forms a cylce, therfore alwas goes in a direction and never to a previous node.




