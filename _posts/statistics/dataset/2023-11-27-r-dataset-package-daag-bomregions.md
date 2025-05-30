---
title: R Dataset / Package DAAG / bomregions
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">bomregions</span> data set which pertains to Australian and Related Historical Annual Climate Data, by region. The <span class="mono">bomregions</span> data set is found in the <span class="mono">DAAG</span> R package. You can load the <span class="mono">bomregions</span> data set in R by issuing the following command at the console <span class="mono">data("bomregions")</span>. This will load the data into a variable called <span class="mono">bomregions</span>. If R says the <span class="mono">bomregions</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("DAAG")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-12938.csv">bomregions R data set</a></span>. The size of this file is about 15,817 bytes.</p><h2>Australian and Related Historical Annual Climate Data, by region</h2>
<h3>Description</h3>
<p>Australian regional temperature data, Australian regional rainfall data, and Annual SOI, are given for the years 1900-2008 or 1900-2011 or 1900-2012. The regional rainfall and temperature data are area-weighted averages for the respective regions. The Southern Oscillation Index (SOI) is the difference in barometric pressure at sea level between Tahiti and Darwin.</p>
<h3>Usage</h3>
<pre>bomregions</pre>
<h3>Format</h3>
<p>This data frame contains the following columns:</p>
<dl>
<dt>Year</dt>
<dd>
<p>Year</p>
</dd>
<dt>eastAVt</dt>
<dd>
<p>Eastern temperature</p>
</dd>
<dt>seAVt</dt>
<dd>
<p>Southeastern region average temperature (degrees C)</p>
</dd>
<dt>southAVt</dt>
<dd>
<p>Southern temperature</p>
</dd>
<dt>swAVt</dt>
<dd>
<p>Southwestern temperature</p>
</dd>
<dt>westAVt</dt>
<dd>
<p>Western temperature</p>
</dd>
<dt>northAVt</dt>
<dd>
<p>Northern temperature</p>
</dd>
<dt>mdbAVt</dt>
<dd>
<p>Murray-Darling basin temperature</p>
</dd>
<dt>auAVt</dt>
<dd>
<p>Australian average temperature, area-weighted mean</p>
</dd>
<dt>eastRain</dt>
<dd>
<p>Eastern rainfall</p>
</dd>
<dt>seRain</dt>
<dd>
<p>Southeast Australian annual rainfall (mm)</p>
</dd>
<dt>southRain</dt>
<dd>
<p>Southern rainfall</p>
</dd>
<dt>swRain</dt>
<dd>
<p>Southwest rainfall</p>
</dd>
<dt>westRain</dt>
<dd>
<p>Western rainfall</p>
</dd>
<dt>northRain</dt>
<dd>
<p>Northern rainfall</p>
</dd>
<dt>mdbRain</dt>
<dd>
<p>Murray-Darling basin rainfall</p>
</dd>
<dt>auRain</dt>
<dd>
<p>Australian average rainfall, area weighted</p>
</dd>
<dt>SOI</dt>
<dd>
<p>Annual average Southern Oscillation Index</p>
</dd>
<dt>co2mlo</dt>
<dd>
<p>Moana Loa CO2 concentrations, from 1959</p>
</dd>
<dt>co2law</dt>
<dd>
<p>Moana Loa CO2 concentrations, 1900 to 1978</p>
</dd>
<dt>CO2</dt>
<dd>
<p>CO2 concentrations, composite series</p>
</dd>
<dt>sunspot</dt>
<dd>
<p>Annual average sunspot counts</p>
</dd>
</dl>
<h3>Source</h3>
<p>Australian Bureau of Meteorology web pages:</p>
<p><a href="http://www.bom.gov.au/climate/change/index.shtml">http://www.bom.gov.au/climate/change/index.shtml</a></p>
<p>The CO2 series <code>co2law</code>, for Law Dome ice core data. is from <a href="http://cdiac.ornl.gov/trends/co2/lawdome.html">http://cdiac.ornl.gov/trends/co2/lawdome.html</a>.</p>
<p>The CO2 series <code>co2mlo</code> is from Dr. Pieter Tans, NOAA/ESRL (<a href="https://www.esrl.noaa.gov/gmd/ccgg/trends/">www.esrl.noaa.gov/gmd/ccgg/trends/</a>)</p>
<p>The series <code>CO2</code> is a composite series, obtained by adding 0.46 to he Law data for 1900 to 1958, then following this with the Moana Loa data that is avaiable from 1959. The addition of 0.46 is designed so that the averages from the two series agree for the period 1959 to 1968</p>
<p>Sunspot data is from <a href="http://sidc.oma.be/sunspot-data/">http://sidc.oma.be/sunspot-data/</a></p>
<h3>References</h3>
<p>D.M. Etheridge, L.P. Steele, R.L. Langenfelds, R.J. Francey, J.-M. Barnola and V.I. Morgan, 1998, <em>Historical CO2 records from the Law Dome DE08, DE08-2, and DSS ice cores</em>, in Trends: A Compendium of Data on Global Change, on line at Carbon Dioxide Information Analysis Center, Oak Ridge National Laboratory, U.S. Department of Energy, Oak Ridge, Tenn., U.S.A. <a href="http://cdiac.ornl.gov/trends/co2/lawdome.html">http://cdiac.ornl.gov/trends/co2/lawdome.html</a></p>
<p>Lavery, B., Joung, G. and Nicholls, N. 1997. An extended high-quality historical rainfall dataset for Australia. Australian Meteorological Magazine, 46, 27-38.</p>
<p>Nicholls, N., Lavery, B., Frederiksen, C.\ and Drosdowsky, W. 1996. Recent apparent changes in relationships between the El Nino – southern oscillation and Australian rainfall and temperature. Geophysical Research Letters 23: 3357-3360.</p>
<p>SIDC-team, World Data Center for the Sunspot Index, Royal Observatory of Belgium, Monthly Report on the International Sunspot Number, online catalogue of the sunspot index: <a href="http://www.sidc.be/sunspot-data/">http://www.sidc.be/sunspot-data/</a>, 1900-2011</p>
<h3>Examples</h3>
<pre>
plot(ts(bomregions[, c("mdbRain","SOI")], start=1900),
 panel=function(y,...)panel.smooth(bomregions$Year, y,...))
avrain &lt;- bomregions[,"mdbRain"]
xbomsoi &lt;- with(bomregions, data.frame(Year=Year, SOI=SOI,
cuberootRain=avrain^0.33))
xbomsoi$trendSOI &lt;- lowess(xbomsoi$SOI, f=0.1)$y
xbomsoi$trendRain &lt;- lowess(xbomsoi$cuberootRain, f=0.1)$y
xbomsoi$detrendRain &lt;-
with(xbomsoi, cuberootRain - trendRain + mean(trendRain))
xbomsoi$detrendSOI &lt;-
with(xbomsoi, SOI - trendSOI + mean(trendSOI))
## Plot time series avrain and SOI: ts object xbomsoi
plot(ts(xbomsoi[, c("cuberootRain","SOI")], start=1900),
 panel=function(y,...)panel.smooth(xbomsoi$Year, y,...),
 xlab = "Year", main="", ylim=list(c(250, 800),c(-20,25)))
par(mfrow=c(1,2))
rainpos &lt;- pretty(xbomsoi$cuberootRain^3, 6)
plot(cuberootRain ~ SOI, data = xbomsoi,
 ylab = "Rainfall (cube root scale)", yaxt="n")
axis(2, at = rainpos^0.33, labels=paste(rainpos))
mtext(side = 3, line = 0.8, "A", adj = -0.025)
with(xbomsoi, lines(lowess(cuberootRain ~ SOI, f=0.75)))
plot(detrendRain ~ detrendSOI, data = xbomsoi,
 xlab="Detrended SOI", ylab = "Detrended rainfall", yaxt="n")
axis(2, at = rainpos^0.33, labels=paste(rainpos))
with(xbomsoi, lines(lowess(detrendRain ~ detrendSOI, f=0.75)))
mtext(side = 3, line = 0.8, "B", adj = -0.025)
par(mfrow=c(1,1))
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-12938.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-12938.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-daag-bomregions.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-12938.json';</script>
