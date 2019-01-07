---
title: Descriptive Statistics and General Probability
layout: default
---

# II. Descriptive Statistics and General Probability

[Home]({{ site.baseurl }}{% link index.md %}) <br/>
[Section Home]({{ site.baseurl }}{% link statistics/index.md %})

## Statistical Methods
__Descriptive__: describe key features of a data set
	
__Inferential__
: draw conclusions about the population based on sample data.

	Where a population refers to an ideal or theoretical group
	that would be too costly to adequately measure.
	
__Statistic__
: a descriptive measure computed from the data of a sample.

__Parameter__
: a descriptive measure computed form the data of a population.

|Measurement | Population Parameter | Sample Statistic |
| :---: | :---: | :---: |
|mean | $$\mu$$ | $$\bar{x}$$ |
|proportion | p | $$\hat{p}$$ |
|variance | $$\sigma^{2}$$ | $$s^2$$ |
|correlation coefficient | $$\rho$$ | r |
{: rules="groups"}

## Sampling Methods and Techniques
__Random Sample__
: a sample of *n* measurements selected from <br/>
a population is random if every different sample of size <br/>
*n* has an equal probability of being selected.

__Simple Random Sampling__
: each individual within a sample is chosen at <br/>
random and each member of the population has an equal probability <br/>
of being included in the sample.

__Systematic Sampling__
: selection of elements from an ordered sampling frame. <br/>
The selection starts by taking an element at random followed by <br/> 
every $k^{th}$ element, where:<br/>
$$ K = (\frac{N}{n})$$

__Stratified Sampling__
: There may often be factors that divide of partition the <br/> 
population into subpopulations (i.e. groups/strata), and we may reasonably <br/>
expect the measurement of interest to vary among them. The strata must therefore <br/>
be disjoint in order to reduce sampling variability.

## [Measurents of Central Tendency]
	
__mean__
: the average of *n* values of data. <br/>
$$\bar{x} = \frac{1}{n}\left (\sum_{i=1}^n{x_i}\right ) = \frac{x_1+x_2+\cdots +x_n}{n}$$

__median__
: the central value of an ordered dataset, more robust than the mean to outliers.

__mode__
: the most frequent data entry in a set. Can have no more, unimodal or bimodal.

## Measures of Spread / Variation

__MAD__
: median absolute deviation
$$ MAD = median_i( | X_i - median_j(x_j) | ) $$

__SSE__
: sum of squared errors
$$ \sum_{i=1}^n{x_i}(x_i - \bar{x}^2)$$

__Standard deviation__
: $$ s = \sqrt{\frac{\sum_{i=1}^N (x_i - \bar{x})^2}{N-1} } $$

__Variance__ 
: $$ s^2 $$

__Coefficient of Variation__
: $$ CV = \frac{s}{\bar{x}}*100% $$

__Range__
: Gives the minimum value and maximum value for a dataset to show the boundaries.

__IQR__
: Interquartile Range, the third quartile minus the first quartile 
$$ IQR = (Q_3 - Q_1) $$.

__Outliers__
: any datapoint that lies more that ( 1.5 * IQR ) lower or higher than the first or third quartiles

## Basic Probability Concepts

Probability of event A, __P(A)__, describes the uncertainty that event A occurs, and is given by values that range from 0 to 1, inclusive.

$$ P(A) = \frac{n_a}{n_s} = \frac{\# of ways event A can occur}{\# of ways an experiment may proceed} $$

Relative frequency concept of probability

$$ P(A) = \lim_{x \to \infty} \frac{n_a}{n} \approx \frac{n_a}{n} = \frac{\# of times event A occured}{\# of times an experiment was run}} $$

*Alternatively, subjective probabilities are based on personal opinion*




