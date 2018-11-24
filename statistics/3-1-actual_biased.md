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

/Users/ginachung/Desktop/Screen Shot 2018-11-24 at 5.40.41 PM.png


```thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='Count of children under 18', ylabel='Pmf')```


