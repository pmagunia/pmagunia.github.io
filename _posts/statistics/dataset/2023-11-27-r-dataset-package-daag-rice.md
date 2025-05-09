---
title: R Dataset / Package DAAG / rice
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">rice</span> data set which pertains to Genetically Modified and Wild Type Rice Data. The <span class="mono">rice</span> data set is found in the <span class="mono">DAAG</span> R package. You can load the <span class="mono">rice</span> data set in R by issuing the following command at the console <span class="mono">data("rice")</span>. This will load the data into a variable called <span class="mono">rice</span>. If R says the <span class="mono">rice</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("DAAG")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-27994.csv">rice R data set</a></span>. The size of this file is about 2,680 bytes.</p><h2>Genetically Modified and Wild Type Rice Data</h2>
<h3>Description</h3>
<p>The <code>rice</code> data frame has 72 rows and 7 columns. The data are from an experiment that compared wild type (wt) and genetically modified rice plants (ANU843), each with three different chemical treatments (F10, NH4Cl, and NH4NO3).</p>
<h3>Usage</h3>
<pre>rice</pre>
<h3>Format</h3>
<p>This data frame contains the following columns:</p>
<dl>
<dt>PlantNo</dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt>Block</dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt>RootDryMass</dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt>ShootDryMass</dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt>trt</dt>
<dd>
<p>a factor with levels <code>F10</code>, <code>NH4Cl</code>, <code>NH4NO3</code>, <code>F10 +ANU843</code>, <code>NH4Cl +ANU843</code>, <code>NH4NO3 +ANU843</code></p>
</dd>
<dt>fert</dt>
<dd>
<p>a factor with levels <code>F10</code> <code>NH4Cl</code> <code>NH4NO3</code></p>
</dd>
<dt>variety</dt>
<dd>
<p>a factor with levels <code>wt</code> <code>ANU843</code></p>
</dd>
</dl>
<h3>Source</h3>
<p>Perrine, F.M., Prayitno, J., Weinman, J.J., Dazzo, F.B. and Rolfe, B. 2001. Rhizobium plasmids are involved in the inhibition or stimulation of rice growth and development. Australian Journal of Plant Physiology 28: 923-927.</p>
<h3>Examples</h3>
<pre>
print("One and Two-Way Comparisons - Example 4.5")
attach(rice)
oldpar &lt;- par(las = 2)
stripchart(ShootDryMass ~ trt, pch=1, cex=1, xlab="Level of factor 1")
detach(rice)
pause()rice.aov &lt;- aov(ShootDryMass ~ trt, data=rice); anova(rice.aov)
anova(rice.aov)
pause()summary.lm(rice.aov)$coef
pause()rice$trt &lt;- relevel(rice$trt, ref="NH4Cl")
# Set NH4Cl as the baselinefac1 &lt;- factor(sapply(strsplit(as.character(rice$trt)," \\+"), function(x)x[1]))
anu843 &lt;- sapply(strsplit(as.character(rice$trt), "\\+"), 
function(x)c("wt","ANU843")[length(x)])
anu843 &lt;- factor(anu843, levels=c("wt", "ANU843"))
attach(rice)
interaction.plot(fac1, anu843, ShootDryMass)
detach(rice)
par(oldpar)</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-27994.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-27994.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-daag-rice.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-27994.json';</script>