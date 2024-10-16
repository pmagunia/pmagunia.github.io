---
title: R Dataset / Package wooldridge / prison
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">prison</span> data set which pertains to prison. The <span class="mono">prison</span> data set is found in the <span class="mono">wooldridge</span> R package. You can load the <span class="mono">prison</span> data set in R by issuing the following command at the console <span class="mono">data("prison")</span>. This will load the data into a variable called <span class="mono">prison</span>. If R says the <span class="mono">prison</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("wooldridge")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-26543.csv">prison R data set</a></span>. The size of this file is about 383,138 bytes.</p><h2>prison</h2>
<h3>Description</h3>
<p>Data loads lazily. Type data(prison) into the console.</p>
<h3>Usage</h3>
<pre>
data(prison)
</pre>
<h3>Format</h3>
<p>A data.frame with 714 rows and 45 variables:</p>
<ul>
<li>
<p>state. alphabetical; DC = 9</p>
</li>
<li>
<p>year. 80 to 93</p>
</li>
<li>
<p>govelec. =1 if gubernatorial election</p>
</li>
<li>
<p>black. proportion black</p>
</li>
<li>
<p>metro. proportion in metro. areas</p>
</li>
<li>
<p>unem. proportion unemployed</p>
</li>
<li>
<p>criv. viol. crimes per 100,000</p>
</li>
<li>
<p>crip. prop. crimes per 100,000</p>
</li>
<li>
<p>lcriv. log(criv)</p>
</li>
<li>
<p>lcrip. log(crip)</p>
</li>
<li>
<p>gcriv. lcriv - lcriv_1</p>
</li>
<li>
<p>gcrip. lcrip - lcrip_1</p>
</li>
<li>
<p>y81. =1 if year == 81</p>
</li>
<li>
<p>y82.</p>
</li>
<li>
<p>y83.</p>
</li>
<li>
<p>y84.</p>
</li>
<li>
<p>y85.</p>
</li>
<li>
<p>y86.</p>
</li>
<li>
<p>y87.</p>
</li>
<li>
<p>y88.</p>
</li>
<li>
<p>y89.</p>
</li>
<li>
<p>y90.</p>
</li>
<li>
<p>y91.</p>
</li>
<li>
<p>y92.</p>
</li>
<li>
<p>y93.</p>
</li>
<li>
<p>ag0_14. prop. pop. 0 to 14 yrs</p>
</li>
<li>
<p>ag15_17. prop. pop. 15 to 17 yrs</p>
</li>
<li>
<p>ag18_24. prop. pop. 18 to 24 yrs</p>
</li>
<li>
<p>ag25_34. prop. pop. 25 to 34 yrs</p>
</li>
<li>
<p>incpc. per capita income, nominal</p>
</li>
<li>
<p>polpc. police per 100,000 residents</p>
</li>
<li>
<p>gincpc. log(incpc) - log(incpc_1)</p>
</li>
<li>
<p>gpolpc. lpolpc - lpolpc_1</p>
</li>
<li>
<p>cag0_14. change in ag0_14</p>
</li>
<li>
<p>cag15_17. change in ag15_17</p>
</li>
<li>
<p>cag18_24. change in ag18_24</p>
</li>
<li>
<p>cag25_34. change in ag25_34</p>
</li>
<li>
<p>cunem. change in unem</p>
</li>
<li>
<p>cblack. change in black</p>
</li>
<li>
<p>cmetro. change in metro</p>
</li>
<li>
<p>pris. prison pop. per 100,000</p>
</li>
<li>
<p>lpris. log(pris)</p>
</li>
<li>
<p>gpris. lpris - lpris[_n-1]</p>
</li>
<li>
<p>final1. =1 if fnl dec on litig, curr yr</p>
</li>
<li>
<p>final2. =1 if dec on litig, prev 2 yrs</p>
</li>
</ul>
<h3>Source</h3>
<p><a href="https://www.cengage.com/cgi-wadsworth/course_products_wp.pl?fid=M20b&amp;product_isbn_issn=9781111531041">https://www.cengage.com/cgi-wadsworth/course_products_wp.pl?fid=M20b&amp;product_isbn_issn=9781111531041</a></p>
<h3>Examples</h3>
<pre>
 str(prison)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-26543.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-26543.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-wooldridge-prison.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-26543.json';</script>