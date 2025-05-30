---
title: R Dataset / Package pscl / iraqVote
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">iraqVote</span> data set which pertains to U.S. Senate vote on the use of force against Iraq, 2002. . The <span class="mono">iraqVote</span> data set is found in the <span class="mono">pscl</span> R package. You can load the <span class="mono">iraqVote</span> data set in R by issuing the following command at the console <span class="mono">data("iraqVote")</span>. This will load the data into a variable called <span class="mono">iraqVote</span>. If R says the <span class="mono">iraqVote</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("pscl")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-19261.csv">iraqVote R data set</a></span>. The size of this file is about 4,688 bytes.</p><h2>U.S. Senate vote on the use of force against Iraq, 2002.</h2>
<h3>Description</h3>
<p>On October 11, 2002, the United States Senate voted 77-23 to authorize the use of military force against Iraq. This data set lists the “Ayes” and “Nays” for each Senator and some covariates.</p>
<h3>Usage</h3>
<pre>data(iraqVote)</pre>
<h3>Format</h3>
<p>A data frame with 100 observations on the following 6 variables.</p>
<dl>
<dt><code>y</code></dt>
<dd>
<p>a numeric vector, the recorded vote (1 if Aye, 0 if Nay)</p>
</dd>
<dt><code>state.abb</code></dt>
<dd>
<p>two letter abbreviation for each state</p>
</dd>
<dt><code>name</code></dt>
<dd>
<p>senator name, party and state, e.g., <code>AKAKA (D HI)</code></p>
</dd>
<dt><code>rep</code></dt>
<dd>
<p>logical, <code>TRUE</code> for Republican senators</p>
</dd>
<dt><code>state.name</code></dt>
<dd>
<p>name of state</p>
</dd>
<dt><code>gorevote</code></dt>
<dd>
<p>numeric, the vote share recorded by Al Gore in the corresponding state in the 2000 Presidential election</p>
</dd>
</dl>
<h3>Details</h3>
<p>The only Republican to vote against the resolution was Lincoln Chafee (Rhode Island); Democrats split 29-22 in favor of the resolution.</p>
<h3>Source</h3>
<p>Keith Poole, 107th Senate Roll Call Data. <a href="ftp://voteview.com/sen107kh.ord">ftp://voteview.com/sen107kh.ord</a> The Iraq vote is vote number 617.</p>
<p>David Leip's Atlas of U.S. Presidential Elections. <a href="http://uselectionatlas.org">http://uselectionatlas.org</a></p>
<h3>References</h3>
<p>Jackman, Simon. 2009. <em>Bayesian Analysis for the Social Sciences</em>. Wiley: Chichester. Example 8.3.</p>
<h3>Examples</h3>
<pre>
data(iraqVote)
## probit model
glm1 &lt;- glm(y ~ gorevote + rep,
data=iraqVote,
family=binomial(link=probit))
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-19261.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-19261.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-pscl-iraqvote.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-19261.json';</script>