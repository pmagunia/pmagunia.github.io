---
title: R Dataset / Package cluster / plantTraits
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">plantTraits</span> data set which pertains to Plant Species Traits Data. The <span class="mono">plantTraits</span> data set is found in the <span class="mono">cluster</span> R package. You can load the <span class="mono">plantTraits</span> data set in R by issuing the following command at the console <span class="mono">data("plantTraits")</span>. This will load the data into a variable called <span class="mono">plantTraits</span>. If R says the <span class="mono">plantTraits</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("cluster")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-37535.csv">plantTraits R data set</a></span>. The size of this file is about 17,957 bytes.</p><h2>Plant Species Traits Data</h2>
<h3>Description</h3>
<p>This dataset constitutes a description of 136 plant species according to biological attributes (morphological or reproductive)</p>
<h3>Usage</h3>
<pre>data(plantTraits)
</pre>
<h3>Format</h3>
<p>A data frame with 136 observations on the following 31 variables.</p>
<dl>
<dt><code>pdias</code></dt>
<dd>
<p>Diaspore mass (mg)</p>
</dd>
<dt><code>longindex</code></dt>
<dd>
<p>Seed bank longevity</p>
</dd>
<dt><code>durflow</code></dt>
<dd>
<p>Flowering duration</p>
</dd>
<dt><code>height</code></dt>
<dd>
<p>Plant height, an ordered factor with levels <code>1</code> &lt; <code>2</code> &lt; ... &lt; <code>8</code>.</p>
</dd>
</dl>
<dl>
<dt><code>begflow</code></dt>
<dd>
<p>Time of first flowering, an ordered factor with levels <code>1</code> &lt; <code>2</code> &lt; <code>3</code> &lt; <code>4</code> &lt; <code>5</code> &lt; <code>6</code> &lt; <code>7</code> &lt; <code>8</code> &lt; <code>9</code></p>
</dd>
</dl>
<dl>
<dt><code>mycor</code></dt>
<dd>
<p>Mycorrhizas, an ordered factor with levels <code>0</code>never &lt; <code>1</code> sometimes&lt; <code>2</code>always</p>
</dd>
<dt><code>vegaer</code></dt>
<dd>
<p>aerial vegetative propagation, an ordered factor with levels <code>0</code>never &lt; <code>1</code> present but limited&lt; <code>2</code>important.</p>
</dd>
<dt><code>vegsout</code></dt>
<dd>
<p>underground vegetative propagation, an ordered factor with 3 levels identical to <code>vegaer</code> above.</p>
</dd>
<dt><code>autopoll</code></dt>
<dd>
<p>selfing pollination, an ordered factor with levels <code>0</code>never &lt; <code>1</code>rare &lt; <code>2</code> often&lt; the rule<code>3</code></p>
</dd>
<dt><code>insects</code></dt>
<dd>
<p>insect pollination, an ordered factor with 5 levels <code>0</code> &lt; ... &lt; <code>4</code>.</p>
</dd>
<dt><code>wind</code></dt>
<dd>
<p>wind pollination, an ordered factor with 5 levels <code>0</code> &lt; ... &lt; <code>4</code>.</p>
</dd>
<dt><code>lign</code></dt>
<dd>
<p>a binary factor with levels <code>0:1</code>, indicating if plant is woody.</p>
</dd>
<dt><code>piq</code></dt>
<dd>
<p>a binary factor indicating if plant is thorny.</p>
</dd>
<dt><code>ros</code></dt>
<dd>
<p>a binary factor indicating if plant is rosette.</p>
</dd>
<dt><code>semiros</code></dt>
<dd>
<p>semi-rosette plant, a binary factor (<code>0</code>: no; <code>1</code>: yes).</p>
</dd>
<dt><code>leafy</code></dt>
<dd>
<p>leafy plant, a binary factor.</p>
</dd>
<dt><code>suman</code></dt>
<dd>
<p>summer annual, a binary factor.</p>
</dd>
<dt><code>winan</code></dt>
<dd>
<p>winter annual, a binary factor.</p>
</dd>
<dt><code>monocarp</code></dt>
<dd>
<p>monocarpic perennial, a binary factor.</p>
</dd>
<dt><code>polycarp</code></dt>
<dd>
<p>polycarpic perennial, a binary factor.</p>
</dd>
<dt><code>seasaes</code></dt>
<dd>
<p>seasonal aestival leaves, a binary factor.</p>
</dd>
<dt><code>seashiv</code></dt>
<dd>
<p>seasonal hibernal leaves, a binary factor.</p>
</dd>
<dt><code>seasver</code></dt>
<dd>
<p>seasonal vernal leaves, a binary factor.</p>
</dd>
<dt><code>everalw</code></dt>
<dd>
<p>leaves always evergreen, a binary factor.</p>
</dd>
<dt><code>everparti</code></dt>
<dd>
<p>leaves partially evergreen, a binary factor.</p>
</dd>
<dt><code>elaio</code></dt>
<dd>
<p>fruits with an elaiosome (dispersed by ants), a binary factor.</p>
</dd>
<dt><code>endozoo</code></dt>
<dd>
<p>endozoochorous fruits, a binary factor.</p>
</dd>
<dt><code>epizoo</code></dt>
<dd>
<p>epizoochorous fruits, a binary factor.</p>
</dd>
<dt><code>aquat</code></dt>
<dd>
<p>aquatic dispersal fruits, a binary factor.</p>
</dd>
<dt><code>windgl</code></dt>
<dd>
<p>wind dispersed fruits, a binary factor.</p>
</dd>
<dt><code>unsp</code></dt>
<dd>
<p>unspecialized mechanism of seed dispersal, a binary factor.</p>
</dd>
</dl>
<h3>Details</h3>
<p>Most of factor attributes are not disjunctive. For example, a plant can be usually pollinated by insects but sometimes self-pollination can occured.</p>
<h3>Source</h3>
<p>Vallet, Jeanne (2005) <em>Structuration de communautés végétales et analyse comparative de traits biologiques le long d'un gradient d'urbanisation</em>. Mémoire de Master 2 'Ecologie-Biodiversité-Evolution'; Université Paris Sud XI, 30p.+ annexes (in french)</p>
<h3>Examples</h3>
<pre>
data(plantTraits)## Calculation of a dissimilarity matrix
library(cluster)
dai.b &lt;- daisy(plantTraits,
 type = list(ordratio = 4:11, symm = 12:13, asymm = 14:31))## Hierarchical classification
agn.trts &lt;- agnes(dai.b, method="ward")
plot(agn.trts, which.plots = 2, cex= 0.6)
plot(agn.trts, which.plots = 1)
cutree6 &lt;- cutree(agn.trts, k=6)
cutree6## Principal Coordinate Analysis
cmdsdai.b &lt;- cmdscale(dai.b, k=6)
plot(cmdsdai.b[, 1:2], asp = 1, col = cutree6)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-37535.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-37535.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-cluster-planttraits.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-37535.json';</script>