[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

**Exercise 4-2:

Here's the code and plots for the PMF and CDF of a range of random numbers generated from 1-1000:

**PMF

```{python}
t = np.random.random(1000)
pmf = thinkstats2.Pmf(t, label='Random #s1-1000')
thinkplot.Pmf(pmf, linewidth=0.1)
thinkplot.Config(xlabel='Random variate', ylabel='PMF')
```

![](https://github.com/missionfromdog/dsp/blob/master/statistics/4-2pmf.png):

**CDF

```{python}
cdf = thinkstats2.Cdf(t, label='Random #s')
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='random#s', ylabel='CDF')
```

![](https://github.com/missionfromdog/dsp/blob/master/statistics/4-2cdf.png):
