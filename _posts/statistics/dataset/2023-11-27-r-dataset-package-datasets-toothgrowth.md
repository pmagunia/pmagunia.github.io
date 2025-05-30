---
title: R Dataset / Package datasets / ToothGrowth
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">ToothGrowth</span> data set which pertains to The Effect of Vitamin C on Tooth Growth in Guinea Pigs. The <span class="mono">ToothGrowth</span> data set is found in the <span class="mono">datasets</span> R package. You can load the <span class="mono">ToothGrowth</span> data set in R by issuing the following command at the console <span class="mono">data("ToothGrowth")</span>. This will load the data into a variable called <span class="mono">ToothGrowth</span>. If R says the <span class="mono">ToothGrowth</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("datasets")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-16324.csv">ToothGrowth R data set</a></span>. The size of this file is about 760 bytes.</p><h2>The Effect of Vitamin C on Tooth Growth in Guinea Pigs</h2>
<h3>Description</h3>
<p>The response is the length of odontoblasts (cells responsible for tooth growth) in 60 guinea pigs. Each animal received one of three dose levels of vitamin C (0.5, 1, and 2 mg/day) by one of two delivery methods, (orange juice or ascorbic acid (a form of vitamin C and coded as <code>VC</code>).</p>
<h3>Usage</h3>
<pre>ToothGrowth</pre>
<h3>Format</h3>
<p>A data frame with 60 observations on 3 variables.</p>
<table>
<caption>
R project statistics dataset table
</caption>
<tr>
<td style="text-align: right;">[,1]</td>
<td style="text-align: left;">len</td>
<td style="text-align: left;">numeric</td>
<td style="text-align: left;">Tooth length</td>
</tr>
<tr>
<td style="text-align: right;">[,2]</td>
<td style="text-align: left;">supp</td>
<td style="text-align: left;">factor</td>
<td style="text-align: left;">Supplement type (VC or OJ).</td>
</tr>
<tr>
<td style="text-align: right;">[,3]</td>
<td style="text-align: left;">dose</td>
<td style="text-align: left;">numeric</td>
<td style="text-align: left;">Dose in milligrams/day</td>
</tr>
</table>
<h3>Source</h3>
<p>C. I. Bliss (1952) <em>The Statistics of Bioassay</em>. Academic Press.</p>
<h3>References</h3>
<p>McNeil, D. R. (1977) <em>Interactive Data Analysis</em>. New York: Wiley.</p>
<p>Crampton, E. W. (1947) The growth of the odontoblast of the incisor teeth as a criterion of vitamin C intake of the guinea pig. <em>The Journal of Nutrition</em> <b>33(5)</b>: 491–504. <a href="http://jn.nutrition.org/content/33/5/491.full.pdf">http://jn.nutrition.org/content/33/5/491.full.pdf</a></p>
<h3>Examples</h3>
<pre>
require(graphics)
coplot(len ~ dose | supp, data = ToothGrowth, panel = panel.smooth,
 xlab = "ToothGrowth data: length vs dose, given type of supplement")
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-16324.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-16324.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-datasets-toothgrowth.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-16324.json';</script>