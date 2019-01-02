

**Exercise 3-1:

Here's a plot of the biased distribution:

```{python}
resp = nsfg.ReadFemResp()
pmf = thinkstats2.Pmf(resp.numkdhh, label='numkdhh')
biased_pmf = BiasPmf(pmf, label='observed')
thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_pmf])
thinkplot.Config(xlabel='Class size', ylabel='PMF')
```

![3-1chart](/Users/caseyhess/Dropbox/ThinkStats2/ThinkStats2/code/3-1chart.png)

Here's the python code to plot their means:

```{python3}
pmf.Mean()
```

output: 1.0242051

```{python3}
biased.Mean()
```

output: 6.9096085

