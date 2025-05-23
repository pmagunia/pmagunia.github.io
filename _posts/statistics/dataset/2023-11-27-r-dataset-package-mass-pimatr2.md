---
title: R Dataset / Package MASS / Pima.tr2
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">Pima.tr2</span> data set which pertains to Diabetes in Pima Indian Women. The <span class="mono">Pima.tr2</span> data set is found in the <span class="mono">MASS</span> R package. You can load the <span class="mono">Pima.tr2</span> data set in R by issuing the following command at the console <span class="mono">data("Pima.tr2")</span>. This will load the data into a variable called <span class="mono">Pima.tr2</span>. If R says the <span class="mono">Pima.tr2</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("MASS")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-16928.csv">Pima.tr2 R data set</a></span>. The size of this file is about 9,332 bytes.</p><h2>Diabetes in Pima Indian Women</h2>
<h3>Description</h3>
<p>A population of women who were at least 21 years old, of Pima Indian heritage and living near Phoenix, Arizona, was tested for diabetes according to World Health Organization criteria. The data were collected by the US National Institute of Diabetes and Digestive and Kidney Diseases. We used the 532 complete records after dropping the (mainly missing) data on serum insulin.</p>
<h3>Usage</h3>
<pre>
Pima.tr
Pima.tr2
Pima.te
</pre>
<h3>Format</h3>
<p>These data frames contains the following columns:</p>
<dl>
<dt><code>npreg</code></dt>
<dd>
<p>number of pregnancies.</p>
</dd>
<dt><code>glu</code></dt>
<dd>
<p>plasma glucose concentration in an oral glucose tolerance test.</p>
</dd>
<dt><code>bp</code></dt>
<dd>
<p>diastolic blood pressure (mm Hg).</p>
</dd>
<dt><code>skin</code></dt>
<dd>
<p>triceps skin fold thickness (mm).</p>
</dd>
<dt><code>bmi</code></dt>
<dd>
<p>body mass index (weight in kg/(height in m)<i>\^2</i>).</p>
</dd>
<dt><code>ped</code></dt>
<dd>
<p>diabetes pedigree function.</p>
</dd>
<dt><code>age</code></dt>
<dd>
<p>age in years.</p>
</dd>
<dt><code>type</code></dt>
<dd>
<p><code>Yes</code> or <code>No</code>, for diabetic according to WHO criteria.</p>
</dd>
</dl>
<h3>Details</h3>
<p>The training set <code>Pima.tr</code> contains a randomly selected set of 200 subjects, and <code>Pima.te</code> contains the remaining 332 subjects. <code>Pima.tr2</code> contains <code>Pima.tr</code> plus 100 subjects with missing values in the explanatory variables.</p>
<h3>Source</h3>
<p>Smith, J. W., Everhart, J. E., Dickson, W. C., Knowler, W. C. and Johannes, R. S. (1988) Using the ADAP learning algorithm to forecast the onset of <em>diabetes mellitus</em>. In <em>Proceedings of the Symposium on Computer Applications in Medical Care (Washington, 1988),</em> ed. R. A. Greenes, pp. 261–265. Los Alamitos, CA: IEEE Computer Society Press.</p>
<p>Ripley, B.D. (1996) <em>Pattern Recognition and Neural Networks.</em> Cambridge: Cambridge University Press.</p>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-16928.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-16928.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-mass-pimatr2.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-16928.json';</script>