---
title: R Dataset / Package wooldridge / loanapp
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">loanapp</span> data set which pertains to loanapp. The <span class="mono">loanapp</span> data set is found in the <span class="mono">wooldridge</span> R package. You can load the <span class="mono">loanapp</span> data set in R by issuing the following command at the console <span class="mono">data("loanapp")</span>. This will load the data into a variable called <span class="mono">loanapp</span>. If R says the <span class="mono">loanapp</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("wooldridge")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-53620.csv">loanapp R data set</a></span>. The size of this file is about 370,913 bytes.</p><h2>loanapp</h2>
<h3>Description</h3>
<p>Data loads lazily. Type data(loanapp) into the console.</p>
<h3>Usage</h3>
<pre>
data(loanapp)
</pre>
<h3>Format</h3>
<p>A data.frame with 1989 rows and 59 variables:</p>
<ul>
<li>
<p>occ. occupancy</p>
</li>
<li>
<p>loanamt. loan amt in thousands</p>
</li>
<li>
<p>action. type of action taken</p>
</li>
<li>
<p>msa. msa number of property</p>
</li>
<li>
<p>suffolk. =1 if property in suffolk co.</p>
</li>
<li>
<p>appinc. applicant income, $1000s</p>
</li>
<li>
<p>typur. type of purchaser of loan</p>
</li>
<li>
<p>unit. number of units in property</p>
</li>
<li>
<p>married. =1 if applicant married</p>
</li>
<li>
<p>dep. number of dependents</p>
</li>
<li>
<p>emp. years employed in line of work</p>
</li>
<li>
<p>yjob. years at this job</p>
</li>
<li>
<p>self. =1 if self employed</p>
</li>
<li>
<p>atotinc. total monthly income</p>
</li>
<li>
<p>cototinc. coapp total monthly income</p>
</li>
<li>
<p>hexp. propose housing expense</p>
</li>
<li>
<p>price. purchase price</p>
</li>
<li>
<p>other. other financing, $1000s</p>
</li>
<li>
<p>liq. liquid assets</p>
</li>
<li>
<p>rep. no. of credit reports</p>
</li>
<li>
<p>gdlin. credit history meets guidelines</p>
</li>
<li>
<p>lines. no. of credit lines on reports</p>
</li>
<li>
<p>mortg. credit history on mortgage paym</p>
</li>
<li>
<p>cons. credit history on consumer stuf</p>
</li>
<li>
<p>pubrec. =1 if filed bankruptcy</p>
</li>
<li>
<p>hrat. housing exp, percent total inc</p>
</li>
<li>
<p>obrat. other oblgs, percent total inc</p>
</li>
<li>
<p>fixadj. fixed or adjustable rate?</p>
</li>
<li>
<p>term. term of loan in months</p>
</li>
<li>
<p>apr. appraised value</p>
</li>
<li>
<p>prop. type of property</p>
</li>
<li>
<p>inss. PMI sought</p>
</li>
<li>
<p>inson. PMI approved</p>
</li>
<li>
<p>gift. gift as down payment</p>
</li>
<li>
<p>cosign. is there a cosigner</p>
</li>
<li>
<p>unver. unverifiable info</p>
</li>
<li>
<p>review. number of times reviewed</p>
</li>
<li>
<p>netw. net worth</p>
</li>
<li>
<p>unem. unemployment rate by industry</p>
</li>
<li>
<p>min30. =1 if minority pop. &gt; 30percent</p>
</li>
<li>
<p>bd. =1 if boarded-up val &gt; MSA med</p>
</li>
<li>
<p>mi. =1 if tract inc &gt; MSA median</p>
</li>
<li>
<p>old. =1 if applic age &gt; MSA median</p>
</li>
<li>
<p>vr. =1 if tract vac rte &gt; MSA med</p>
</li>
<li>
<p>sch. =1 if &gt; 12 years schooling</p>
</li>
<li>
<p>black. =1 if applicant black</p>
</li>
<li>
<p>hispan. =1 if applicant Hispanic</p>
</li>
<li>
<p>male. =1 if applicant male</p>
</li>
<li>
<p>reject. =1 if action == 3</p>
</li>
<li>
<p>approve. =1 if action == 1 or 2</p>
</li>
<li>
<p>mortno. no mortgage history</p>
</li>
<li>
<p>mortperf. no late mort. payments</p>
</li>
<li>
<p>mortlat1. one or two late payments</p>
</li>
<li>
<p>mortlat2. &gt; 2 late payments</p>
</li>
<li>
<p>chist. =0 if accnts deliq. &gt;= 60 days</p>
</li>
<li>
<p>multi. =1 if two or more units</p>
</li>
<li>
<p>loanprc. amt/price</p>
</li>
<li>
<p>thick. =1 if rep &gt; 2</p>
</li>
<li>
<p>white. =1 if applicant white</p>
</li>
</ul>
<h3>Source</h3>
<p><a href="https://www.cengage.com/cgi-wadsworth/course_products_wp.pl?fid=M20b&amp;product_isbn_issn=9781111531041">https://www.cengage.com/cgi-wadsworth/course_products_wp.pl?fid=M20b&amp;product_isbn_issn=9781111531041</a></p>
<h3>Examples</h3>
<pre>
 str(loanapp)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-53620.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-53620.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-wooldridge-loanapp.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-53620.json';</script>