---
title: R Dataset / Package DAAG / ironslag
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">ironslag</span> data set which pertains to Iron Content Measurements. The <span class="mono">ironslag</span> data set is found in the <span class="mono">DAAG</span> R package. You can load the <span class="mono">ironslag</span> data set in R by issuing the following command at the console <span class="mono">data("ironslag")</span>. This will load the data into a variable called <span class="mono">ironslag</span>. If R says the <span class="mono">ironslag</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("DAAG")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-71710.csv">ironslag R data set</a></span>. The size of this file is about 340 bytes.</p><h2>Iron Content Measurements</h2>
<h3>Description</h3>
<p>The <code>ironslag</code> data frame has 53 rows and 2 columns. Two methods for measuring the iron content in samples of slag were compared, a chemical and a magnetic method. The chemical method requires greater effort than the magnetic method.</p>
<h3>Usage</h3>
<pre>ironslag</pre>
<h3>Format</h3>
<p>This data frame contains the following columns:</p>
<dl>
<dt>chemical</dt>
<dd>
<p>a numeric vector containing the measurements coming from the chemical method</p>
</dd>
<dt>magnetic</dt>
<dd>
<p>a numeric vector containing the measurments coming from the magnetic method</p>
</dd>
</dl>
<h3>Source</h3>
<p>Hand, D.J., Daly, F., McConway, K., Lunn, D., and Ostrowski, E. eds (1993) A Handbook of Small Data Sets. London: Chapman &amp; Hall.</p>
<h3>Examples</h3>
<pre>
iron.lm &lt;- lm(chemical ~ magnetic, data = ironslag)
oldpar &lt;- par(mfrow = c(2,2))
plot(iron.lm)
par(oldpar)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-71710.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-71710.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-daag-ironslag.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-71710.json';</script>