[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

**Exercise 5-1:

To determine the percentage of US population that is in the range between 5'10'' and 6'1'' tall, I set two variables representing the short and tall heights, short and tall.  I used the dist.cdf function to calculate both of them, and then Jupyter code snippet in python:

**PMF

```{python}
import scipy.stats
mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
type(dist)
dist.mean(), dist.std()
dist.cdf(mu-sigma)

short = dist.cdf(177.8)
tall = dist.cdf(185.4)
short, tall, tall-short
```

  *For the short end, the 177.8cm (5'10'') Blue man, **48.963** percent of the male population falls into this group.

  *For the tall end, 185.4cm (or 6'1''), **83.17** percent of the male population falls into this group.

  *To determine the percentage in between, I took the taller dist.cdf and subtracted the smaller dist.cdf. The total population that falls between the two heights is **34.209** percent of the male population that could try out to be Blue Men.
