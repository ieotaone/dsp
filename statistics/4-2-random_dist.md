[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

Generate 1000 numbers from numpy.random.random and plot their PMF. What goes wrong?

```
t = np.random.random(1000)
pmf = thinkstats2.Pmf(t)
thinkplot.Pmf(pmf, linewidth=0.1)
thinkplot.Config(xlabel='Random variate', ylabel='PMF')
```
![image](https://github.com/ieotaone/dsp/blob/master/statistics/graph4.png)
```
cdf = thinkstats2.Cdf(x, label='random')
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='random', ylabel='CDF')
```
![image](https://github.com/ieotaone/dsp/blob/master/statistics/graph5.png)  

The distribution is not uniform 