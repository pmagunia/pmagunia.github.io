---
title: R Dataset / Package mediation / student
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">student</span> data set which pertains to Hypothetical student-level data. The <span class="mono">student</span> data set is found in the <span class="mono">mediation</span> R package. You can load the <span class="mono">student</span> data set in R by issuing the following command at the console <span class="mono">data("student")</span>. This will load the data into a variable called <span class="mono">student</span>. If R says the <span class="mono">student</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("mediation")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-33722.csv">student R data set</a></span>. The size of this file is about 283,952 bytes.</p><h2>Hypothetical student-level data</h2>
<h3>Description</h3>
<p>The original data source is the Education Longitudinal Study of 2002. To deal with the issue on individually identifiable information, we generated hypothetical student-level data using a multiple imputation method. The Education Longitudinal Study of 2002 used a two-stage sample selection process. First, a national sample of schools was selected using stratified probability proportional to size (PPS), and school contacting resulted in 1,221 eligible public, Catholic, and other private schools from a population of approximately 27,000 schools containing 10th grade students. Of the eligible schools, 752 participated in the study. In the second stage of sample selection, a sample of approximately 26 sophomores, from within each of the participating public and private schools was selected. Each school was asked to provide a list of 10th grade students, and quality assurance (QA) checks were performed on each list that was received.</p>
<h3>Usage</h3>
<pre>data</pre>
<h3>Format</h3>
<p>A data matrix with 9,679 rows and 17 columns, containing no missing values. The data are provided only for illustrative purposes and not for inference about education effectiveness, for which the original data source should be consulted.</p>
<dl>
<dt>SCH_ID:</dt>
<dd>
<p>School indicator.</p>
</dd>
<dt>fight:</dt>
<dd>
<p>Indicator variable for fight at school. 1 = fight.</p>
</dd>
<dt>attachment:</dt>
<dd>
<p>Indicator variable for attachment to school. 1 = like.</p>
</dd>
<dt>work:</dt>
<dd>
<p>Indicator variable for part-time job. 1 = work.</p>
</dd>
<dt>score:</dt>
<dd>
<p>Measure of math score.</p>
</dd>
<dt>late:</dt>
<dd>
<p>Frequency in which the student was late for school. 5 levels.</p>
</dd>
<dt>coed:</dt>
<dd>
<p>Indicator variable for coeducation. 1 = coeducation.</p>
</dd>
<dt>smorale:</dt>
<dd>
<p>Measure of student morale in the school. 4 levels.</p>
</dd>
<dt>gender:</dt>
<dd>
<p>Indicator variable for gender. 1 = female.</p>
</dd>
<dt>income:</dt>
<dd>
<p>Total family income. 13 levels.</p>
</dd>
<dt>free:</dt>
<dd>
<p>Percent of 10th grade students receiving free lunch. 1 to 7 levels.</p>
</dd>
<dt>pared:</dt>
<dd>
<p>Parents highest level of education. 8 levels</p>
</dd>
<dt>catholic:</dt>
<dd>
<p>Indicator variable for catholic school. 1 = catholic school.</p>
</dd>
</dl>
<h3>Source</h3>
<p>The complete student-level data is available from the data archives at <a href="http://www.icpsr.umich.edu/">www.icpsr.umich.edu/</a></p>
<h3>References</h3>
<p>United States Department of Education. National Center for Education Statistics</p>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-33722.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-33722.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-mediation-student.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-33722.json';</script>