---
title: R Dataset / Package mediation / jobs
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">jobs</span> data set which pertains to JOBS II data. The <span class="mono">jobs</span> data set is found in the <span class="mono">mediation</span> R package. You can load the <span class="mono">jobs</span> data set in R by issuing the following command at the console <span class="mono">data("jobs")</span>. This will load the data into a variable called <span class="mono">jobs</span>. If R says the <span class="mono">jobs</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("mediation")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-15363.csv">jobs R data set</a></span>. The size of this file is about 136,796 bytes.</p><h2>JOBS II data</h2>
<h3>Description</h3>
<p>Job Search Intervention Study (JOBS II). JOBS II is a randomized field experiment that investigates the efficacy of a job training intervention on unemployed workers. The program is designed to not only increase reemployment among the unemployed but also enhance the mental health of the job seekers. In the JOBS II field experiment, 1,801 unemployed workers received a pre-screening questionnaire and were then randomly assigned to treatment and control groups. Those in the treatment group participated in job-skills workshops. In the workshops, respondents learned job-search skills and coping strategies for dealing with setbacks in the job-search process. Those in the control condition received a booklet describing job-search tips. In follow-up interviews, the two key outcome variables were measured; a continuous measure of depressive symptoms based on the Hopkins Symptom Checklist, and a binary variable, representing whether the respondent had become employed.</p>
<h3>Usage</h3>
<pre>data</pre>
<h3>Format</h3>
<p>A data matrix with 899 rows and 17 columns, containing no missing values. The data are provided only for illustrative purposes and not for inference about program efficacy, for which the original data source should be consulted.</p>
<dl>
<dt>econ_hard:</dt>
<dd>
<p>Level of economic hardship pre-treatment with values from 1 to 5.</p>
</dd>
<dt>depress1:</dt>
<dd>
<p>Measure of depressive symptoms pre-treatment.</p>
</dd>
<dt>sex:</dt>
<dd>
<p>Indicator variable for sex. 1 = female</p>
</dd>
<dt>age:</dt>
<dd>
<p>Age in years.</p>
</dd>
<dt>occp:</dt>
<dd>
<p>Factor with seven categories for various occupations.</p>
</dd>
<dt>marital:</dt>
<dd>
<p>Factor with five categories for marital status.</p>
</dd>
<dt>nonwhite:</dt>
<dd>
<p>Indicator variable for race. 1 = nonwhite.</p>
</dd>
<dt>educ:</dt>
<dd>
<p>Factor with five categories for educational attainment.</p>
</dd>
<dt>income:</dt>
<dd>
<p>Factor with five categories for level of income.</p>
</dd>
<dt>job_seek:</dt>
<dd>
<p>A continuous scale measuring the level of job-search self-efficacy with values from 1 to 5. The mediator variable.</p>
</dd>
<dt>depress2:</dt>
<dd>
<p>Measure of depressive symptoms post-treatment.</p>
</dd>
<dt>work1:</dt>
<dd>
<p>Indicator variable for employment. 1 = employed.</p>
</dd>
<dt>job_dich:</dt>
<dd>
<p>The job_seek measure recoded into two categories of high and low. 1 = high job search self-efficacy.</p>
</dd>
<dt>job_disc:</dt>
<dd>
<p>The job_seek measure recoded into four categories from lowest to highest.</p>
</dd>
<dt>treat:</dt>
<dd>
<p>Indicator variable for whether participant was randomly selected for the JOBS II training program. 1 = assignment to participation.</p>
</dd>
<dt>comply:</dt>
<dd>
<p>Indicator variable for whether participant actually participated in the JOBS II program. 1 = participation.</p>
</dd>
<dt>control:</dt>
<dd>
<p>Indicator variable for whether participant was randomly selected to not participate in the JOBS II training program. 1 = non-participation.</p>
</dd>
</dl>
<h3>Source</h3>
<p>The complete JOBS II data is available from the data archives at <a href="http://www.icpsr.umich.edu/">www.icpsr.umich.edu/</a></p>
<h3>References</h3>
<p>Vinokur, A. and Schul, Y. (1997). Mastery and inoculation against setbacks as active ingredients in the jobs intervention for the unemployed. Journal of Consulting and Clinical Psychology 65, 5.</p>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-15363.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-15363.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-mediation-jobs.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-15363.json';</script>