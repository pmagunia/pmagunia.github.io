---
title: R Dataset / Package vcd / Federalist
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">Federalist</span> data set which pertains to ‘May’ in Federalist Papers. The <span class="mono">Federalist</span> data set is found in the <span class="mono">vcd</span> R package. You can load the <span class="mono">Federalist</span> data set in R by issuing the following command at the console <span class="mono">data("Federalist")</span>. This will load the data into a variable called <span class="mono">Federalist</span>. If R says the <span class="mono">Federalist</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("vcd")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-66982.csv">Federalist R data set</a></span>. The size of this file is about 60 bytes.</p><h2>‘May’ in Federalist Papers</h2>
<h3>Description</h3>
<p>Data from Mosteller &amp; Wallace (1984) investigating the use of certain keywords (‘may’ in this data set) to identify the author of 12 disputed ‘Federalist Papers’ by Alexander Hamilton, John Jay and James Madison.</p>
<h3>Usage</h3>
<pre>
data("Federalist")
</pre>
<h3>Format</h3>
<p>A 1-way table giving the number of occurrences of ‘may’ in 262 blocks of text. The variable and its levels are</p>
<table>
<caption>
R project statistics dataset table
</caption>
<tr>
<td style="text-align: right;">No</td>
<td style="text-align: left;">Name</td>
<td style="text-align: left;">Levels</td>
</tr>
<tr>
<td style="text-align: right;">1</td>
<td style="text-align: left;">nMay</td>
<td style="text-align: left;">0, 1, ..., 6</td>
</tr>
</table>
<h3>Source</h3>
<p>Michael Friendly (2000), Visualizing Categorical Data, page 19.</p>
<h3>References</h3>
<p>F. Mosteller &amp; D. L. Wallace (1984), <em>Applied Bayesian and Classical Inference: The Case of the Federalist Papers</em>. Springer-Verlag, New York, NY.</p>
<p>M. Friendly (2000), <em>Visualizing Categorical Data</em>. SAS Institute, Cary, NC.</p>
<h3>Examples</h3>
<pre>
data("Federalist")
gf &lt;- goodfit(Federalist, type = "nbinomial")
summary(gf)
plot(gf)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-66982.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-66982.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-vcd-federalist.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-66982.json';</script>