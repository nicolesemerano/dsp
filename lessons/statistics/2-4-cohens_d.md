[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)
"""Using the variable totalwgt_lb, investigate whether first babies are lighter or heavier than others. Compute Cohen’s d to quantify the difference between the groups. How does it compare to the difference in pregnancy length?"""
>> REPLACE THIS TEXT WITH YOUR RESPONSE
'''python
import pandas as pd
import numpy as np
import math
def cohens(totalwgt_lb1, totalwgt_lb2):
    diff = totalwgt_lb1.mean() - totalwgt_lb2.mean()
    n1, n2 = len(totalwgt_lb1), len(totalwgt_lb2)
    stdev1 = totalwgt_lb1.std()
    stdev2 = totalwgt_lb2.std()
    num = math.sqrt((stdev1 ** 2) + (stdev2 ** 2))
    pooled = num / 2
    d = diff / pooled
    return d
'''