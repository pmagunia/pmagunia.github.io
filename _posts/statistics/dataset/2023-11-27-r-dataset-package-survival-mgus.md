---
title: R Dataset / Package survival / mgus
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">mgus</span> data set which pertains to Monoclonal gammapothy data. The <span class="mono">mgus</span> data set is found in the <span class="mono">survival</span> R package. You can load the <span class="mono">mgus</span> data set in R by issuing the following command at the console <span class="mono">data("mgus")</span>. This will load the data into a variable called <span class="mono">mgus</span>. If R says the <span class="mono">mgus</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("survival")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-62816.csv">mgus R data set</a></span>. The size of this file is about 11,493 bytes.</p><h2>Monoclonal gammapothy data</h2>
<h3>Description</h3>
<p>Natural history of 241 subjects with monoclonal gammapothy of undetermined significance (MGUS).</p>
<h3>Usage</h3>
<pre>
mgus
mgus1
</pre>
<h3>Format</h3>
<p>mgus: A data frame with 241 observations on the following 12 variables.</p>
<table>
<caption>
R project statistics dataset table
</caption>
<tr>
<td style="text-align: left;">id:</td>
<td style="text-align: left;">subject id</td>
</tr>
<tr>
<td style="text-align: left;">age:</td>
<td style="text-align: left;">age in years at the detection of MGUS</td>
</tr>
<tr>
<td style="text-align: left;">sex:</td>
<td style="text-align: left;"><code>male</code> or <code>female</code></td>
</tr>
<tr>
<td style="text-align: left;">dxyr:</td>
<td style="text-align: left;">year of diagnosis</td>
</tr>
<tr>
<td style="text-align: left;">pcdx:</td>
<td style="text-align: left;">for subjects who progress to a plasma cell malignancy</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;">the subtype of malignancy: multiple myeloma (MM) is the</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;">most common, followed by amyloidosis (AM), macroglobulinemia (MA),</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;">and other lymphprolifative disorders (LP)</td>
</tr>
<tr>
<td style="text-align: left;">pctime:</td>
<td style="text-align: left;">days from MGUS until diagnosis of a plasma cell malignancy</td>
</tr>
<tr>
<td style="text-align: left;">futime:</td>
<td style="text-align: left;">days from diagnosis to last follow-up</td>
</tr>
<tr>
<td style="text-align: left;">death:</td>
<td style="text-align: left;">1= follow-up is until death</td>
</tr>
<tr>
<td style="text-align: left;">alb:</td>
<td style="text-align: left;">albumin level at MGUS diagnosis</td>
</tr>
<tr>
<td style="text-align: left;">creat:</td>
<td style="text-align: left;">creatinine at MGUS diagnosis</td>
</tr>
<tr>
<td style="text-align: left;">hgb:</td>
<td style="text-align: left;">hemoglobin at MGUS diagnosis</td>
</tr>
<tr>
<td style="text-align: left;">mspike:</td>
<td style="text-align: left;">size of the monoclonal protein spike at diagnosis</td>
</tr>
<tr>
<td style="text-align: left;"></td>
</tr>
</table>
<p>mgus1: The same data set in start,stop format. Contains the id, age, sex, and laboratory variable described above along with</p>
<table>
<caption>
R project statistics dataset table
</caption>
<tr>
<td style="text-align: left;">start, stop:</td>
<td style="text-align: left;">sequential intervals of time for each subject</td>
</tr>
<tr>
<td style="text-align: left;">status:</td>
<td style="text-align: left;">=1 if the interval ends in an event</td>
</tr>
<tr>
<td style="text-align: left;">event:</td>
<td style="text-align: left;">a factor containing the event type: censor, death, or plasma cell malignancy</td>
</tr>
<tr>
<td style="text-align: left;">enum:</td>
<td style="text-align: left;">event number for each subject: 1 or 2</td>
</tr>
</table>
<h3>Details</h3>
<p>Plasma cells are responsible for manufacturing immunoglobulins, an important part of the immune defense. At any given time there are estimated to be about <i>10^6</i> different immunoglobulins in the circulation at any one time. When a patient has a plasma cell malignancy the distribution will become dominated by a single isotype, the product of the malignant clone, visible as a spike on a serum protein electrophoresis. Monoclonal gammapothy of undertermined significance (MGUS) is the presence of such a spike, but in a patient with no evidence of overt malignancy. This data set of 241 sequential subjects at Mayo Clinic was the groundbreaking study defining the natural history of such subjects. Due to the diligence of the principle investigator 0 subjects have been lost to follow-up.</p>
<p>Three subjects had MGUS detected on the day of death. In data set <code>mgus1</code> these subjects have the time to MGUS coded as .5 day before the death in order to avoid tied times.</p>
<p>These data sets were updated in Jan 2015 to correct some small errors.</p>
<h3>Source</h3>
<p>Mayo Clinic data courtesy of Dr. Robert Kyle.</p>
<h3>References</h3>
<p>R Kyle, Benign monoclonal gammopathy – after 20 to 35 years of follow-up, Mayo Clinic Proc 1993; 68:26-36.</p>
<h3>Examples</h3>
<pre>
# Create the competing risk curves for time to first of death or PCM
sfit &lt;- survfit(Surv(start, stop, event) ~ sex, mgus1, subset=(enum==1))
print(sfit)# the order of printout is the order in which they plotplot(sfit, xscale=365.25, lty=c(2,1,2,1), col=c(1,1,2,2),
 xlab="Years after MGUS detection", ylab="Proportion")
legend(0, .8, c("Death/male", "Death/female", "PCM/male", "PCM/female"),
 lty=c(1,1,2,2), col=c(2,1,2,1), bty='n')title("Curves for the first of plasma cell malignancy or death")
# The plot shows that males have a higher death rate than females (no
# surprise) but their rates of conversion to PCM are essentially the same.
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-62816.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-62816.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-survival-mgus.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-62816.json';</script>