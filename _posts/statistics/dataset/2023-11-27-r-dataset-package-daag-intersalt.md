---
title: R Dataset / Package DAAG / intersalt
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">intersalt</span> data set which pertains to Blood pressure versus Salt; inter-population data. The <span class="mono">intersalt</span> data set is found in the <span class="mono">DAAG</span> R package. You can load the <span class="mono">intersalt</span> data set in R by issuing the following command at the console <span class="mono">data("intersalt")</span>. This will load the data into a variable called <span class="mono">intersalt</span>. If R says the <span class="mono">intersalt</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("DAAG")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-28920.csv">intersalt R data set</a></span>. The size of this file is about 1,342 bytes.</p><h2>Blood pressure versus Salt; inter-population data</h2>
<h3>Description</h3>
<p>Median blood pressure, as a fuction of salt intake, for each of 52 human populations.</p>
<h3>Usage</h3>
<pre>intersalt</pre>
<h3>Format</h3>
<p>A data frame with 52 observations on the following 4 variables.</p>
<dl>
<dt><code>b</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt><code>bp</code></dt>
<dd>
<p>mean diastolic blood pressure (mm Hg)</p>
</dd>
<dt><code>na</code></dt>
<dd>
<p>mean sodium excretion (mmol/24h)</p>
</dd>
<dt><code>country</code></dt>
<dd>
<p>a character vector</p>
</dd>
</dl>
<h3>Details</h3>
<p>For each population took a sample of 25 males and 25 females from each decade in the age range 20 - 50, i.e. 200 individuals in all.</p>
<h3>Source</h3>
<p>Intersalt Cooperative Research Group. 1988. Intersalt: an international study of electrolyte excretion and blood pressure: results for 24 hour urinary sodium and potassium excretion. <em>British Medical Journal</em> 297: 319-328.</p>
<h3>References</h3>
<p>Maindonald, J.H. <em>The Design of Research Studies ? A Statistical Perspective</em>, viii + 109pp. Graduate School Occasional Paper 00/2, Australian National University 2000.</p>
<h3>Examples</h3>
<pre>
data(intersalt)
plot(bp ~ na, data=intersalt, xlab="Median sodium excretion (mmol/24h)",
 ylab="Median diatoluc blood pressure (mm Hg)")
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-28920.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-28920.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-daag-intersalt.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-28920.json';</script>