[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>>'''python
import numpy as np
import thinkstats2
import thinkplot
values = np.random.random(1000)
pmf = thinkstats2.Pmf(values)
thinkplot.Pmf(pmf, linewidth=0.2)
thinkplot.Config(xlabel = 'Random variable', ylabel = 'PMF')
cdf = thinkstats2.Cdf(values)
thinkplot.Cdf(cdf, linewidth = 2)
thinkplot.Config(xlabel = 'Random Variable', ylabel = 'CDF')
'''
