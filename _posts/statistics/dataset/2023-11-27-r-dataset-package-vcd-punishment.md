---
title: R Dataset / Package vcd / Punishment
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">Punishment</span> data set which pertains to Corporal Punishment Data. The <span class="mono">Punishment</span> data set is found in the <span class="mono">vcd</span> R package. You can load the <span class="mono">Punishment</span> data set in R by issuing the following command at the console <span class="mono">data("Punishment")</span>. This will load the data into a variable called <span class="mono">Punishment</span>. If R says the <span class="mono">Punishment</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("vcd")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-97599.csv">Punishment R data set</a></span>. The size of this file is about 1,279 bytes.</p><h2>Corporal Punishment Data</h2>
<h3>Description</h3>
<p>Data from a study of the Gallup Institute in Denmark in 1979 about the attitude of a random sample of 1,456 persons towards corporal punishment of children.</p>
<h3>Usage</h3>
<pre>
data("Punishment")
</pre>
<h3>Format</h3>
<p>A data frame with 36 observations and 5 variables.</p>
<dl>
<dt>Freq</dt>
<dd>
<p>frequency.</p>
</dd>
<dt>attitude</dt>
<dd>
<p>factor indicating attitude: (no, moderate) punishment of children.</p>
</dd>
<dt>memory</dt>
<dd>
<p>factor indicating whether the person had memories of corporal punishment as a child (yes, no).</p>
</dd>
<dt>education</dt>
<dd>
<p>factor indicating highest level of education (elementary, secondary, high).</p>
</dd>
<dt>age</dt>
<dd>
<p>factor indicating age group in years (15-24, 25-39, 40-).</p>
</dd>
</dl>
<h3>Note</h3>
<p>Anderson (1991) erroneously indicates the total sum of respondents to be 783.</p>
<h3>Source</h3>
<p>E. B. Andersen (1991), The Statistical Analysis of Categorical Data, pages 207–208.</p>
<h3>References</h3>
<p>E. B. Andersen (1991), <em>The Statistical Analysis of Categorical Data</em>. 2nd edition. Springer-Verlag, Berlin.</p>
<h3>Examples</h3>
<pre>
data("Punishment", package = "vcd")
pun &lt;- xtabs(Freq ~ memory + attitude + age + education, data = Punishment)## model: ~ (memory + attitude) * age * education
## use maximum sum-of-squares test/shading
cotabplot(~ memory + attitude | age + education, data = pun, panel = cotab_coindep,
n = 5000, type = "assoc", test = "maxchisq", interpolate = 1:2)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-97599.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-97599.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-vcd-punishment.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-97599.json';</script>