---
title: R Dataset / Package robustbase / pilot
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">pilot</span> data set which pertains to Pilot-Plant Data. The <span class="mono">pilot</span> data set is found in the <span class="mono">robustbase</span> R package. You can load the <span class="mono">pilot</span> data set in R by issuing the following command at the console <span class="mono">data("pilot")</span>. This will load the data into a variable called <span class="mono">pilot</span>. If R says the <span class="mono">pilot</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("robustbase")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-57616.csv">pilot R data set</a></span>. The size of this file is about 140 bytes.</p><h2>Pilot-Plant Data</h2>
<h3>Description</h3>
<p>Pilot-Plant data from Daniel and Wood (1971). The response variable corresponds to the acid content determined by titration and the explanatory variable is the organic acid content determined by extraction and weighing. This data set was analyzed also by Yale and Forsythe (1976).</p>
<h3>Usage</h3>
<pre>data(pilot)</pre>
<h3>Format</h3>
<p>A data frame with 20 observations on the following 2 variables.</p>
<dl>
<dt><code>X</code></dt>
<dd>
<p>Organic acid content - extraction</p>
</dd>
<dt><code>Y</code></dt>
<dd>
<p>Acid content - titration</p>
</dd>
</dl>
<h3>Source</h3>
<p>P. J. Rousseeuw and A. M. Leroy (1987) <em>Robust Regression and Outlier Detection</em>; Wiley, page 21, table 1.</p>
<h3>Examples</h3>
<pre>
data(pilot)
summary(lm.pilot &lt;- lm(Y ~.,data=pilot))</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-57616.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-57616.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-robustbase-pilot.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-57616.json';</script>