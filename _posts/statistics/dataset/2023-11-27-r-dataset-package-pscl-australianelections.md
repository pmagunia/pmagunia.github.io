---
title: R Dataset / Package pscl / AustralianElections
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">AustralianElections</span> data set which pertains to elections to Australian House ofRepresentatives, 1949-2007. The <span class="mono">AustralianElections</span> data set is found in the <span class="mono">pscl</span> R package. You can load the <span class="mono">AustralianElections</span> data set in R by issuing the following command at the console <span class="mono">data("AustralianElections")</span>. This will load the data into a variable called <span class="mono">AustralianElections</span>. If R says the <span class="mono">AustralianElections</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("pscl")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-10270.csv">AustralianElections R data set</a></span>. The size of this file is about 2,030 bytes.</p><h2>elections to Australian House of Representatives, 1949-2007</h2>
<h3>Description</h3>
<p>Aggregate data on the 24 elections to Australia's House of Representatives, 1949 to 2007.</p>
<h3>Usage</h3>
<pre>data(AustralianElections)</pre>
<h3>Format</h3>
<p>A data frame with the following variables:</p>
<dl>
<dt><code>date</code></dt>
<dd>
<p>date of election, stored using the <code>Date</code> class</p>
</dd>
<dt><code>Seats</code></dt>
<dd>
<p>numeric, number of seats in the House of Representatives</p>
</dd>
<dt><code>Uncontested</code></dt>
<dd>
<p>numeric, number of uncontested seats</p>
</dd>
<dt><code>ALPSeats</code></dt>
<dd>
<p>numeric, number of seats won by the Australian Labor Party</p>
</dd>
<dt><code>LPSeats</code></dt>
<dd>
<p>numeric, number of seats won by the Liberal Party</p>
</dd>
<dt><code>NPSeats</code></dt>
<dd>
<p>numeric, number of seats won by the National Party (previously known as the Country Party)</p>
</dd>
<dt><code>OtherSeats</code></dt>
<dd>
<p>numeric, number of seats won by other parties and/or independent candidates</p>
</dd>
<dt><code>ALP</code></dt>
<dd>
<p>numeric, percentage of first preference votes cast for Australian Labor Party candidates</p>
</dd>
<dt><code>ALP2PP</code></dt>
<dd>
<p>numeric, percentage of the two-party preferred vote won by Australian Labor Party candidates</p>
</dd>
<dt><code>LP</code></dt>
<dd>
<p>numeric, percent of first preference votes cast for Liberal Party candidates</p>
</dd>
<dt><code>NP</code></dt>
<dd>
<p>numeric, percent of first preference votes cast for National Party (Country Party) candidates</p>
</dd>
<dt><code>DLP</code></dt>
<dd>
<p>numeric, percent of first preference votes cast for Democratic Labor Party candidates</p>
</dd>
<dt><code>Dem</code></dt>
<dd>
<p>numeric, percent of first preference votes cast for Australian Democrat candidates</p>
</dd>
<dt><code>Green</code></dt>
<dd>
<p>numeric, percent of first preference votes cast for Green Party candidates</p>
</dd>
<dt><code>Hanson</code></dt>
<dd>
<p>numeric, percent of first preference votes cast for candidates from Pauline Hanson's One Nation party</p>
</dd>
<dt><code>Com</code></dt>
<dd>
<p>numeric, percent of first preference votes cast for Communist Party candidates</p>
</dd>
<dt><code>AP</code></dt>
<dd>
<p>numeric, percent of first preference votes cast for Australia Party candidates</p>
</dd>
<dt><code>Informal</code></dt>
<dd>
<p>numeric, percent of ballots cast that are spoiled, blank, or otherwise uncountable (usually because of errors in enumerating preferences)</p>
</dd>
<dt><code>Turnout</code></dt>
<dd>
<p>numeric, percent of enrolled voters recorded as having turned out to vote (Australia has compulsory voting)</p>
</dd>
</dl>
<h3>Source</h3>
<p>Australian Electoral Commission. <a href="http://www.aec.gov.au">http://www.aec.gov.au</a>.</p>
<h3>References</h3>
<p>Jackman, Simon. 2009. <em>Bayesian Analysis for the Social Sciences</em>. Wiley: Hoboken, New Jersey. Example 3.5.</p>
<h3>Examples</h3>
<pre>
data(AustralianElections)
attach(AustralianElections)
alpSeatShare &lt;- ALPSeats/Seats
alpVoteShare &lt;- ALP2PP/100## log-odds transforms
x &lt;- log(alpVoteShare/(1-alpVoteShare))
y &lt;- log(alpSeatShare/(1-alpSeatShare))ols &lt;- lm(y~x) ## Tufte-style seats-votes regressionxseq &lt;- seq(-4.5,4.5,length=500)
yhat &lt;- coef(ols)[1] + coef(ols)[2]*xseq
yhat &lt;- exp(yhat)/(1+exp(yhat))
xseq &lt;- exp(xseq)/(1+exp(xseq))## seats vote curve
plot(x=alpVoteShare,
 y=alpSeatShare,
 xlab="ALP Vote Share",
 ylab="ALP Seat Share")
lines(xseq,yhat,lwd=2)
abline(h=.5,lty=2)
abline(v=.5,lty=2)
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-10270.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-10270.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-pscl-australianelections.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-10270.json';</script>