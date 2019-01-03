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

## R is an Object Oriented Programming Language: <br/>
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
Construction of a matrix is by column as the default.
	
	> matrixA <- matrix(1:6,nrow=2,ncol=3)
	> matrixA
		   [1] [2] [3]
		[1] 1   3   5
		[2] 2   4   6	
	> rownames(matrixA) <- c("this", "that")
	> colnames(matrixA) <- c("here", "there", "where")
        > matrixA
                   here there where
                this 1   3   5
                that 2   4   6

Functions to combine vectors into matrices.
	
	> plant_seed <- rbind(c(30,20,50),c(10,20,30))
	> dimnames(plant_seed) <- list(c("Round","Wrinkled"),c("Y","G","R"))
	> plant_seed
			 Y    G    R
                Round    30   20   50
                Wrinkled 10   20   30
	> t(plant_seed)
		   Round Wrinkled		
		Y 30 20
		G 20 20
		R 50 30

## DataFrames: <br/>
The most common data storage format.
Each column is stored as a variable, which have names.

	> aa <- c( 7, 10, 12, 34)
	> bb <- c( 4, 9, 15, 29)
	> cc <- data.frame(sampleI = aa, sampleII = bb)
	> cc
		sampleI sampleII
	1	7	4
	2	10	9
	3	12	15
	4	34	29


To access the variables within a DataFrame...

	Use the __$__ notation.

		> cc$sampleI
			[1] 7 10 12 34

	Make the variable directly callable with __attach()__.

		> attach(cc)
		> sampleII
			[1] 4 9 15 29

	Remove the DataFrame with __detach()__. 

	Additional data may be appened to an existing DataFrame with rbind() and/or cbind().
