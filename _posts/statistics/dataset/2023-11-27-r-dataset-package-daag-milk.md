---
title: R Dataset / Package DAAG / milk
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">milk</span> data set which pertains to Milk Sweetness Study. The <span class="mono">milk</span> data set is found in the <span class="mono">DAAG</span> R package. You can load the <span class="mono">milk</span> data set in R by issuing the following command at the console <span class="mono">data("milk")</span>. This will load the data into a variable called <span class="mono">milk</span>. If R says the <span class="mono">milk</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("DAAG")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-33271.csv">milk R data set</a></span>. The size of this file is about 3,647 bytes.</p><h2>Milk Sweetness Study</h2>
<h3>Description</h3>
<p>The <code>milk</code> data frame has 17 rows and 2 columns. Each of 17 panelists compared two milk samples for sweetness.</p>
<h3>Usage</h3>
<pre>milk</pre>
<h3>Format</h3>
<p>This data frame contains the following columns:</p>
<dl>
<dt>four</dt>
<dd>
<p>a numeric vector consisting of the assessments for four units of additive</p>
</dd>
<dt>one</dt>
<dd>
<p>a numeric vector while the is the assessment for one unit of additive</p>
</dd>
</dl>
<h3>Source</h3>
<p>J.H. Maindonald</p>
<h3>Examples</h3>
<pre>
print("Rug Plot - Example 1.8.1")
xyrange &lt;- range(milk)
plot(four ~ one, data = milk, xlim = xyrange, ylim = xyrange, pch = 16)
rug(milk$one)
rug(milk$four, side = 2)
abline(0, 1)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-33271.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-33271.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-daag-milk.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-33271.json';</script>