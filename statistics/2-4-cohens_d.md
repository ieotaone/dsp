[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>>Exercise 2.4 Using the variable totalwgt_lb, investigate whether first ba- bies are lighter or heavier than others. Compute Cohen’s d to quantify the difference between the groups. How does it compare to the difference in pregnancy length?

```from __future__ import print_function, division  
%matplotlib inline  
import numpy as np  
import nsfg  
import first

CohenEffectSize(firsts.prglngth, others.prglngth)
```
0.028879044654449883  

```  
firsts.totalwgt_lb.mean(),others.totalwgt_lb.mean()
```
(7.201094430437772, 7.325855614973262)
```
CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)  
```
-0.088672927072602    
```
CohenEffectSize(firsts.prglngth, others.prglngth) - CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)  
```
0.1175519717270519   

The value of the difference in groups is almost 4 times the difference in pregnancy length  
