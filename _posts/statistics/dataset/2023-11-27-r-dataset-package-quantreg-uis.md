---
title: R Dataset / Package quantreg / uis
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">uis</span> data set which pertains to UIS Drug Treatment study data. The <span class="mono">uis</span> data set is found in the <span class="mono">quantreg</span> R package. You can load the <span class="mono">uis</span> data set in R by issuing the following command at the console <span class="mono">data("uis")</span>. This will load the data into a variable called <span class="mono">uis</span>. If R says the <span class="mono">uis</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("quantreg")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-69014.csv">uis R data set</a></span>. The size of this file is about 62,061 bytes.</p><h2>UIS Drug Treatment study data</h2>
<h3>Description</h3>
<p>There are 628 data points in the original data, 575 of which have no missing values.</p>
<p>Variable descriptions:</p>
<table>
<caption>
R project statistics dataset table
</caption>
<tr>
<td style="text-align: left;">Variable</td>
<td style="text-align: left;">Description</td>
<td style="text-align: left;">Codes/Values</td>
</tr>
<tr>
<td style="text-align: left;">ID</td>
<td style="text-align: left;">Identification Code</td>
<td style="text-align: left;">1 - 628</td>
</tr>
<tr>
<td style="text-align: left;">AGE</td>
<td style="text-align: left;">Age at Enrollment</td>
<td style="text-align: left;">Years</td>
</tr>
<tr>
<td style="text-align: left;">BECK</td>
<td style="text-align: left;">Beck DepressionScore</td>
<td style="text-align: left;">0.000 - 54.000</td>
</tr>
<tr>
<td style="text-align: left;">HC</td>
<td style="text-align: left;">Heroin/Cocaine Use During</td>
<td style="text-align: left;">1 = Heroin &amp; Cocaine</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;">3 Months Prior to Admission</td>
<td style="text-align: left;">2 = Heroin Only</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
<td style="text-align: left;">3 = Cocaine Only</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
<td style="text-align: left;">4 = Neither Heroin nor Cocaine</td>
</tr>
<tr>
<td style="text-align: left;">IV</td>
<td style="text-align: left;">History of IV Drug Use</td>
<td style="text-align: left;">1 = Never</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
<td style="text-align: left;">2 = Previous</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
<td style="text-align: left;">3 = Recent</td>
</tr>
<tr>
<td style="text-align: left;">NDT</td>
<td style="text-align: left;">Number of Prior Drug Treatments</td>
<td style="text-align: left;">0 - 40</td>
</tr>
<tr>
<td style="text-align: left;">RACE</td>
<td style="text-align: left;">Subject's Race</td>
<td style="text-align: left;">0 = White</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
<td style="text-align: left;">1 = Non-White</td>
</tr>
<tr>
<td style="text-align: left;">TREAT</td>
<td style="text-align: left;">Treatment Randomization</td>
<td style="text-align: left;">0 = Short</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;">Assignment</td>
<td style="text-align: left;">1 = Long</td>
</tr>
<tr>
<td style="text-align: left;">SITE</td>
<td style="text-align: left;">Treatment Site</td>
<td style="text-align: left;">0 = A</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
<td style="text-align: left;">1 = B</td>
</tr>
<tr>
<td style="text-align: left;">LEN.T</td>
<td style="text-align: left;">Length of Stay in Treatment</td>
<td style="text-align: left;">Days</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;">(Admission Date to Exit Date)</td>
<td style="text-align: left;"></td>
</tr>
<tr>
<td style="text-align: left;">TIME</td>
<td style="text-align: left;">Time to Drug Relapse</td>
<td style="text-align: left;">Days</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;">(Measured from Admission Date)</td>
<td style="text-align: left;"></td>
</tr>
<tr>
<td style="text-align: left;">CENSOR</td>
<td style="text-align: left;">Event for Treating Lost to</td>
<td style="text-align: left;">1 = Returned to Drugs</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;">Follow-Up as Returned to Drugs</td>
<td style="text-align: left;">or Lost to Follow-Up</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
<td style="text-align: left;">0 = Otherwise</td>
</tr>
<tr>
<td style="text-align: left;">Y</td>
<td style="text-align: left;">log of TIME</td>
<td style="text-align: left;"></td>
</tr>
<tr>
<td style="text-align: left;">ND1</td>
<td style="text-align: left;">Component of NDT</td>
<td style="text-align: left;"></td>
</tr>
<tr>
<td style="text-align: left;">ND2</td>
<td style="text-align: left;">Component of NDT</td>
<td style="text-align: left;"></td>
</tr>
<tr>
<td style="text-align: left;">LNDT</td>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
</tr>
<tr>
<td style="text-align: left;">FRAC</td>
<td style="text-align: left;">Compliance fraction</td>
<td style="text-align: left;">LEN.T/90 for short trt</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
<td style="text-align: left;">LEN.T/180 for long trt</td>
</tr>
<tr>
<td style="text-align: left;">IV3</td>
<td style="text-align: left;">Recent IV use</td>
<td style="text-align: left;">1 = Yes</td>
</tr>
<tr>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
<td style="text-align: left;">0 = No</td>
</tr>
</table>
<h3>Usage</h3>
<pre>data(uis)</pre>
<h3>Format</h3>
<p>A data frame with dimension 575 by 18.</p>
<h3>Source</h3>
<p>Table 1.3 of Hosmer,D.W. and Lemeshow, S. (1998)</p>
<h3>References</h3>
<p>Hosmer,D.W. and Lemeshow, S. (1998) Applied Survival Analysis: Regression Modeling of Time to Event Data, John Wiley and Sons Inc., New York, NY</p>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-69014.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-69014.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-quantreg-uis.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-69014.json';</script>