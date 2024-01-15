---
title: R Dataset / Package boot / aids
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">aids</span> data set which pertains to Delay in AIDS Reporting in England and Wales. The <span class="mono">aids</span> data set is found in the <span class="mono">boot</span> R package. You can load the <span class="mono">aids</span> data set in R by issuing the following command at the console <span class="mono">data("aids")</span>. This will load the data into a variable called <span class="mono">aids</span>. If R says the <span class="mono">aids</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("boot")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-75692.csv">aids R data set</a></span>. The size of this file is about 2,954 bytes.</p><h2>Delay in AIDS Reporting in England and Wales</h2>
<h3>Description</h3>
<p>The <code>aids</code> data frame has 570 rows and 6 columns.</p>
<p>Although all cases of AIDS in England and Wales must be reported to the Communicable Disease Surveillance Centre, there is often a considerable delay between the time of diagnosis and the time that it is reported. In estimating the prevalence of AIDS, account must be taken of the unknown number of cases which have been diagnosed but not reported. The data set here records the reported cases of AIDS diagnosed from July 1983 and until the end of 1992. The data are cross-classified by the date of diagnosis and the time delay in the reporting of the cases.</p>
<h3>Usage</h3>
<pre>
aids
</pre>
<h3>Format</h3>
<p>This data frame contains the following columns:</p>
<dl>
<dt><code>year</code></dt>
<dd>
<p>The year of the diagnosis.</p>
</dd>
<dt><code>quarter</code></dt>
<dd>
<p>The quarter of the year in which diagnosis was made.</p>
</dd>
<dt><code>delay</code></dt>
<dd>
<p>The time delay (in months) between diagnosis and reporting. 0 means that the case was reported within one month. Longer delays are grouped in 3 month intervals and the value of <code>delay</code> is the midpoint of the interval (therefore a value of <code>2</code> indicates that reporting was delayed for between 1 and 3 months).</p>
</dd>
<dt><code>dud</code></dt>
<dd>
<p>An indicator of censoring. These are categories for which full information is not yet available and the number recorded is a lower bound only.</p>
</dd>
<dt><code>time</code></dt>
<dd>
<p>The time interval of the diagnosis. That is the number of quarters from July 1983 until the end of the quarter in which these cases were diagnosed.</p>
</dd>
<dt><code>y</code></dt>
<dd>
<p>The number of AIDS cases reported.</p>
</dd>
</dl>
<h3>Source</h3>
<p>The data were obtained from</p>
<p>De Angelis, D. and Gilks, W.R. (1994) Estimating acquired immune deficiency syndrome accounting for reporting delay. <em>Journal of the Royal Statistical Society, A</em>, <b>157</b>, 31–40.</p>
<h3>References</h3>
<p>Davison, A.C. and Hinkley, D.V. (1997) <em>Bootstrap Methods and Their Application</em>. Cambridge University Press.</p>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-75692.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-75692.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-boot-aids.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-75692.json';</script>