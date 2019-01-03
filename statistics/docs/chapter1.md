# I. *Introduction to the R Programming Language*

Let's begin by opening up an R session. <br/>
The ">" symbol displays at the beginning of the line to prompt you for a command. <br/>
Type the command "ls()", followed by enter. <br/>

R will then execute the command and print the result to the screen. <br/>
You will notice that R displays the ">" symbol when the execution of the command is complete, and awaits further input. <br/>
Type q() to exit R. <br/>


## To get help in R: <br/>
	#### If the function name is known (ex. "sum") <br/>
		> help(sum) <br/>
		> help(sd) <br/>
		> ?sum <br/>
		> ?sd() <br/>
	#### If the function name is not known <br/>
		> help.search("standard deviation") <br/>


## Variable Names and Assignments: <br/>
	--- Flexible, but cannot begin with a number. <br/>
	--- Cannot start with a period followed by a digit. <br/>
	--- Names are case-sensitive. <br/>
	--- Specific, system-names to avoid using: <br/>
		(e.g.) c, q, t, C, D, F, I, T, diff, etc. <br/>
	--- Symbolic variables can be assigned values.
		> xy <- 3	(Assign the numeric value 3 to variable "xy" ) <br/>
		> xy	(Reference the assigned variable.) <br/>
		    [1] 3	(R returns the one-element long vector, everything in R is a vector!) <br/>

## R is an Object Oriented Programming Language: <br/>
	This means that everything in R is an object belonging to some class.<br/>
		> mode(): a classification of objects according to their basic structure. <br/>
		modes include numeric, character, logical, list, function. <br/>
		> class(): a property assigned to an object, which determines how any function operates with an object of a particular class. <br/>

## Vectors in R: <br/>
	--- The elementary datatypes in R are all vectors. <br/>
	--- The c() construct is used to create concatenated vectors. <br/>
	--- Elements of a vector must have the same mode. <br/>
	> seq() <br/>
		A sequence function, used to generate equidistant series of numbers. <br/>
	> seq(start, end, step-size)<br/><br/>
	> rep() <br/>
		A function to replicate, generate repeated values. <br/>
	> rep(1,3) <br/>	
		[1] 1 1 1 <br/>	
	> rep(1:3,3) <br/>
		[1] 1 2 3 1 2 3 1 2 3 <br/>
	> rep(8:10, 1:3) <br/>
		[1] 8 9 9 10 10 10 <br/>

## Data Matrices in R: <br/>







