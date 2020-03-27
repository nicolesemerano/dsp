[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> '''python
import scipy.stats
mu = 178    #This is aproximately 5'10"
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
type(dist)
z1 = (185.4 - mu)/sigma
area1 = .5
area2 = dist.cdf(185.4)
diff = area2 - area1
ans = diff * 100
ans
'''

<!--Area1 is .5 because that is the mean/median, so half the data is to the left. -->

