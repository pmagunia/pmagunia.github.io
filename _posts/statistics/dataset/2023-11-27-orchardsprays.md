---
title: OrchardSprays
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<h2>Potency of Orchard Sprays</h2>
<p>An experiment was conducted to assess the potency of various constituents of orchard sprays in repelling honeybees, using a Latin square design.</p>
<h3>Usage</h3>
<pre>OrchardSprays</pre>
<h3>Format</h3>
<p>A data frame with 64 observations on 4 variables.</p>
<table>
<caption>
R project statistics dataset table
</caption>
<tr>
<td style="text-align: right;">[,1]</td>
<td style="text-align: left;">rowpos</td>
<td style="text-align: left;">numeric</td>
<td style="text-align: left;">Row of the design</td>
</tr>
<tr>
<td style="text-align: right;">[,2]</td>
<td style="text-align: left;">colpos</td>
<td style="text-align: left;">numeric</td>
<td style="text-align: left;">Column of the design</td>
</tr>
<tr>
<td style="text-align: right;">[,3]</td>
<td style="text-align: left;">treatment</td>
<td style="text-align: left;">factor</td>
<td style="text-align: left;">Treatment level</td>
</tr>
<tr>
<td style="text-align: right;">[,4]</td>
<td style="text-align: left;">decrease</td>
<td style="text-align: left;">numeric</td>
<td style="text-align: left;">Response</td>
</tr>
</table>
<h3>Details</h3>
<p>Individual cells of dry comb were filled with measured amounts of lime sulphur emulsion in sucrose solution. Seven different concentrations of lime sulphur ranging from a concentration of 1/100 to 1/1,562,500 in successive factors of 1/5 were used as well as a solution containing no lime sulphur.</p>
<p>The responses for the different solutions were obtained by releasing 100 bees into the chamber for two hours, and then measuring the decrease in volume of the solutions in the various cells.</p>
<p>An <i>8 x 8</i> Latin square design was used and the treatments were coded as follows:</p>
<table>
<caption>
R project statistics dataset table
</caption>
<tr>
<td style="text-align: right;">A</td>
<td style="text-align: left;">highest level of lime sulphur</td>
</tr>
<tr>
<td style="text-align: right;">B</td>
<td style="text-align: left;">next highest level of lime sulphur</td>
</tr>
<tr>
<td style="text-align: right;">.</td>
<td style="text-align: left;"></td>
</tr>
<tr>
<td style="text-align: right;">.</td>
<td style="text-align: left;"></td>
</tr>
<tr>
<td style="text-align: right;">.</td>
<td style="text-align: left;"></td>
</tr>
<tr>
<td style="text-align: right;">G</td>
<td style="text-align: left;">lowest level of lime sulphur</td>
</tr>
<tr>
<td style="text-align: right;">H</td>
<td style="text-align: left;">no lime sulphur</td>
</tr>
</table>
<h3>Source</h3>
<p>Finney, D. J. (1947) <em>Probit Analysis</em>. Cambridge.</p>
<h3>References</h3>
<p>McNeil, D. R. (1977) <em>Interactive Data Analysis</em>. New York: Wiley.</p>
<h3>Examples</h3>
<pre>
require(graphics)
pairs(OrchardSprays, main = "OrchardSprays data")
</pre></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-66683.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-66683.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/orchardsprays.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-66683.json';</script>