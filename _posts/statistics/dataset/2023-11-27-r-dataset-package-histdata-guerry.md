---
title: R Dataset / Package HistData / Guerry
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">Guerry</span> data set which pertains to Data from A.-M. Guerry, "Essay on the Moral Statistics of France". The <span class="mono">Guerry</span> data set is found in the <span class="mono">HistData</span> R package. You can load the <span class="mono">Guerry</span> data set in R by issuing the following command at the console <span class="mono">data("Guerry")</span>. This will load the data into a variable called <span class="mono">Guerry</span>. If R says the <span class="mono">Guerry</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("HistData")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-38726.csv">Guerry R data set</a></span>. The size of this file is about 9,358 bytes.</p><h2>Data from A.-M. Guerry, "Essay on the Moral Statistics of France"</h2>
<h3>Description</h3>
<p>Andre-Michel Guerry (1833) was the first to systematically collect and analyze social data on such things as crime, literacy and suicide with the view to determining social laws and the relations among these variables.</p>
<p>The Guerry data frame comprises a collection of 'moral variables' on the 86 departments of France around 1830. A few additional variables have been added from other sources.</p>
<h3>Usage</h3>
<pre>data(Guerry)</pre>
<h3>Format</h3>
<p>A data frame with 86 observations (the departments of France) on the following 23 variables.</p>
<dl>
<dt><code>dept</code></dt>
<dd>
<p>Department ID: Standard numbers for the departments, except for Corsica (200)</p>
</dd>
<dt><code>Region</code></dt>
<dd>
<p>Region of France ('N'='North', 'S'='South', 'E'='East', 'W'='West', 'C'='Central'). Corsica is coded as NA</p>
</dd>
<dt><code>Department</code></dt>
<dd>
<p>Department name: Departments are named according to usage in 1830, but without accents. A factor with levels <code>Ain</code> <code>Aisne</code> <code>Allier</code> ... <code>Vosges</code> <code>Yonne</code></p>
</dd>
<dt><code>Crime_pers</code></dt>
<dd>
<p>Population per Crime against persons. Source: A2 (Compte général, 1825-1830)</p>
</dd>
<dt><code>Crime_prop</code></dt>
<dd>
<p>Population per Crime against property. Source: A2 (Compte général, 1825-1830)</p>
</dd>
<dt><code>Literacy</code></dt>
<dd>
<p>Percent Read &amp; Write: Percent of military conscripts who can read and write. Source: A2</p>
</dd>
<dt><code>Donations</code></dt>
<dd>
<p>Donations to the poor. Source: A2 (Bulletin des lois)</p>
</dd>
<dt><code>Infants</code></dt>
<dd>
<p>Population per illegitimate birth. Source: A2 (Bureaau des Longitudes, 1817-1821)</p>
</dd>
<dt><code>Suicides</code></dt>
<dd>
<p>Population per suicide. Source: A2 (Compte général, 1827-1830)</p>
</dd>
<dt><code>MainCity</code></dt>
<dd>
<p>Size of principal city ('1:Sm', '2:Med', '3:Lg'), used as a surrogate for poulation density. Large refers to the top 10, small to the bottom 10; all the rest are classed Medium. Source: A1. An ordered factor with levels <code>1:Sm</code> &lt; <code>2:Med</code> &lt; <code>3:Lg</code></p>
</dd>
<dt><code>Wealth</code></dt>
<dd>
<p>Per capita tax on personal property. A ranked index based on taxes on personal and movable property per inhabitant. Source: A1</p>
</dd>
<dt><code>Commerce</code></dt>
<dd>
<p>Commerce and Industry, measured by the rank of the number of patents / population. Source: A1</p>
</dd>
<dt><code>Clergy</code></dt>
<dd>
<p>Distribution of clergy, measured by the rank of the number of Catholic priests in active service / population. Source: A1 (Almanach officiel du clergy, 1829)</p>
</dd>
<dt><code>Crime_parents</code></dt>
<dd>
<p>Crimes against parents, measured by the rank of the ratio of crimes against parents to all crimes– Average for the years 1825-1830. Source: A1 (Compte général)</p>
</dd>
<dt><code>Infanticide</code></dt>
<dd>
<p>Infanticides per capita. A ranked ratio of number of infanticides to population– Average for the years 1825-1830. Source: A1 (Compte général)</p>
</dd>
<dt><code>Donation_clergy</code></dt>
<dd>
<p>Donations to the clergy. A ranked ratio of the number of bequests and donations inter vivios to population– Average for the years 1815-1824. Source: A1 (Bull. des lois, ordunn. d'autorisation)</p>
</dd>
<dt><code>Lottery</code></dt>
<dd>
<p>Per capita wager on Royal Lottery. Ranked ratio of the proceeds bet on the royal lottery to population— Average for the years 1822-1826. Source: A1 (Compte rendus par le ministre des finances)</p>
</dd>
<dt><code>Desertion</code></dt>
<dd>
<p>Military disertion, ratio of the number of young soldiers accused of desertion to the force of the military contingent, minus the deficit produced by the insufficiency of available billets– Average of the years 1825-1827. Source: A1 (Compte du ministere du guerre, 1829 etat V)</p>
</dd>
<dt><code>Instruction</code></dt>
<dd>
<p>Instruction. Ranks recorded from Guerry's map of Instruction. Note: this is inversely related to <code>Literacy</code> (as defined here)</p>
</dd>
<dt><code>Prostitutes</code></dt>
<dd>
<p>Prostitutes in Paris. Number of prostitutes registered in Paris from 1816 to 1834, classified by the department of their birth Source: Parent-Duchatelet (1836), <em>De la prostitution en Paris</em></p>
</dd>
<dt><code>Distance</code></dt>
<dd>
<p>Distance to Paris (km). Distance of each department centroid to the centroid of the Seine (Paris) Source: cakculated from department centroids</p>
</dd>
<dt><code>Area</code></dt>
<dd>
<p>Area (1000 km^2). Source: Angeville (1836)</p>
</dd>
<dt><code>Pop1831</code></dt>
<dd>
<p>1831 population. Population in 1831, taken from Angeville (1836), <em>Essai sur la Statistique de la Population français</em>, in 1000s</p>
</dd>
</dl>
<h3>Details</h3>
<p>Note that most of the variables (e.g., <code>Crime_pers</code>) are scaled so that 'more is better' morally.</p>
<p>Values for the quantitative variables displayed on Guerry's maps were taken from Table A2 in the English translation of Guerry (1833) by Whitt and Reinking. Values for the ranked variables were taken from Table A1, with some corrections applied. The maximum is indicated by rank 1, and the minimum by rank 86.</p>
<h3>Source</h3>
<p>Angeville, A. (1836). <em>Essai sur la Statistique de la Population française</em> Paris: F. Doufour.</p>
<p>Guerry, A.-M. (1833). <em>Essai sur la statistique morale de la France</em> Paris: Crochard. English translation: Hugh P. Whitt and Victor W. Reinking, Lewiston, N.Y. : Edwin Mellen Press, 2002.</p>
<p>Parent-Duchatelet, A. (1836). <em>De la prostitution dans la ville de Paris</em>, 3rd ed, 1857, p. 32, 36</p>
<h3>References</h3>
<p>Dray, S. and Jombart, T. (2011). A Revisit Of Guerry's Data: Introducing Spatial Constraints In Multivariate Analysis. <em>The Annals of Applied Statistics</em>, Vol. 5, No. 4, 2278-2299. <a href="http://arxiv.org/pdf/1202.6485.pdf">http://arxiv.org/pdf/1202.6485.pdf</a>, DOI: 10.1214/10-AOAS356.</p>
<p>Brunsdon, C. and Dykes, J. (2007). Geographically weighted visualization: interactive graphics for scale-varying exploratory analysis. Geographical Information Science Research Conference (GISRUK 07), NUI Maynooth, Ireland, April, 2007.</p>
<p>Friendly, M. (2007). A.-M. Guerry's Moral Statistics of France: Challenges for Multivariable Spatial Analysis. <em>Statistical Science</em>, 22, 368-399.</p>
<p>Friendly, M. (2007). Data from A.-M. Guerry, Essay on the Moral Statistics of France (1833), <a href="http://datavis.ca/gallery/guerry/guerrydat.html">http://datavis.ca/gallery/guerry/guerrydat.html</a>.</p>
<h3>See Also</h3>
<p>The <span class="pkg">Guerry</span> package for maps of France: <code>gfrance</code> and related data.</p>
<h3>Examples</h3>
<pre>
data(Guerry)
## maybe str(Guerry) ; plot(Guerry) ...
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-38726.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-38726.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-histdata-guerry.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-38726.json';</script>