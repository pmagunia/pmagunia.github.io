---
title: R Dataset / Package HistData / Wheat.monarchs
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">Wheat.monarchs</span> data set which pertains to Playfair's Data on Wages and the Price of Wheat. The <span class="mono">Wheat.monarchs</span> data set is found in the <span class="mono">HistData</span> R package. You can load the <span class="mono">Wheat.monarchs</span> data set in R by issuing the following command at the console <span class="mono">data("Wheat.monarchs")</span>. This will load the data into a variable called <span class="mono">Wheat.monarchs</span>. If R says the <span class="mono">Wheat.monarchs</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("HistData")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-77745.csv">Wheat.monarchs R data set</a></span>. The size of this file is about 310 bytes.</p><h2>Playfair's Data on Wages and the Price of Wheat</h2>
<h3>Description</h3>
<p>Playfair (1821) used a graph, showing parallel time-series of the price of wheat and the typical weekly wage for a "good mechanic" from 1565 to 1821 to argue that working men had never been as well-off in terms of purchasing power as they had become toward the end of this period.</p>
<p>His graph is a classic in the history of data visualization, but commits the sin of showing two non-commensurable Y variables on different axes. Scatterplots of wages vs. price or plots of ratios (e.g., wages/price) are in some ways better, but both of these ideas were unknown in 1821.</p>
<p>In this version, information on the reigns of British monarchs is provided in a separate data.frame, <code>Wheat.monarch</code>.</p>
<h3>Usage</h3>
<pre>
data(Wheat)
data(Wheat.monarchs)
</pre>
<h3>Format</h3>
<p><code>Wheat</code>A data frame with 53 observations on the following 3 variables.</p>
<dl>
<dt><code>Year</code></dt>
<dd>
<p>Year, in intervals of 5 from 1565 to 1821: a numeric vector</p>
</dd>
<dt><code>Wheat</code></dt>
<dd>
<p>Price of Wheat (Shillings/Quarter bushel): a numeric vector</p>
</dd>
<dt><code>Wages</code></dt>
<dd>
<p>Weekly wage (Shillings): a numeric vector</p>
</dd>
</dl>
<p><code>Wheat.monarchs</code> A data frame with 12 observations on the following 4 variables.</p>
<dl>
<dt><code>name</code></dt>
<dd>
<p>Reigning monarch, a factor with levels <code>Anne</code> <code>Charles I</code> <code>Charles II</code> <code>Cromwell</code> <code>Elizabeth</code> <code>George I</code> <code>George II</code> <code>George III</code> <code>George IV</code> <code>James I</code> <code>James II</code> <code>W&amp;M</code></p>
</dd>
<dt><code>start</code></dt>
<dd>
<p>Starting year of reign, a numeric vector</p>
</dd>
<dt><code>end</code></dt>
<dd>
<p>Starting year of reign, a numeric vector</p>
</dd>
<dt><code>commonwealth</code></dt>
<dd>
<p>A binary variable indicating the period of the Commonwealth under Cromwell</p>
</dd>
</dl>
<h3>Source</h3>
<p>Playfair, W. (1821). <em>Letter on our Agricultural Distresses, Their Causes and Remedies</em>. London: W. Sams, 1821</p>
<p>Data values: originally digitized from <a href="http://www.math.yorku.ca/SCS/Gallery/images/playfair-wheat1.gif">http://www.math.yorku.ca/SCS/Gallery/images/playfair-wheat1.gif</a> now taken from <a href="http://mbostock.github.com/protovis/ex/wheat.js">http://mbostock.github.com/protovis/ex/wheat.js</a></p>
<h3>References</h3>
<p>Friendly, M. &amp; Denis, D. (2005). The early origins and development of the scatterplot <em>Journal of the History of the Behavioral Sciences</em>, 41, 103-130.</p>
<h3>Examples</h3>
<pre>
data(Wheat)data(Wheat)# ------------------------------------
# Playfair's graph, largely reproduced
# ------------------------------------# convenience function to fill area under a curve down to a minimum value
fillpoly &lt;- function(x,y, low=min(y),...) {
n &lt;- length(x)
polygon( c(x, x[n], x[1]), c(y, low, low), ...)
}# For best results, this graph should be viewed with width ~ 2 * height
# Note use of type='s' to plot a step function for Wheat
# and panel.first to provide a background grid()
# The curve for Wages is plotted after the polygon below it is filled
with(Wheat, {
plot(Year, Wheat, type="s", ylim=c(0,105), 
ylab="Price of the Quarter of Wheat (shillings)", 
panel.first=grid(col=gray(.9), lty=1))
fillpoly(Year, Wages, low=0, col="lightskyblue", border=NA)
lines(Year, Wages, lwd=3, col="red")
})
# add some annotations
text(1625,10, "Weekly wages of a good mechanic", cex=0.8, srt=3, col="red")# cartouche
text(1650, 85, "Chart", cex=2, font=2)
text(1650, 70, 
paste("Shewing at One View", 
"The Price of the Quarter of Wheat", 
"&amp; Wages of Labor by the Week", 
"from the Year 1565 to 1821",
"by William Playfair",
sep="\n"), font=3)# add the time series bars to show reigning monarchs
# distinguish Cromwell visually, as Playfair did
with(Wheat.monarchs, {
y &lt;- ifelse( !commonwealth &amp; (!seq_along(start) %% 2), 102, 104)
segments(start, y, end, y, col="black", lwd=7, lend=1)
segments(start, y, end, y, col=ifelse(commonwealth, "white", NA), lwd=4, lend=1)
text((start+end)/2, y-2, name, cex=0.5)
})# -----------------------------------------
# plot the labor cost of a quarter of wheat
# -----------------------------------------
Wheat1 &lt;- within(na.omit(Wheat), {Labor=Wheat/Wages})
with(Wheat1, {
plot(Year, Labor, type='b', pch=16, cex=1.5, lwd=1.5, 
 ylab="Labor cost of a Quarter of Wheat (weeks)",
 ylim=c(1,12.5));
lines(lowess(Year, Labor), col="red", lwd=2)
})

# cartouche
text(1740, 10, "Chart", cex=2, font=2)
text(1740, 8.5, 
paste("Shewing at One View", 
"The Work Required to Purchase", 
"One Quarter of Wheat", 
sep="\n"), cex=1.5, font=3)with(Wheat.monarchs, {
y &lt;- ifelse( !commonwealth &amp; (!seq_along(start) %% 2), 12.3, 12.5)
segments(start, y, end, y, col="black", lwd=7, lend=1)
segments(start, y, end, y, col=ifelse(commonwealth, "white", NA), lwd=4, lend=1)
text((start+end)/2, y-0.2, name, cex=0.5)
})
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-77745.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-77745.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-histdata-wheatmonarchs.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-77745.json';</script>