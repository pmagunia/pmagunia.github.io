---
title: R Dataset / Package DAAG / roller
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">roller</span> data set which pertains to Lawn Roller Data. The <span class="mono">roller</span> data set is found in the <span class="mono">DAAG</span> R package. You can load the <span class="mono">roller</span> data set in R by issuing the following command at the console <span class="mono">data("roller")</span>. This will load the data into a variable called <span class="mono">roller</span>. If R says the <span class="mono">roller</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("DAAG")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-97560.csv">roller R data set</a></span>. The size of this file is about 89 bytes.</p><h2>Lawn Roller Data</h2>
<h3>Description</h3>
<p>The <code>roller</code> data frame has 10 rows and 2 columns. Different weights of roller were rolled over different parts of a lawn, and the depression was recorded.</p>
<h3>Usage</h3>
<pre>roller</pre>
<h3>Format</h3>
<p>This data frame contains the following columns:</p>
<dl>
<dt>weight</dt>
<dd>
<p>a numeric vector consisting of the roller weights</p>
</dd>
<dt>depression</dt>
<dd>
<p>the depth of the depression made in the grass under the roller</p>
</dd>
</dl>
<h3>Source</h3>
<p>Stewart, K.M., Van Toor, R.F., Crosbie, S.F. 1988. Control of grass grub (Coleoptera: Scarabaeidae) with rollers of different design. N.Z. Journal of Experimental Agriculture 16: 141-150.</p>
<h3>Examples</h3>
<pre>
plot(roller)
roller.lm &lt;- lm(depression ~ weight, data = roller)
plot(roller.lm, which = 4)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-97560.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-97560.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-daag-roller.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-97560.json';</script>