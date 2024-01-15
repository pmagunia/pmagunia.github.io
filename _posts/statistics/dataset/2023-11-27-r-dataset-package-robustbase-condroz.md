---
title: R Dataset / Package robustbase / condroz
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">condroz</span> data set which pertains to Condroz Data . The <span class="mono">condroz</span> data set is found in the <span class="mono">robustbase</span> R package. You can load the <span class="mono">condroz</span> data set in R by issuing the following command at the console <span class="mono">data("condroz")</span>. This will load the data into a variable called <span class="mono">condroz</span>. If R says the <span class="mono">condroz</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("robustbase")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-33291.csv">condroz R data set</a></span>. The size of this file is about 3,394 bytes.</p><h2>Condroz Data</h2>
<h3>Description</h3>
<p>Dataset with pH-value and Calcium content in soil samples, collected in different communities of the Condroz region in Belgium. The data pertain to a subset of 428 samples with a pH-value between 7.0 and 7.5.</p>
<h3>Usage</h3>
<pre>data(condroz)</pre>
<h3>Format</h3>
<p>A data frame with 428 observations on the following 2 variables.</p>
<dl>
<dt><code>Ca</code></dt>
<dd>
<p>Calcium content of the soil sample</p>
</dd>
<dt><code>pH</code></dt>
<dd>
<p>pH value of the soil sample</p>
</dd>
</dl>
<h3>Details</h3>
<p>For more information on the dataset, cf. Goegebeur et al. (2005).</p>
<h3>Source</h3>
<p>Hubert and Vandervieren (2006), p. 10. This dataset is also studied in Vandewalle et al. (2004).</p>
<h3>References</h3>
<p>See also those for <code>adjbox</code>.</p>
<p>Goegebeur, Y., Planchon, V., Beirlant, J., Oger, R. (2005). Quality Assesment of Pedochemical Data Using Extreme Value Methodology, Journal of Applied Science, 5, p. 1092-1102.</p>
<p>Vandewalle, B., Beirlant, J., Hubert, M. (2004). A robust estimator of the tail index based on an exponential regression model, in Hubert, M., Pison G., Struyf, A. and S. Van Aelst, ed., Theory and Applications of Recent Robust Methods, Birkhäuser, Basel, p. 367-376.</p>
<h3>Examples</h3>
<pre>
adjbox(condroz$Ca)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-33291.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-33291.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-robustbase-condroz.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-33291.json';</script>