---
title: R Dataset / Package MASS / Cars93
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">Cars93</span> data set which pertains to Data from 93 Cars on Sale in the USA in 1993. The <span class="mono">Cars93</span> data set is found in the <span class="mono">MASS</span> R package. You can load the <span class="mono">Cars93</span> data set in R by issuing the following command at the console <span class="mono">data("Cars93")</span>. This will load the data into a variable called <span class="mono">Cars93</span>. If R says the <span class="mono">Cars93</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("MASS")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-83422.csv">Cars93 R data set</a></span>. The size of this file is about 14,411 bytes.</p><h2>Data from 93 Cars on Sale in the USA in 1993</h2>
<h3>Description</h3>
<p>The <code>Cars93</code> data frame has 93 rows and 27 columns.</p>
<h3>Usage</h3>
<pre>
Cars93
</pre>
<h3>Format</h3>
<p>This data frame contains the following columns:</p>
<dl>
<dt><code>Manufacturer</code></dt>
<dd>
<p>Manufacturer.</p>
</dd>
<dt><code>Model</code></dt>
<dd>
<p>Model.</p>
</dd>
<dt><code>Type</code></dt>
<dd>
<p>Type: a factor with levels <code>"Small"</code>, <code>"Sporty"</code>, <code>"Compact"</code>, <code>"Midsize"</code>, <code>"Large"</code> and <code>"Van"</code>.</p>
</dd>
<dt><code>Min.Price</code></dt>
<dd>
<p>Minimum Price (in \$1,000): price for a basic version.</p>
</dd>
<dt><code>Price</code></dt>
<dd>
<p>Midrange Price (in \$1,000): average of <code>Min.Price</code> and <code>Max.Price</code>.</p>
</dd>
<dt><code>Max.Price</code></dt>
<dd>
<p>Maximum Price (in \$1,000): price for “a premium version”.</p>
</dd>
<dt><code>MPG.city</code></dt>
<dd>
<p>City MPG (miles per US gallon by EPA rating).</p>
</dd>
<dt><code>MPG.highway</code></dt>
<dd>
<p>Highway MPG.</p>
</dd>
<dt><code>AirBags</code></dt>
<dd>
<p>Air Bags standard. Factor: none, driver only, or driver &amp; passenger.</p>
</dd>
<dt><code>DriveTrain</code></dt>
<dd>
<p>Drive train type: rear wheel, front wheel or 4WD; (factor).</p>
</dd>
<dt><code>Cylinders</code></dt>
<dd>
<p>Number of cylinders (missing for Mazda RX-7, which has a rotary engine).</p>
</dd>
<dt><code>EngineSize</code></dt>
<dd>
<p>Engine size (litres).</p>
</dd>
<dt><code>Horsepower</code></dt>
<dd>
<p>Horsepower (maximum).</p>
</dd>
<dt><code>RPM</code></dt>
<dd>
<p>RPM (revs per minute at maximum horsepower).</p>
</dd>
<dt><code>Rev.per.mile</code></dt>
<dd>
<p>Engine revolutions per mile (in highest gear).</p>
</dd>
<dt><code>Man.trans.avail</code></dt>
<dd>
<p>Is a manual transmission version available? (yes or no, Factor).</p>
</dd>
<dt><code>Fuel.tank.capacity</code></dt>
<dd>
<p>Fuel tank capacity (US gallons).</p>
</dd>
<dt><code>Passengers</code></dt>
<dd>
<p>Passenger capacity (persons)</p>
</dd>
<dt><code>Length</code></dt>
<dd>
<p>Length (inches).</p>
</dd>
<dt><code>Wheelbase</code></dt>
<dd>
<p>Wheelbase (inches).</p>
</dd>
<dt><code>Width</code></dt>
<dd>
<p>Width (inches).</p>
</dd>
<dt><code>Turn.circle</code></dt>
<dd>
<p>U-turn space (feet).</p>
</dd>
<dt><code>Rear.seat.room</code></dt>
<dd>
<p>Rear seat room (inches) (missing for 2-seater vehicles).</p>
</dd>
<dt><code>Luggage.room</code></dt>
<dd>
<p>Luggage capacity (cubic feet) (missing for vans).</p>
</dd>
<dt><code>Weight</code></dt>
<dd>
<p>Weight (pounds).</p>
</dd>
<dt><code>Origin</code></dt>
<dd>
<p>Of non-USA or USA company origins? (factor).</p>
</dd>
<dt><code>Make</code></dt>
<dd>
<p>Combination of Manufacturer and Model (character).</p>
</dd>
</dl>
<h3>Details</h3>
<p>Cars were selected at random from among 1993 passenger car models that were listed in both the <em>Consumer Reports</em> issue and the <em>PACE Buying Guide</em>. Pickup trucks and Sport/Utility vehicles were eliminated due to incomplete information in the <em>Consumer Reports</em> source. Duplicate models (e.g., Dodge Shadow and Plymouth Sundance) were listed at most once.</p>
<p>Further description can be found in Lock (1993).</p>
<h3>Source</h3>
<p>Lock, R. H. (1993) 1993 New Car Data. <em>Journal of Statistics Education</em> <b>1</b>(1). <a href="http://www.amstat.org/publications/jse/v1n1/datasets.lock.html">http://www.amstat.org/publications/jse/v1n1/datasets.lock.html</a>.</p>
<h3>References</h3>
<p>Venables, W. N. and Ripley, B. D. (1999) <em>Modern Applied Statistics with S-PLUS.</em> Third Edition. Springer.</p>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-83422.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-83422.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-mass-cars93.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-83422.json';</script>