---
title: R Dataset / Package datasets / swiss
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">swiss</span> data set which pertains to Swiss Fertility and Socioeconomic Indicators (1888) Data. The <span class="mono">swiss</span> data set is found in the <span class="mono">datasets</span> R package. You can load the <span class="mono">swiss</span> data set in R by issuing the following command at the console <span class="mono">data("swiss")</span>. This will load the data into a variable called <span class="mono">swiss</span>. If R says the <span class="mono">swiss</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("datasets")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-48809.csv">swiss R data set</a></span>. The size of this file is about 1,660 bytes.</p><h2>Swiss Fertility and Socioeconomic Indicators (1888) Data</h2>
<h3>Description</h3>
<p>Standardized fertility measure and socio-economic indicators for each of 47 French-speaking provinces of Switzerland at about 1888.</p>
<h3>Usage</h3>
<pre>swiss</pre>
<h3>Format</h3>
<p>A data frame with 47 observations on 6 variables, <em>each</em> of which is in percent, i.e., in <i>[0, 100]</i>.</p>
<table>
<caption>
R project statistics dataset table
</caption>
<tr>
<td style="text-align: right;">[,1]</td>
<td style="text-align: left;">Fertility</td>
<td style="text-align: left;"><i>Ig</i>, ‘common standardized fertility measure’</td>
</tr>
<tr>
<td style="text-align: right;">[,2]</td>
<td style="text-align: left;">Agriculture</td>
<td style="text-align: left;">% of males involved in agriculture as occupation</td>
</tr>
<tr>
<td style="text-align: right;">[,3]</td>
<td style="text-align: left;">Examination</td>
<td style="text-align: left;">% draftees receiving highest mark on army examination</td>
</tr>
<tr>
<td style="text-align: right;">[,4]</td>
<td style="text-align: left;">Education</td>
<td style="text-align: left;">% education beyond primary school for draftees.</td>
</tr>
<tr>
<td style="text-align: right;">[,5]</td>
<td style="text-align: left;">Catholic</td>
<td style="text-align: left;">% ‘catholic’ (as opposed to ‘protestant’).</td>
</tr>
<tr>
<td style="text-align: right;">[,6]</td>
<td style="text-align: left;">Infant.Mortality</td>
<td style="text-align: left;">live births who live less than 1 year.</td>
</tr>
</table>
<p>All variables but ‘Fertility’ give proportions of the population.</p>
<h3>Details</h3>
<p>(paraphrasing Mosteller and Tukey):</p>
<p>Switzerland, in 1888, was entering a period known as the <em>demographic transition</em>; i.e., its fertility was beginning to fall from the high level typical of underdeveloped countries.</p>
<p>The data collected are for 47 French-speaking “provinces” at about 1888.</p>
<p>Here, all variables are scaled to <i>[0, 100]</i>, where in the original, all but <code>"Catholic"</code> were scaled to <i>[0, 1]</i>.</p>
<h3>Note</h3>
<p>Files for all 182 districts in 1888 and other years have been available at <a href="https://opr.princeton.edu/archive/pefp/switz.aspx">https://opr.princeton.edu/archive/pefp/switz.aspx</a>.</p>
<p>They state that variables <code>Examination</code> and <code>Education</code> are averages for 1887, 1888 and 1889.</p>
<h3>Source</h3>
<p>Project “16P5”, pages 549–551 in</p>
<p>Mosteller, F. and Tukey, J. W. (1977) <em>Data Analysis and Regression: A Second Course in Statistics</em>. Addison-Wesley, Reading Mass.</p>
<p>indicating their source as “Data used by permission of Franice van de Walle. Office of Population Research, Princeton University, 1976. Unpublished data assembled under NICHD contract number No 1-HD-O-2077.”</p>
<h3>References</h3>
<p>Becker, R. A., Chambers, J. M. and Wilks, A. R. (1988) <em>The New S Language</em>. Wadsworth &amp; Brooks/Cole.</p>
<h3>Examples</h3>
<pre>
require(stats); require(graphics)
pairs(swiss, panel = panel.smooth, main = "swiss data",
col = 3 + (swiss$Catholic &gt; 50))
summary(lm(Fertility ~ . , data = swiss))
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-48809.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-48809.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-datasets-swiss.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-48809.json';</script>