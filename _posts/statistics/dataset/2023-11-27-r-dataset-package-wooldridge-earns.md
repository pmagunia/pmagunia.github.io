---
title: R Dataset / Package wooldridge / earns
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">earns</span> data set which pertains to earns. The <span class="mono">earns</span> data set is found in the <span class="mono">wooldridge</span> R package. You can load the <span class="mono">earns</span> data set in R by issuing the following command at the console <span class="mono">data("earns")</span>. This will load the data into a variable called <span class="mono">earns</span>. If R says the <span class="mono">earns</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("wooldridge")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-82653.csv">earns R data set</a></span>. The size of this file is about 8,852 bytes.</p><h2>earns</h2>
<h3>Description</h3>
<p>Data loads lazily. Type data(earns) into the console.</p>
<h3>Usage</h3>
<pre>
data(earns)
</pre>
<h3>Format</h3>
<p>A data.frame with 41 rows and 14 variables:</p>
<ul>
<li>
<p>year. 1947 to 1987</p>
</li>
<li>
<p>wkearns. avg. real weekly earnings</p>
</li>
<li>
<p>wkhours. avg. weekly hours</p>
</li>
<li>
<p>outphr. output per labor hour</p>
</li>
<li>
<p>hrwage. wkearns/wkhours</p>
</li>
<li>
<p>lhrwage. log(hrwage)</p>
</li>
<li>
<p>loutphr. log(outphr)</p>
</li>
<li>
<p>t. time trend: t=1 to 47</p>
</li>
<li>
<p>ghrwage. lhrwage - lhrwage[_n-1]</p>
</li>
<li>
<p>goutphr. loutphr - loutphr[_n-1]</p>
</li>
<li>
<p>ghrwge_1. ghrwage[_n-1]</p>
</li>
<li>
<p>goutph_1. goutphr[_n-1]</p>
</li>
<li>
<p>goutph_2. goutphr[_n-2]</p>
</li>
<li>
<p>lwkhours. log(wkhours)</p>
</li>
</ul>
<h3>Source</h3>
<p><a href="https://www.cengage.com/cgi-wadsworth/course_products_wp.pl?fid=M20b&amp;product_isbn_issn=9781111531041">https://www.cengage.com/cgi-wadsworth/course_products_wp.pl?fid=M20b&amp;product_isbn_issn=9781111531041</a></p>
<h3>Examples</h3>
<pre>
 str(earns)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-82653.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-82653.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-wooldridge-earns.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-82653.json';</script>