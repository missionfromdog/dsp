

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

![](https://user-images.githubusercontent.com/44006857/50600245-23bc8d00-0e76-11e9-90c7-a79b900ad82c.png)

Here's the python code to plot their means:

```{python3}
pmf.Mean()
```

output: 1.0242051

```{python3}
biased.Mean()
```

output: 6.9096085

