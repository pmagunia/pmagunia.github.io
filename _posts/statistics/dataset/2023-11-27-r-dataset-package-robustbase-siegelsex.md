---
title: R Dataset / Package robustbase / SiegelsEx
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">SiegelsEx</span> data set which pertains to Siegel's Exact Fit Example Data. The <span class="mono">SiegelsEx</span> data set is found in the <span class="mono">robustbase</span> R package. You can load the <span class="mono">SiegelsEx</span> data set in R by issuing the following command at the console <span class="mono">data("SiegelsEx")</span>. This will load the data into a variable called <span class="mono">SiegelsEx</span>. If R says the <span class="mono">SiegelsEx</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("robustbase")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-17444.csv">SiegelsEx R data set</a></span>. The size of this file is about 50 bytes.</p><h2>Siegel's Exact Fit Example Data</h2>
<h3>Description</h3>
<p>A small counterexample data set devised by Andrew Siegel. Six (out of nine) data points lie on the line <i>y = 0</i> such that some robust regression estimators exhibit the “<em>exact fit</em>” property.</p>
<h3>Usage</h3>
<pre>data(SiegelsEx)</pre>
<h3>Format</h3>
<p>A data frame with 9 observations on the following 2 variables.</p>
<dl>
<dt><code>x</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt><code>y</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
</dl>
<h3>Source</h3>
<p>Emerson and Hoaglin (1983, p.139)</p>
<h3>References</h3>
<p>Peter J. Rousseeuw and Annick M. Leroy (1987) <em>Robust Regression and Outlier Detection</em> Wiley, p.60–61</p>
<h3>Examples</h3>
<pre>
data(SiegelsEx)
plot(SiegelsEx, main = "Siegel's example for 'exact fit'")
abline(lm(y ~ x, data = SiegelsEx))
abline(MASS::lqs(y ~ x, data = SiegelsEx, method = "lms"), col = 2)
legend("topright", leg = c("lm", "LMS"), col=1:2, lwd=1, inset = 1/20)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-17444.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-17444.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-robustbase-siegelsex.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-17444.json';</script>