---
title: R Dataset / Package gamclass / FARS
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">FARS</span> data set which pertains to US fatal road accident data for automobiles, 1998 to 2010. The <span class="mono">FARS</span> data set is found in the <span class="mono">gamclass</span> R package. You can load the <span class="mono">FARS</span> data set in R by issuing the following command at the console <span class="mono">data("FARS")</span>. This will load the data into a variable called <span class="mono">FARS</span>. If R says the <span class="mono">FARS</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("gamclass")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-13447.csv">FARS R data set</a></span>. The size of this file is about 11,455,059 bytes.</p><h2>US fatal road accident data for automobiles, 1998 to 2010</h2>
<h3>Description</h3>
<p>Data are from the US FARS (Fatality Analysis Recording System) archive that is intended to include every accident in which there was at least one fatality. Data are limited to vehicles where the front seat passenger seat was occupied.</p>
<h3>Usage</h3>
<pre>FARS</pre>
<h3>Format</h3>
<p>A data frame with 153338 observations on the following 17 variables.</p>
<dl>
<dt><code>caseid</code></dt>
<dd>
<p>a character vector: identifies the vehicle</p>
</dd>
<dt><code>state</code></dt>
<dd>
<p>a numeric vector. See the FARS website for details</p>
</dd>
<dt><code>age</code></dt>
<dd>
<p>a numeric vector; 998=not reported; 999=not known</p>
</dd>
<dt><code>airbag</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt><code>injury</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt><code>restraint</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt><code>sex</code></dt>
<dd>
<p>1=male, 2=female, 9=unknown</p>
</dd>
<dt><code>inimpact</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt><code>modelyr</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt><code>airbagAvail</code></dt>
<dd>
<p>a factor with levels <code>no</code> <code>yes</code> <code>NA-code</code></p>
</dd>
<dt><code>airbagDeploy</code></dt>
<dd>
<p>a factor with levels <code>no</code> <code>yes</code> <code>NA-code</code></p>
</dd>
<dt><code>Restraint</code></dt>
<dd>
<p>a factor with levels <code>no</code> <code>yes</code> <code>NA-code</code></p>
</dd>
<dt><code>D_injury</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt><code>D_airbagAvail</code></dt>
<dd>
<p>a factor with levels <code>no</code> <code>yes</code> <code>NA-code</code></p>
</dd>
<dt><code>D_airbagDeploy</code></dt>
<dd>
<p>a factor with levels <code>no</code> <code>yes</code> <code>NA-code</code></p>
</dd>
<dt><code>D_Restraint</code></dt>
<dd>
<p>a factor with levels <code>no</code> <code>yes</code> <code>NA-code</code></p>
</dd>
<dt><code>year</code></dt>
<dd>
<p>year of accident</p>
</dd>
</dl>
<h3>Details</h3>
<p>Data is for automabiles where the right passenger seat was occupied, with one observation for each such passenger. Observations for vehicles where the most harmful event was a fire or explosion or immersion or gas inhalation, or where someone fell or jumped from the vehicle, are omitted. Data are limited to vehicle body types 1 to 19,48,49,61, or 62. This excludes large trucks, pickup trucks, vans and buses. The 2009 and 2010 data does not include information on whether airbags were installed.</p>
<h3>Note</h3>
<p>The papers given as references demonstrate the use of Fatal Accident Recording System data to assess the effectiveness of airbags (even differences between different types of airbags) and seatbelts. Useful results can be obtained by matching driver mortality, with and without airabgs, to mortality rates for right front seat passengers in cars without passenger airbags.</p>
<h3>Source</h3>
<p><a href="http://www-fars.nhtsa.dot.gov/Main/index.aspx">http://www-fars.nhtsa.dot.gov/Main/index.aspx</a></p>
<h3>References</h3>
<p><a href="http://maths-people.anu.edu.au/~johnm/nzsr/taws.html">http://maths-people.anu.edu.au/~johnm/nzsr/taws.html</a></p>
<p>Olson CM, Cummings P, Rivara FP. 2006. Association of first- and second-generation air bags with front occupant death in car crashes: a matched cohort study. Am J Epidemiol 164:161-169</p>
<p>Cummings, P; McKnight, B, 2010. Accounting for vehicle, crash, and occupant characteristics in traffic crash studies. Injury Prevention 16: 363-366</p>
<p>Braver, ER; Shardell, M; Teoh, ER, 2010. <em>How have changes in air bag designs affected frontal crash mortality?</em> Ann Epidemiol 20:499-510.</p>
<h3>Examples</h3>
<pre>
data(FARS)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-13447.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-13447.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-gamclass-fars.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-13447.json';</script>