---
title: R Dataset / Package Ecdat / DoctorContacts
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">DoctorContacts</span> data set which pertains to Contacts With Medical Doctor . The <span class="mono">DoctorContacts</span> data set is found in the <span class="mono">Ecdat</span> R package. You can load the <span class="mono">DoctorContacts</span> data set in R by issuing the following command at the console <span class="mono">data("DoctorContacts")</span>. This will load the data into a variable called <span class="mono">DoctorContacts</span>. If R says the <span class="mono">DoctorContacts</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("Ecdat")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-45713.csv">DoctorContacts R data set</a></span>. The size of this file is about 1,969,426 bytes.</p><h2>Contacts With Medical Doctor</h2>
<h3>Description</h3>
<p>a cross-section from 1977–1978</p>
<p><em>number of observations</em> : 20186</p>
<h3>Usage</h3>
<pre>data(DoctorContacts)</pre>
<h3>Format</h3>
<p>A time serie containing :</p>
<dl>
<dt>mdu</dt>
<dd>
<p>number of outpatient visits to a medical doctor</p>
</dd>
<dt>lc</dt>
<dd>
<p>log(coinsrate+1) where coinsurance rate is 0 to 100</p>
</dd>
<dt>idp</dt>
<dd>
<p>individual deductible plan ?</p>
</dd>
<dt>lpi</dt>
<dd>
<p>log(annual participation incentive payment) or 0 if no payment</p>
</dd>
<dt>fmde</dt>
<dd>
<p>log(max(medical deductible expenditure)) if IDP=1 and MDE&gt;1 or 0 otherw</p>
</dd>
<dt>physlim</dt>
<dd>
<p>physical limitation ?</p>
</dd>
<dt>ndisease</dt>
<dd>
<p>number of chronic diseases</p>
</dd>
<dt>health</dt>
<dd>
<p>self–rate health (excellent,good,fair,poor)</p>
</dd>
<dt>linc</dt>
<dd>
<p>log of annual family income (in \$)</p>
</dd>
<dt>lfam</dt>
<dd>
<p>log of family size</p>
</dd>
<dt>educdec</dt>
<dd>
<p>years of schooling of household head</p>
</dd>
<dt>age</dt>
<dd>
<p>exact age</p>
</dd>
<dt>sex</dt>
<dd>
<p>sex (male,female)</p>
</dd>
<dt>child</dt>
<dd>
<p>age less than 18 ?</p>
</dd>
<dt>black</dt>
<dd>
<p>is household head black ?</p>
</dd>
</dl>
<h3>Source</h3>
<p>Deb, P. and P.K. Trivedi (2002) “The Structure of Demand for Medical Care: Latent Class versus Two-Part Models”, <em>Journal of Health Economics</em>, <b>21</b>, 601–625.</p>
<h3>References</h3>
<p>Cameron, A.C. and P.K. Trivedi (2005) <em>Microeconometrics : methods and applications</em>, Cambridge, pp. 553–556 and 565.</p>
<h3>See Also</h3>
<p><code>Index.Source</code>, <code>Index.Economics</code>, <code>Index.Econometrics</code>, <code>Index.Observations</code>,</p>
<p><code>Index.Time.Series</code></p>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-45713.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-45713.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-ecdat-doctorcontacts.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-45713.json';</script>