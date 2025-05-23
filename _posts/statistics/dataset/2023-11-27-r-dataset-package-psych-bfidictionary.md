---
title: R Dataset / Package psych / bfi.dictionary
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">bfi.dictionary</span> data set which pertains to 25 Personality items representing 5 factors. The <span class="mono">bfi.dictionary</span> data set is found in the <span class="mono">psych</span> R package. You can load the <span class="mono">bfi.dictionary</span> data set in R by issuing the following command at the console <span class="mono">data("bfi.dictionary")</span>. This will load the data into a variable called <span class="mono">bfi.dictionary</span>. If R says the <span class="mono">bfi.dictionary</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("psych")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-37624.csv">bfi.dictionary R data set</a></span>. The size of this file is about 2,532 bytes.</p><h2>25 Personality items representing 5 factors</h2>
<h3>Description</h3>
<p>25 personality self report items taken from the International Personality Item Pool (ipip.ori.org) were included as part of the Synthetic Aperture Personality Assessment (SAPA) web based personality assessment project. The data from 2800 subjects are included here as a demonstration set for scale construction, factor analysis, and Item Response Theory analysis. Three additional demographic variables (sex, education, and age) are also included.</p>
<h3>Usage</h3>
<pre>data(bfi)
data(bfi.dictionary)
</pre>
<h3>Format</h3>
<p>A data frame with 2800 observations on the following 28 variables. (The q numbers are the SAPA item numbers).</p>
<dl>
<dt><code>A1</code></dt>
<dd>
<p>Am indifferent to the feelings of others. (q_146)</p>
</dd>
<dt><code>A2</code></dt>
<dd>
<p>Inquire about others' well-being. (q_1162)</p>
</dd>
<dt><code>A3</code></dt>
<dd>
<p>Know how to comfort others. (q_1206)</p>
</dd>
<dt><code>A4</code></dt>
<dd>
<p>Love children. (q_1364)</p>
</dd>
<dt><code>A5</code></dt>
<dd>
<p>Make people feel at ease. (q_1419)</p>
</dd>
<dt><code>C1</code></dt>
<dd>
<p>Am exacting in my work. (q_124)</p>
</dd>
<dt><code>C2</code></dt>
<dd>
<p>Continue until everything is perfect. (q_530)</p>
</dd>
<dt><code>C3</code></dt>
<dd>
<p>Do things according to a plan. (q_619)</p>
</dd>
<dt><code>C4</code></dt>
<dd>
<p>Do things in a half-way manner. (q_626)</p>
</dd>
<dt><code>C5</code></dt>
<dd>
<p>Waste my time. (q_1949)</p>
</dd>
<dt><code>E1</code></dt>
<dd>
<p>Don't talk a lot. (q_712)</p>
</dd>
<dt><code>E2</code></dt>
<dd>
<p>Find it difficult to approach others. (q_901)</p>
</dd>
<dt><code>E3</code></dt>
<dd>
<p>Know how to captivate people. (q_1205)</p>
</dd>
<dt><code>E4</code></dt>
<dd>
<p>Make friends easily. (q_1410)</p>
</dd>
<dt><code>E5</code></dt>
<dd>
<p>Take charge. (q_1768)</p>
</dd>
<dt><code>N1</code></dt>
<dd>
<p>Get angry easily. (q_952)</p>
</dd>
<dt><code>N2</code></dt>
<dd>
<p>Get irritated easily. (q_974)</p>
</dd>
<dt><code>N3</code></dt>
<dd>
<p>Have frequent mood swings. (q_1099</p>
</dd>
<dt><code>N4</code></dt>
<dd>
<p>Often feel blue. (q_1479)</p>
</dd>
<dt><code>N5</code></dt>
<dd>
<p>Panic easily. (q_1505)</p>
</dd>
<dt><code>O1</code></dt>
<dd>
<p>Am full of ideas. (q_128)</p>
</dd>
<dt><code>O2</code></dt>
<dd>
<p>Avoid difficult reading material.(q_316)</p>
</dd>
<dt><code>O3</code></dt>
<dd>
<p>Carry the conversation to a higher level. (q_492)</p>
</dd>
<dt><code>O4</code></dt>
<dd>
<p>Spend time reflecting on things. (q_1738)</p>
</dd>
<dt><code>O5</code></dt>
<dd>
<p>Will not probe deeply into a subject. (q_1964)</p>
</dd>
<dt><code>gender</code></dt>
<dd>
<p>Males = 1, Females =2</p>
</dd>
<dt><code>education</code></dt>
<dd>
<p>1 = HS, 2 = finished HS, 3 = some college, 4 = college graduate 5 = graduate degree</p>
</dd>
<dt><code>age</code></dt>
<dd>
<p>age in years</p>
</dd>
</dl>
<h3>Details</h3>
<p>The first 25 items are organized by five putative factors: Agreeableness, Conscientiousness, Extraversion, Neuroticism, and Opennness. The scoring key is created using <code>make.keys</code>, the scores are found using <code>score.items</code>.</p>
<p>These five factors are a useful example of using <code>irt.fa</code> to do Item Response Theory based latent factor analysis of the <code>polychoric</code> correlation matrix. The endorsement plots for each item, as well as the item information functions reveal that the items differ in their quality.</p>
<p>The item data were collected using a 6 point response scale: 1 Very Inaccurate 2 Moderately Inaccurate 3 Slightly Inaccurate 4 Slightly Accurate 5 Moderately Accurate 6 Very Accurate</p>
<p>as part of the Synthetic Apeture Personality Assessment (SAPA <a href="http://sapa-project.org">http://sapa-project.org</a>) project. To see an example of the data collection technique, visit <a href="http://SAPA-project.org">http://SAPA-project.org</a>. The items given were sampled from the International Personality Item Pool of Lewis Goldberg using the sampling technique of SAPA. This is a sample data set taken from the much larger SAPA data bank.</p>
<h3>Note</h3>
<p>The bfi data set and items should not be confused with the BFI (Big Five Inventory) of Oliver John and colleagues (John, O. P., Donahue, E. M., &amp; Kentle, R. L. (1991). The Big Five Inventory–Versions 4a and 54. Berkeley, CA: University of California,Berkeley, Institute of Personality and Social Research.)</p>
<h3>Source</h3>
<p>The items are from the ipip (Goldberg, 1999). The data are from the SAPA project (Revelle, Wilt and Rosenthal, 2010) , collected Spring, 2010 ( <a href="http://sapa-project.org">http://sapa-project.org</a>).</p>
<h3>References</h3>
<p>Goldberg, L.R. (1999) A broad-bandwidth, public domain, personality inventory measuring the lower-level facets of several five-factor models. In Mervielde, I. and Deary, I. and De Fruyt, F. and Ostendorf, F. (eds) Personality psychology in Europe. 7. Tilburg University Press. Tilburg, The Netherlands.</p>
<p>Revelle, W., Wilt, J., and Rosenthal, A. (2010) Individual Differences in Cognition: New Methods for examining the Personality-Cognition Link In Gruszka, A. and Matthews, G. and Szymura, B. (Eds.) Handbook of Individual Differences in Cognition: Attention, Memory and Executive Control, Springer.</p>
<h3>See Also</h3>
<p><code>bi.bars</code> to show the data by age and gender, <code>irt.fa</code> for item factor analysis applying the irt model.</p>
<h3>Examples</h3>
<pre>
data(bfi)
describe(bfi)
 
 keys.list &lt;-
list(agree=c("-A1","A2","A3","A4","A5"),conscientious=c("C1","C2","C3","-C4","-C5"),
extraversion=c("-E1","-E2","E3","E4","E5"),neuroticism=c("N1","N2","N3","N4","N5"),
openness = c("O1","-O2","O3","O4","-O5")) 
 scores &lt;- scoreItems(keys.list,bfi,min=1,max=6) #specify the minimum and maximum values
 scores
 #show the use of the fa.lookup with a dictionary
 keys.lookup(keys.list,bfi.dictionary[,1:4])
 
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-37624.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-37624.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-psych-bfidictionary.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-37624.json';</script>