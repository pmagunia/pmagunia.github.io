---
title: R Dataset / Package datasets / morley
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">morley</span> data set which pertains to Michelson Speed of Light Data. The <span class="mono">morley</span> data set is found in the <span class="mono">datasets</span> R package. You can load the <span class="mono">morley</span> data set in R by issuing the following command at the console <span class="mono">data("morley")</span>. This will load the data into a variable called <span class="mono">morley</span>. If R says the <span class="mono">morley</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("datasets")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-77488.csv">morley R data set</a></span>. The size of this file is about 880 bytes.</p><h2>Michelson Speed of Light Data</h2>
<h3>Description</h3>
<p>A classical data of Michelson (but not this one with Morley) on measurements done in 1879 on the speed of light. The data consists of five experiments, each consisting of 20 consecutive ‘runs’. The response is the speed of light measurement, suitably coded (km/sec, with <code>299000</code> subtracted).</p>
<h3>Usage</h3>
<pre>
morley
</pre>
<h3>Format</h3>
<p>A data frame with 100 observations on the following 3 variables.</p>
<dl>
<dt><code>Expt</code></dt>
<dd>
<p>The experiment number, from 1 to 5.</p>
</dd>
<dt><code>Run</code></dt>
<dd>
<p>The run number within each experiment.</p>
</dd>
<dt><code>Speed</code></dt>
<dd>
<p>Speed-of-light measurement.</p>
</dd>
</dl>
<h3>Details</h3>
<p>The data is here viewed as a randomized block experiment with ‘experiment’ and ‘run’ as the factors. ‘run’ may also be considered a quantitative variate to account for linear (or polynomial) changes in the measurement over the course of a single experiment.</p>
<h3>Note</h3>
<p>This is the same dataset as <code>michelson</code> in package <a href="https://CRAN.R-project.org/package=MASS"><span class="pkg">MASS</span></a>.</p>
<h3>Source</h3>
<p>A. J. Weekes (1986) <em>A Genstat Primer</em>. London: Edward Arnold.</p>
<p>S. M. Stigler (1977) Do robust estimators work with real data? <em>Annals of Statistics</em> <b>5</b>, 1055–1098. (See Table 6.)</p>
<p>A. A. Michelson (1882) Experimental determination of the velocity of light made at the United States Naval Academy, Annapolis. <em>Astronomic Papers</em> <b>1</b> 135–8. U.S. Nautical Almanac Office. (See Table 24.)</p>
<h3>Examples</h3>
<pre>
require(stats); require(graphics)
michelson &lt;- transform(morley,
 Expt = factor(Expt), Run = factor(Run))
xtabs(~ Expt + Run, data = michelson)# 5 x 20 balanced (two-way)
plot(Speed ~ Expt, data = michelson,
 main = "Speed of Light Data", xlab = "Experiment No.")
fm &lt;- aov(Speed ~ Run + Expt, data = michelson)
summary(fm)
fm0 &lt;- update(fm, . ~ . - Run)
anova(fm0, fm)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-77488.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-77488.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-datasets-morley.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-77488.json';</script>