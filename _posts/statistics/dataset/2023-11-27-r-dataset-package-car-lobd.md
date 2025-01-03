---
title: R Dataset / Package car / LoBD
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">LoBD</span> data set which pertains to Cancer drug data use to provide an example of the use of the skew power distributions.. The <span class="mono">LoBD</span> data set is found in the <span class="mono">car</span> R package. You can load the <span class="mono">LoBD</span> data set in R by issuing the following command at the console <span class="mono">data("LoBD")</span>. This will load the data into a variable called <span class="mono">LoBD</span>. If R says the <span class="mono">LoBD</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("car")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-99905.csv">LoBD R data set</a></span>. The size of this file is about 2,983 bytes.</p><h2>Cancer drug data use to provide an example of the use of the skew power distributions.</h2>
<h3>Description</h3>
<p>A portion of an experiment to determine the limit of blank/limit of detection in a biochemical assay.</p>
<h3>Usage</h3>
<pre>LoBD</pre>
<h3>Format</h3>
<p>A data frame with 84 observations on the following 9 variables.</p>
<dl>
<dt><code>pool</code></dt>
<dd>
<p>a factor with levels <code>1</code> <code>2</code> <code>3</code> <code>4</code> <code>5</code> <code>6</code> <code>7</code> <code>8</code> <code>9</code> <code>10</code> <code>11</code> <code>12</code> denoting the 12 pools used in the experiment; each pool had a different level of drug.</p>
</dd>
<dt><code>I1L1</code></dt>
<dd>
<p>a numeric vector giving the measured concentration in pmol/L of drug in the assay</p>
</dd>
<dt><code>I1L2</code></dt>
<dd>
<p>a numeric vector giving the measured concentration in pmol/L of drug in the assay</p>
</dd>
<dt><code>I2L1</code></dt>
<dd>
<p>a numeric vector giving the measured concentration in pmol/L of drug in the assay</p>
</dd>
<dt><code>I2L2</code></dt>
<dd>
<p>a numeric vector giving the measured concentration in pmol/L of drug in the assay</p>
</dd>
<dt><code>I3L1</code></dt>
<dd>
<p>a numeric vector giving the measured concentration in pmol/L of drug in the assay</p>
</dd>
<dt><code>I3L2</code></dt>
<dd>
<p>a numeric vector giving the measured concentration in pmol/L of drug in the assay</p>
</dd>
<dt><code>I4L1</code></dt>
<dd>
<p>a numeric vector giving the measured concentration in pmol/L of drug in the assay</p>
</dd>
<dt><code>I4L2</code></dt>
<dd>
<p>a numeric vector giving the measured concentration in pmol/L of drug in the assay</p>
</dd>
</dl>
<h3>Details</h3>
<p>Important characteristics of a clinical chemistry assay are its limit of blank (LoB), and its limit of detection (LoD). The LoB, conceptually the highest reading likely to be obtained from a zero-concentration sample, is defined operationally by the upper 95% point of readings obtained from samples that do not contain the analyte. The LoD, conceptually the lowest level of analyte that can be reliably determined not to be blank, is defined operationally as true value at which there is a 95% chance of the reading being above the LoB.</p>
<p>These data are from a portion of a LoB/D study of an assay for a drug used to treat certain cancers. Twelve pools were used, four of them blanks of different types, and eight with successively increasing drug levels. The 8 columns of the data set refer to measurements made using different instruments I and reagent lots L.</p>
<h3>Source</h3>
<p>Used as an illustrative example for Box-Cox type transformations with negative readings in Hawkins and Weisberg (2015). For examples of its use, see <code>skewPower</code>.</p>
<h3>References</h3>
<p>Hawkins, D. and Weisberg, S. (2015) Combining the Box-Cox Power and Generalized Log Transformations to Accommodate Negative Responses, submitted for publication.</p>
<h3>Examples</h3>
<pre>
LoBD
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-99905.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-99905.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-car-lobd.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-99905.json';</script>