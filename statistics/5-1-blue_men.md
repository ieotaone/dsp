[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

How many people are between 5'10" and 6'1"?

```
y=dist.cdf(177.8)
x=dist.cdf(185.4)
z=x-y
q=round(z*100,2)
print (x)
print (y)
print ("{} % are between 5'10 and 6'1".format(q))
```
0.8317337108107857  
0.48963902786483265  
34.21 % of the male population are between 5'10 and 6'1

```
male population in the US in 2018 is 151.8 million 
p=z* 151800000
print (p)
```
51929972.871195674