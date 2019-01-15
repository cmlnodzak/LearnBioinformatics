---
title: Statistics - Chapter 3
layout: default
---

# III. Random Variables and Probability Distributions

[Home]({{ site.baseurl }}{% link index.md %}) <br/>
[Section Home]({{ site.baseurl }}{% link statistics/index.md %})


Probabilities are based on observations of random outcomes of an experiment. <br/>
Outcomes can be numerical or categorical. (RNAseq counts, amino acids, secondary structure type, etc.) <br/> 
For non-numerical outcomes we are generally may be more interested in a numerical aspect of the outcome, <br/> 
rather than the outcome itself. <br/>
Random Variables are used to assign a nuerical value to each experimental outcome.</br>
They are some function that associates a real number with an element in the sample space.

## Discrete Random Variables

The number of possible values is finite. <br/>
Typically, the values of all outcomes are positive integers. <br/>
The behavior of random variables can be described in terms of probabilities (PDF and CDF) <br/>

__Probability Density Function__
: The PDF/PMF is a list of all possible values of a random variable and their probabilities.

$$ P(X) = (X = x) $$

Two essential properties of a probability distribution for a discrete random variable.

1. $$ P(X = x ) \geq 0 $$
2. $$ \sum(P(X = x)) = 1 $$	, for all x.


