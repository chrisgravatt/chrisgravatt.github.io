---
layout: post
title: "Building a Stochastic Simulation in Three Lines of Code"
date: 2016-04-03
permalink: /:title
categories: [jekyll]
tags: [jekyll]
---

Today, you are going to be awesome. You are going to program a stochastic simulation from scratch using a programming language called Python. This is intended for the total noob, someone who has little to no experience with programming languages, or even computers in general. If you have programming experience, leave now while you still can. 

Let's break down the intimidating term "stochastic simulation". Stochastic basically means random. It refers to a computer program that outputs something different every time. The opposite of a stochastic program is a deterministic one. A deterministic program outputs the same thing every time. `print 1 + 1` will always output 2. 

A simulation is anything that exists in the real world, that is modeled or replicated in the computer. For example, a die is something in the real world that lands on a random number every time you roll it. Today you are going to create a die in the computer, a stochastic simulation!

Most beginner tutorials will recommend which Python implementations to download, but that is tedious and boring. If you don't already have Python, don't worry about it. Go to [Skulpt](http://www.skulpt.org). It's an in-browser implementation of Python! Genius. 

Now, to write code! First erase everything that is already in the box under "Demo". Then type:

	import random

	die = [1, 2, 3, 4, 5, 6]

	print random.choice(die)

Then hit "run"

In the output box, it will show a number. Hit "run" as much as you want, you'll see that it's a random number every time. 

So easy! 

Let me explain exactly what the code does so you know what's going on. 

	import random

`import` is a statement that tells Python to bring something into our program that somebody else made. Python has a ton of packages, code that other people have written that you can use. You won't see this code directly when you import it, but you can use it. 

`random` is one of those packages. It contains a lot of useful code for doing things randomly. More on this in a bit.

	die = [1, 2, 3, 4, 5, 6]

`die` is a variable. A variable is a name you give something that stores a value. That value can be a number, a list, words, and many other things. You can name variables anything you want. 

`die =` the equals sign is an assignment statement. It tells Python to assign whatever comes after the equals sign to the variable. 

`die = [1, 2, 3, 4, 5, 6]` is the full assignment statement. The thing that is assigned to the variable is called a list. A list is a special format in Python. It is always enclosed in brackets, and the items in the list are always separated by commas. Here, it is a list of numbers 1 through 6, the faces of our die. 

	print random.choice(die)

`print` is another statement in Python. Whatever comes after it is displayed in the output. Easy. You can still run this program without the `print` statement, the computer will still execute the program, but you won't see anything. 

Now here's the fun part. You imported the Python package `random` for a reason. You are going to use something from that package called `choice`, a mini-program inside the `random` package that will randomly choose one item from a list. In order to use this mini-program, known as a function, first type `random.choice`. The package name and the function are separated by a period. Because that's just what you do. 

Now, `choice` is a function, which can be thought of as a magical black box of wonder, where you input something, something magical happens inside of the black box, and it spits out something new. Here, the function `choice` takes in a list. You already have a list, and you gave it a name `die`. In order to set `die` as the input, you have to put it in parenthesis directly after the function name `random.choice(die)`. The `choice` function takes in the list of six numbers and spits out a random one. So awesome. 	

Because you specified to print it, you see the number in the output when you hit run. 

And that's it! You just implemented a stochastic simulation from scratch! 