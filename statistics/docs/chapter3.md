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

__Cumulative Distribution Function__
: let X be a discrete random variable, then the CDF for X is given by F.

$$ F(x) = P( X \neq x ) $$


## Expectation and Distribution Parameters
The mean ($$\mu$$) is the expected value and the variance describes the distribution from the mean.

$$ variance = \sigma^2 = \sum((x - \mu)^2 * P(x)) $$ 


## Bernoulli Random Variables
A single (one trial) experiment with only two possible outcomes.<br/>
success = 1 , failure = 0 <br/>

* p = p(success)
* (1-p) = p(failure)

(e.g) The number of membrane bound proteins form a randomly selected set of 50 protein structures.


## Binomial Random Values
1. Only two possible outcomes per trail.<br/>
success = 1 , failure = 0 <br/>

2. Each trial is independent. <br/>
The result of one trial will no impact the next trial.

3. The probabiltiy of success is fixed, it is the same for all trials.

4. The number of trials n, is fixed in advanced and each trial is identical.

The Binomial random variable X is the sum of identically distributed, independent bernoulli random variable.

$$ PMF = P(X=x) = {n \choose k}p^k (1-p)^{n-k} $$





