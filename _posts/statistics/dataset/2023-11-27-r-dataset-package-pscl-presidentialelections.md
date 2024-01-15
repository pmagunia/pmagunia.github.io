---
title: R Dataset / Package pscl / presidentialElections
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">presidentialElections</span> data set which pertains to elections for U.S. President, 1932-2012, by state. The <span class="mono">presidentialElections</span> data set is found in the <span class="mono">pscl</span> R package. You can load the <span class="mono">presidentialElections</span> data set in R by issuing the following command at the console <span class="mono">data("presidentialElections")</span>. This will load the data into a variable called <span class="mono">presidentialElections</span>. If R says the <span class="mono">presidentialElections</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("pscl")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-31287.csv">presidentialElections R data set</a></span>. The size of this file is about 29,408 bytes.</p><h2>elections for U.S. President, 1932-2012, by state</h2>
<h3>Description</h3>
<p>Democratic share of the presidential vote, 1932-2012, in each state and the District of Columbia.</p>
<h3>Usage</h3>
<pre>data(presidentialElections)</pre>
<h3>Format</h3>
<ul>
<li>
<p>statecharacter, name of state</p>
</li>
<li>
<p>demVotenumeric, percent of the vote for president won by the Democratic candidate</p>
</li>
<li>
<p>yearnumeric, integer</p>
</li>
<li>
<p>southlogical, <code>TRUE</code> if state is one of the 11 states of the former Confederacy</p>
</li>
</ul>
<h3>Note</h3>
<p>1,047 observations, unbalanced panel data in long format. Hawaii and Alaska contribute data from 1960 onwards the District of Columbia contributes data from 1964 onward; Alabama has missing data for 1948 and 1964.</p>
<h3>Source</h3>
<p>David Leip's Atlas of U.S. Presidential Elections <a href="http://uselectionsatlas.org">http://uselectionsatlas.org</a></p>
<h3>Examples</h3>
<pre>
data(presidentialElections)
lattice::xyplot(demVote ~ year | state,
 panel=panel.lines,
 ylab="Democratic Vote for President (percent)",
 xlab="Year",
 data=presidentialElections,
 scales=list(y=list(cex=.6),x=list(cex=.35)),
 strip=strip.custom(par.strip.text=list(cex=.6)))## Obama vs Kerry, except DC
y08 &lt;- presidentialElections$year==2008
y04 &lt;- presidentialElections$year==2004
tmpData &lt;- merge(y=presidentialElections[y08,],
 x=presidentialElections[y04,],
 by="state")
tmpData &lt;- tmpData[tmpData$state!="DC",]
xlim &lt;- range(tmpData$demVote.x,tmpData$demVote.y)
col &lt;- rep("black",dim(tmpData)[1])
col[tmpData$south.x] &lt;- "red"plot(demVote.y ~ demVote.x,
 xlab="Kerry Vote Share, 2004 (percent)",
 ylab="Obama Vote Share, 2008 (percent)",
 xlim=xlim,
 ylim=xlim,
 type="n",
 las=1,
 data=tmpData)
abline(0,1,lwd=2,col=gray(.65))
ols &lt;- lm(demVote.y ~ demVote.x,
data=tmpData)
abline(ols,lwd=2) text(tmpData$demVote.x,
 tmpData$demVote.y,
 tmpData$state,
 col=col,
 cex=.65)
legend(x="topleft",
 bty="n",
 lwd=c(2,2),
 col=c(gray(.65),"black"),
 legend=c("No Change from 2004","Regression"))
legend(x="bottomright",
 bty="n",
 text.col=c("red","black"),
 legend=c("South","Non-South"))</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-31287.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-31287.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-pscl-presidentialelections.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-31287.json';</script>