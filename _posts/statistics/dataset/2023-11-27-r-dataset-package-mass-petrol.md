---
title: R Dataset / Package MASS / petrol
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">petrol</span> data set which pertains to N. L. Prater's Petrol Refinery Data. The <span class="mono">petrol</span> data set is found in the <span class="mono">MASS</span> R package. You can load the <span class="mono">petrol</span> data set in R by issuing the following command at the console <span class="mono">data("petrol")</span>. This will load the data into a variable called <span class="mono">petrol</span>. If R says the <span class="mono">petrol</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("MASS")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-24175.csv">petrol R data set</a></span>. The size of this file is about 837 bytes.</p><h2>N. L. Prater's Petrol Refinery Data</h2>
<h3>Description</h3>
<p>The yield of a petroleum refining process with four covariates. The crude oil appears to come from only 10 distinct samples.</p>
<p>These data were originally used by Prater (1956) to build an estimation equation for the yield of the refining process of crude oil to gasoline.</p>
<h3>Usage</h3>
<pre>
petrol
</pre>
<h3>Format</h3>
<p>The variables are as follows</p>
<dl>
<dt><code>No</code></dt>
<dd>
<p>crude oil sample identification label. (Factor.)</p>
</dd>
<dt><code>SG</code></dt>
<dd>
<p>specific gravity, degrees API. (Constant within sample.)</p>
</dd>
<dt><code>VP</code></dt>
<dd>
<p>vapour pressure in pounds per square inch. (Constant within sample.)</p>
</dd>
<dt><code>V10</code></dt>
<dd>
<p>volatility of crude; ASTM 10% point. (Constant within sample.)</p>
</dd>
<dt><code>EP</code></dt>
<dd>
<p>desired volatility of gasoline. (The end point. Varies within sample.)</p>
</dd>
<dt><code>Y</code></dt>
<dd>
<p>yield as a percentage of crude.</p>
</dd>
</dl>
<h3>Source</h3>
<p>N. H. Prater (1956) Estimate gasoline yields from crudes. <em>Petroleum Refiner</em> <b>35</b>, 236–238.</p>
<p>This dataset is also given in D. J. Hand, F. Daly, K. McConway, D. Lunn and E. Ostrowski (eds) (1994) <em>A Handbook of Small Data Sets.</em> Chapman &amp; Hall.</p>
<h3>References</h3>
<p>Venables, W. N. and Ripley, B. D. (2002) <em>Modern Applied Statistics with S.</em> Fourth edition. Springer.</p>
<h3>Examples</h3>
<pre>
library(nlme)
Petrol &lt;- petrol
Petrol[, 2:5] &lt;- scale(as.matrix(Petrol[, 2:5]), scale = FALSE)
pet3.lme &lt;- lme(Y ~ SG + VP + V10 + EP,
random = ~ 1 | No, data = Petrol)
pet3.lme &lt;- update(pet3.lme, method = "ML")
pet4.lme &lt;- update(pet3.lme, fixed = Y ~ V10 + EP)
anova(pet4.lme, pet3.lme)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-24175.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-24175.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-mass-petrol.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-24175.json';</script>