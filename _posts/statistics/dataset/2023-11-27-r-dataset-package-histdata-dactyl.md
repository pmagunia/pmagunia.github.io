---
title: R Dataset / Package HistData / Dactyl
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">Dactyl</span> data set which pertains to Edgeworth's counts of dactyls in Virgil's Aeneid. The <span class="mono">Dactyl</span> data set is found in the <span class="mono">HistData</span> R package. You can load the <span class="mono">Dactyl</span> data set in R by issuing the following command at the console <span class="mono">data("Dactyl")</span>. This will load the data into a variable called <span class="mono">Dactyl</span>. If R says the <span class="mono">Dactyl</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("HistData")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-75441.csv">Dactyl R data set</a></span>. The size of this file is about 851 bytes.</p><h2>Edgeworth's counts of dactyls in Virgil's Aeneid</h2>
<h3>Description</h3>
<p>Edgeworth (1885) took the first 75 lines in Book XI of Virgil's <em>Aeneid</em> and classified each of the first four "feet" of the line as a dactyl (one long syllable followed by two short ones) or not.</p>
<p>Grouping the lines in blocks of five gave a 4 x 25 table of counts, represented here as a data frame with ordered factors, <code>Foot</code> and <code>Lines</code>. Edgeworth used this table in what was among the first examples of analysis of variance applied to a two-way classification.</p>
<h3>Usage</h3>
<pre>data(Dactyl)</pre>
<h3>Format</h3>
<p>A data frame with 60 observations on the following 3 variables.</p>
<dl>
<dt><code>Foot</code></dt>
<dd>
<p>an ordered factor with levels <code>1</code> &lt; <code>2</code> &lt; <code>3</code> &lt; <code>4</code></p>
</dd>
<dt><code>Lines</code></dt>
<dd>
<p>an ordered factor with levels <code>1:5</code> &lt; <code>6:10</code> &lt; <code>11:15</code> &lt; <code>16:20</code> &lt; <code>21:25</code> &lt; <code>26:30</code> &lt; <code>31:35</code> &lt; <code>36:40</code> &lt; <code>41:45</code> &lt; <code>46:50</code> &lt; <code>51:55</code> &lt; <code>56:60</code> &lt; <code>61:65</code> &lt; <code>66:70</code> &lt; <code>71:75</code></p>
</dd>
<dt><code>count</code></dt>
<dd>
<p>number of dactyls</p>
</dd>
</dl>
<h3>Source</h3>
<p>Stigler, S. (1999) <em>Statistics on the Table</em> Cambridge, MA: Harvard University Press, table 5.1.</p>
<h3>References</h3>
<p>Edgeworth, F. Y. (1885). On methods of ascertaining variations in the rate of births, deaths and marriages. <em>Journal of the [Royal] Statistical Society</em>, 48, 628-649.</p>
<h3>Examples</h3>
<pre>
data(Dactyl)# display the basic table
xtabs(count ~ Foot+Lines, data=Dactyl)# simple two-way anova
anova(dact.lm &lt;- lm(count ~ Foot+Lines, data=Dactyl))# plot the lm-quartet
op &lt;- par(mfrow=c(2,2))
plot(dact.lm)
par(op)# show table as a simple mosaicplot
mosaicplot(xtabs(count ~ Foot+Lines, data=Dactyl), shade=TRUE)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-75441.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-75441.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-histdata-dactyl.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-75441.json';</script>