[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```
from __future__ import print_function, division

%matplotlib inline

import numpy as np

import nsfg
import first
import thinkstats2
import thinkplot 

ct= nsfg.ReadFemResp()
pmf = thinkstats2.Pmf(ct.numkdhh, label='numkdhh')

hist = thinkstats2.Hist(ct.numkdhh, label='numkdhh')
thinkplot.Hist(hist)
thinkplot.Config(xlabel='Count of children under 18', ylabel='Count')
```
![image](https://github.com/ieotaone/dsp/blob/master/statistics/graph.png)

```thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='Count of children under 18', ylabel='Pmf')
```

![image](https://github.com/ieotaone/dsp/blob/master/statistics/graph2.png)

```
biased_pmf = BiasPmf(pmf, label='bias')
thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_pmf])
thinkplot.Config(xlabel='Count of children under 18', ylabel='PMF')
```

![image](https://github.com/ieotaone/dsp/blob/master/statistics/graph3.jpg)

```
print('Actual mean', pmf.Mean())
print('Biased mean', biased_pmf.Mean())
```
Actual mean 1.024205155043831  
Observed mean 2.403679100664282

