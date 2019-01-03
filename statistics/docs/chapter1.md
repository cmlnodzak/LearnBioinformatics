---
title: Introduction
layout: default
---

# I. *Introduction to the __R__ Programming Language*

[Home]({{ site.baseurl }}{% link index.md %}) <br/>
[Section Home]({{ site.baseurl }}{% link statistics/index.md %})


Let's begin by opening up an __R__ session. <br/>
The __">"__ symbol displays at the beginning of the line to prompt you for a command. <br/>
Type the command __"ls()"__, followed by enter. <br/>

R will then execute the command and print the result to the screen. <br/>
You will notice that __R__ displays the ">" symbol when the execution of the command is complete, and awaits further input. <br/>
Type __q()__ to exit __R__. <br/>


## To get help in __R__: <br/>
	If the function name is known (ex. "sum")
		> help(sum)
		> help(sd)
		> ?sum
		> ?sd()
	If the function name is not known
		> help.search("standard deviation")


## Variable Names and Assignments:
	-- Flexible, but cannot begin with a number.
	-- Cannot start with a period followed by a digit.
	-- Names are case-sensitive.
	-- Specific, system-names to avoid using:
		(e.g.) c, q, t, C, D, F, I, T, diff, etc.
	-- Symbolic variables can be assigned values.
		> xy <- 3	(Assign the numeric value 3 to variable "xy" )
		> xy	(Reference the assigned variable.)
		    [1] 3	(R returns the one-element long vector, everything in R is a vector!)
## R is an Object Oriented Programming Language:
	This means that everything in R is an object belonging to some class.
		> mode(): a classification of objects according to their basic structure.
			modes include numeric, character, logical, list, function.
		> class(): a property assigned to an object, which determines how any function operates with an object of a particular class.
## Vectors in R: <br/>
	-- The elementary datatypes in R are all vectors.
	-- The c() construct is used to create concatenated vector.
	-- Elements of a vector must have the same mode.
		> seq()
			A sequence function, used to generate equidistant series of numbers.
		> seq(start, end, step-size)
		> rep()
			A function to replicate, generate repeated values.
		> rep(1,3)	
			[1] 1 1 1	
		> rep(1:3,3)
			[1] 1 2 3 1 2 3 1 2 3
		> rep(8:10, 1:3)
			[1] 8 9 9 10 10 10

## Data Matrices in R: <br/>







