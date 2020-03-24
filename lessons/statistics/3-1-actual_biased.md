[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)


resp = nsfg.ReadFemResp()
pmf = thinkstats2.Pmf(resp.numkdhh, label = 'NUMKDHH')
thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='Number of children', ylabel='PMF')
                                   
biased = BiasPmf(pmf, label='biased')
thinkplot.pmf(biased)
thinkplot.Config(xlabel='Number of children', ylabel='PMF')
                                   
thinkplot.Pmfs([pmf, biased])
thinkplot.Config(xlabel='Number of children', ylabel='PMF')
                                   
print(pmf.Mean())
print(biased.Mean())

