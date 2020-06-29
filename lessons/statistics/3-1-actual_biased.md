[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

*Had to check the solutions and work backwards with this one*


**Here is the required label for the biased graph**


pmf = thinkstats2.Pmf(resp.numkdhh, label='numkdhh')

**Plotted**

inkplot.Pmf(pmf)
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

**The bias fix**

biased = BiasPmf(pmf, label='biased')


thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased])
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

pmf.Mean() = 1.024205155043831

biased.Mean() = 2.403679100664282
