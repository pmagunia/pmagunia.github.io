---
title: R Dataset / Package robustbase / possumDiv
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">possumDiv</span> data set which pertains to Possum Diversity Data. The <span class="mono">possumDiv</span> data set is found in the <span class="mono">robustbase</span> R package. You can load the <span class="mono">possumDiv</span> data set in R by issuing the following command at the console <span class="mono">data("possumDiv")</span>. This will load the data into a variable called <span class="mono">possumDiv</span>. If R says the <span class="mono">possumDiv</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("robustbase")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-45000.csv">possumDiv R data set</a></span>. The size of this file is about 5,236 bytes.</p><h2>Possum Diversity Data</h2>
<h3>Description</h3>
<p>Possum diversity data: As issued from a study of the diversity of possum (arboreal marsupials) in the Montane ash forest (Australia), this dataset was collected in view of the management of hardwood forest to take conservation and recreation values, as well as wood production, into account.</p>
<p>The study is fully described in the two references. The number of different species of arboreal marsupials (possum) was observed on 151 different 3ha sites with uniform vegetation. For each site the nine variable measures (see below) were recorded. The problem is to model the relationship between <code>diversity</code> and these other variables.</p>
<h3>Usage</h3>
<pre>data(possumDiv)</pre>
<h3>Format</h3>
<p>Two different representations of the same data are available:</p>
<p><code>possumDiv</code> is a data frame of 151 observations of 9 variables, where the last two are factors, <code>eucalyptus</code> with 3 levels and <code>aspect</code> with 4 levels.</p>
<p><code>possum.mat</code> is a numeric (integer) matrix of 151 rows (observations) and 14 columns (variables) where the last seven ones are 0-1 dummy variables, three (<code>E.*</code>) are coding for the kind of <code>eucalyptus</code> and the last four are 0-1 coding for the <code>aspect</code> factor.</p>
<p>The variables have the following meaning:</p>
<dl>
<dt>Diversity</dt>
<dd>
<p>main variable of interest is the number of different species of arboreal marsupial (possum) observed, with values in 0:5.</p>
</dd>
<dt>Shrubs</dt>
<dd>
<p>the number of shrubs.</p>
</dd>
<dt>Stumps</dt>
<dd>
<p>the number of cut stumps from past logging operations.</p>
</dd>
<dt>Stags</dt>
<dd>
<p>the number of stags (hollow-bearing trees).</p>
</dd>
<dt>Bark</dt>
<dd>
<p>bark index (integer) vector reflecting the quantity of decorticating bark.</p>
</dd>
<dt>Habitat</dt>
<dd>
<p>an integer score indicating the suitability of nesting and foraging habitat for Leadbeater's possum.</p>
</dd>
<dt>BAcacia</dt>
<dd>
<p>a numeric vector giving the basal area of acacia species.</p>
</dd>
</dl>
<dl>
<dt>eucalyptus</dt>
<dd>
<p>a 3-level <code>factor</code> specifying the species of eucalypt with the greatest stand basal area. This has the same information as the following three variables</p>
</dd>
<dt>E.regnans</dt>
<dd>
<p>0-1 indicator for Eucalyptus regnans</p>
</dd>
<dt>E.delegatensis</dt>
<dd>
<p>0-1 indicator for Eucalyptus deleg.</p>
</dd>
<dt>E.nitens</dt>
<dd>
<p>0-1 indicator for Eucalyptus nitens</p>
</dd>
</dl>
<dl>
<dt>aspect</dt>
<dd>
<p>a 4-level <code>factor</code> specifying the aspect of the site. It is the same information as the following four variables.</p>
</dd>
<dt>NW-NE</dt>
<dd>
<p>0-1 indicator</p>
</dd>
<dt>NW-SE</dt>
<dd>
<p>0-1 indicator</p>
</dd>
<dt>SE-SW</dt>
<dd>
<p>0-1 indicator</p>
</dd>
<dt>SW-NW</dt>
<dd>
<p>0-1 indicator</p>
</dd>
</dl>
<h3>Source</h3>
<p>Eva Cantoni (2004) Analysis of Robust Quasi-deviances for Generalized Linear Models. <em>Journal of Statistical Software</em> <b>10</b>, 04, <a href="http://www.jstatsoft.org/v10/i04">http://www.jstatsoft.org/v10/i04</a></p>
<h3>References</h3>
<p>Lindenmayer, D. B., Cunningham, R. B., Tanton, M. T., Nix, H. A. and Smith, A. P. (1991) The conservation of arboreal marsupials in the montane ash forests of the central highlands of victoria, south-east australia: III. The habitat requirements of leadbeater's possum <em>gymnobelideus leadbeateri</em> and models of the diversity and abundance of arboreal marsupials. <em>Biological Conservation</em> <b>56</b>, 295–315.</p>
<p>Lindenmayer, D. B., Cunningham, R. B., Tanton, M. T., Smith, A. P. and Nix, H. A. (1990) The conservation of arboreal marsupials in the montane ash forests of the victoria, south-east australia, I. Factors influencing the occupancy of trees with hollows, <em>Biological Conservation</em> <b>54</b>, 111–131.</p>
<p>See also the references in <code>glmrob</code>.</p>
<h3>Examples</h3>
<pre>
data(possumDiv)
head(possum.mat)str(possumDiv)
## summarize all variables as multilevel factors:
summary(as.data.frame(lapply(possumDiv, function(v)
 if(is.integer(v)) factor(v) else v)))## Following Cantoni &amp; Ronchetti (2001), JASA, p.1026 f.:% cf. ../tests/poisson-ex.R
pdFit &lt;- glmrob(Diversity ~ . , data = possumDiv,
family=poisson, tcc = 1.6, weights.on.x = "hat", acc = 1e-15)
summary(pdFit)
summary(pdF2 &lt;- update(pdFit, ~ . -Shrubs))
summary(pdF3 &lt;- update(pdF2,~ . -eucalyptus))
summary(pdF4 &lt;- update(pdF3,~ . -Stumps))
summary(pdF5 &lt;- update(pdF4,~ . -BAcacia))
summary(pdF6 &lt;- update(pdF5,~ . -aspect))# too much ..
anova(pdFit, pdF3, pdF4, pdF5, pdF6, test = "QD") # indeed,
## indeed, the last simplification is too much
possumD.2 &lt;- within(possumDiv, levels(aspect)[1:3] &lt;- rep("other", 3))
## and use this binary 'aspect' instead of the 4-level one:
summary(pdF5.1 &lt;- update(pdF5, data = possumD.2))if(FALSE) # not ok, as formually not nested.
anova(pdF5, pdF5.1)summarizeRobWeights(weights(pdF5.1, type="rob"), eps = 0.73)
##-&gt;"outliers"(1, 59, 110)
wrob &lt;- setNames(weights(pdF5.1, type="rob"), rownames(possumDiv))
head(sort(wrob))
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-45000.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-45000.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-robustbase-possumdiv.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-45000.json';</script>
