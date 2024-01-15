---
title: R Dataset / Package psych / cubits
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">cubits</span> data set which pertains to Galton's example of the relationship between height and 'cubit' or forearm length. The <span class="mono">cubits</span> data set is found in the <span class="mono">psych</span> R package. You can load the <span class="mono">cubits</span> data set in R by issuing the following command at the console <span class="mono">data("cubits")</span>. This will load the data into a variable called <span class="mono">cubits</span>. If R says the <span class="mono">cubits</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("psych")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-25319.csv">cubits R data set</a></span>. The size of this file is about 222 bytes.</p><h2>Galton's example of the relationship between height and 'cubit' or forearm length</h2>
<h3>Description</h3>
<p>Francis Galton introduced the 'co-relation' in 1888 with a paper discussing how to measure the relationship between two variables. His primary example was the relationship between height and forearm length. The data table (cubits) is taken from Galton (1888). Unfortunately, there seem to be some errors in the original data table in that the marginal totals do not match the table.</p>
<p>The data frame, <code>heights</code>, is converted from this table.</p>
<h3>Usage</h3>
<pre>data(cubits)</pre>
<h3>Format</h3>
<p>A data frame with 9 observations on the following 8 variables.</p>
<dl>
<dt><code>16.5</code></dt>
<dd>
<p>Cubit length &lt; 16.5</p>
</dd>
<dt><code>16.75</code></dt>
<dd>
<p>16.5 &lt;= Cubit length &lt; 17.0</p>
</dd>
<dt><code>17.25</code></dt>
<dd>
<p>17.0 &lt;= Cubit length &lt; 17.5</p>
</dd>
<dt><code>17.75</code></dt>
<dd>
<p>17.5 &lt;= Cubit length &lt; 18.0</p>
</dd>
<dt><code>18.25</code></dt>
<dd>
<p>18.0 &lt;= Cubit length &lt; 18.5</p>
</dd>
<dt><code>18.75</code></dt>
<dd>
<p>18.5 &lt;= Cubit length &lt; 19.0</p>
</dd>
<dt><code>19.25</code></dt>
<dd>
<p>19.0 &lt;= Cubit length &lt; 19.5</p>
</dd>
<dt><code>19.75</code></dt>
<dd>
<p>19.5 &lt;= Cubit length</p>
</dd>
</dl>
<h3>Details</h3>
<p>Sir Francis Galton (1888) published the first demonstration of the correlation coefficient. The regression (or reversion to mediocrity) of the height to the length of the left forearm (a cubit) was found to .8. There seem to be some errors in the table as published in that the row sums do not agree with the actual row sums. These data are used to create a matrix using <code>table2matrix</code> for demonstrations of analysis and displays of the data.</p>
<h3>Source</h3>
<p>Galton (1888)</p>
<h3>References</h3>
<p>Galton, Francis (1888) Co-relations and their measurement. Proceedings of the Royal Society. London Series,45,135-145,</p>
<h3>See Also</h3>
<p><code>table2matrix</code>, <code>table2df</code>, <code>ellipses</code>, <code>heights</code>, <code>peas</code>,<code>galton</code></p>
<h3>Examples</h3>
<pre>
data(cubits)
cubits
heights &lt;- table2df(cubits,labs = c("height","cubit"))
ellipses(heights,n=1,main="Galton's co-relation data set")
ellipses(jitter(heights$height,3),jitter(heights$cubit,3),pch=".",
 main="Galton's co-relation data set",xlab="height",
 ylab="Forearm (cubit)") #add in some noise to see the points
pairs.panels(heights,jiggle=TRUE,main="Galton's cubits data set")
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-25319.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-25319.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-psych-cubits.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-25319.json';</script>