---
title: R Dataset / Package HistData / Langren1644
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">Langren1644</span> data set which pertains to van Langren's Data on Longitude Distance between Toledo and Rome. The <span class="mono">Langren1644</span> data set is found in the <span class="mono">HistData</span> R package. You can load the <span class="mono">Langren1644</span> data set in R by issuing the following command at the console <span class="mono">data("Langren1644")</span>. This will load the data into a variable called <span class="mono">Langren1644</span>. If R says the <span class="mono">Langren1644</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("HistData")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-13846.csv">Langren1644 R data set</a></span>. The size of this file is about 1,077 bytes.</p><h2>van Langren's Data on Longitude Distance between Toledo and Rome</h2>
<h3>Description</h3>
<p>Michael Florent van Langren (1598-1675) was a Dutch mathematician and astronomer, who served as a royal mathematician to King Phillip IV of Spain, and who worked on one of the most significant problems of his time— the accurate determination of longitude, particularly for navigation at sea.</p>
<p>In order to convince the Spanish court of the seriousness of the problem (often resulting in great losses through ship wrecks), he prepared a 1-dimensional line graph, showing all the available estimates of the distance in longitude between Toledo and Rome, which showed large errors, for even this modest distance. This 1D line graph, from Langren (1644), is believed to be the first known graph of statistical data (Friendly etal., 2010). It provides a compelling example of the notions of statistical variability and bias.</p>
<p>The data frame <code>Langren1644</code> gives the estimates and other information derived from the previously known 1644 graph. It turns out that van Langren produced other versions of this graph, as early as 1628. The data frame <code>Langren.all</code> gives the estimates derived from all known versions of this graph.</p>
<h3>Usage</h3>
<pre>
data(Langren1644)
data(Langren.all)
</pre>
<h3>Format</h3>
<p><code>Langren1644</code>: A data frame with 12 observations on the following 9 variables, giving determinations of the distance in longitude between Toledo and Rome, from the 1644 graph.</p>
<dl>
<dt><code>Name</code></dt>
<dd>
<p>The name of the person giving a determination, a factor with levels <code>A. Argelius</code> ... <code>T. Brahe</code></p>
</dd>
<dt><code>Longitude</code></dt>
<dd>
<p>Estimated value of the longitude distance between Toledo and Rome</p>
</dd>
<dt><code>Year</code></dt>
<dd>
<p>Year associated with this determination</p>
</dd>
<dt><code>Longname</code></dt>
<dd>
<p>A longer version of the <code>Name</code>, where appropriate; a factor with levels <code>Andrea Argoli</code> <code>Christoph Clavius</code> <code>Tycho Brahe</code></p>
</dd>
<dt><code>City</code></dt>
<dd>
<p>The principal city where this person worked; a factor with levels <code>Alexandria</code> <code>Amsterdam</code> <code>Bamberg</code> <code>Bologna</code> <code>Frankfurt</code> <code>Hven</code> <code>Leuven</code> <code>Middelburg</code> <code>Nuremberg</code> <code>Padua</code> <code>Paris</code> <code>Rome</code></p>
</dd>
<dt><code>Country</code></dt>
<dd>
<p>The country where this person worked; a factor with levels <code>Belgium</code> <code>Denmark</code> <code>Egypt</code> <code>Flanders</code> <code>France</code> <code>Germany</code> <code>Italy</code> <code>Italy</code></p>
</dd>
<dt><code>Latitude</code></dt>
<dd>
<p>Latitude of this <code>City</code>; a numeric vector</p>
</dd>
<dt><code>Source</code></dt>
<dd>
<p>Likely source for this determination of Longitude; a factor with levels <code>Astron</code> <code>Map</code></p>
</dd>
<dt><code>Gap</code></dt>
<dd>
<p>A numeric vector indicating whether the <code>Longitude</code> value is below or above the median</p>
</dd>
</dl>
<p><code>Langren.all</code>: A data frame with 61 observations on the following 4 variables, giving determinations of Longitude between Toledo and Rome from all known versions of van Langren's graph.</p>
<dl>
<dt><code>Author</code></dt>
<dd>
<p>Author of the graph, a factor with levels <code>Langren</code> <code>Lelewel</code></p>
</dd>
<dt><code>Year</code></dt>
<dd>
<p>Year of publication</p>
</dd>
<dt><code>Name</code></dt>
<dd>
<p>The name of the person giving a determination, a factor with levels <code>Algunos1</code> <code>Algunos2</code> <code>Apianus</code> ... <code>Schonerus</code></p>
</dd>
<dt><code>Longitude</code></dt>
<dd>
<p>Estimated value of the longitude distance between Toledo and Rome</p>
</dd>
</dl>
<h3>Details</h3>
<p>In all the graphs, Toledo is implicitly at the origin and Rome is located relatively at the value of <code>Longitude</code> To judge correspondence with an actual map, the positions in (lat, long) are</p>
<p><code>toledo &lt;- c(39.86, -4.03); rome &lt;- c(41.89, 12.5)</code></p>
<h3>Source</h3>
<p>The longitude values were digitized from images of the various graphs, which may be found on the Supplementary materials page for Friendly etal. (2009).</p>
<h3>References</h3>
<p>Friendly, M., Valero-Mora, P. and Ulargui, J. I. (2010). The First (Known) Statistical Graph: Michael Florent van Langren and the "Secret" of Longitude. <em>The American Statistician</em>, <b>64</b> (2), 185-191. Supplementary materials: <a href="http://datavis.ca/gallery/langren/">http://datavis.ca/gallery/langren/</a>.</p>
<p>Langren, M. F. van. (1644). <em>La Verdadera Longitud por Mar y Tierra</em>. Antwerp: (n.p.), 1644. English translation available at <a href="http://www.math.yorku.ca/SCS/Gallery/langren/verdadera.pdf">http://www.math.yorku.ca/SCS/Gallery/langren/verdadera.pdf</a>.</p>
<p>Lelewel, J. (1851). <em>G?ographie du Moyen ?ge</em>. Paris: Pilliet, 1851.</p>
<h3>Examples</h3>
<pre>
data(Langren1644)####################################################
# reproductions of Langren's graph overlaid on a map
####################################################if (require(jpeg, quietly=TRUE)) {gimage &lt;- readJPEG(system.file("images", "google-toledo-rome3.jpg", package="HistData"))
# NB: dimensions from readJPEG are y, x, colorsgdim &lt;- dim(gimage)[1:2]
ylim &lt;- c(1,gdim[1])
xlim &lt;- c(1,gdim[2])
op &lt;- par(bty="n", xaxt="n", yaxt="n", mar=c(2, 1, 1, 1) + 0.1)
# NB: necessary to scale the plot to the pixel coordinates, and use asp=1
plot(xlim, ylim, xlim=xlim, ylim=ylim, type="n", ann=FALSE, asp=1 )
rasterImage(gimage, 1, 1, gdim[2], gdim[1])# pixel coordinates of Toledo and Rome in the image, measured from the bottom left corner
toledo.map &lt;- c(131, 59)
rome.map &lt;- c(506, 119)

# confirm locations of Toledo and Rome
points(rbind(toledo.map, rome.map), cex=2)
text(131, 95, "Toledo", cex=1.5)
text(506, 104, "Roma", cex=1.5)# set a scale for translation of lat,long to pixel x,y
scale &lt;- data.frame(x=c(131, 856), y=c(52,52))
rownames(scale)=c(0,30)# translate from degrees longitude to pixels
xlate &lt;- function(x) {
131+x*726/30
}# draw an axis
lines(scale)
ticks &lt;- xlate(seq(0,30,5))
segments(ticks, 52, ticks, 45)
text(ticks, 40, seq(0,30,5))
text(xlate(8), 17, "Grados de la Longitud", cex=1.7)# label the observations with the names
points(x=xlate(Langren1644$Longitude), y=rep(57, nrow(Langren1644)), 
 pch=25, col="blue", bg="blue")
text(x=xlate(Langren1644$Longitude), y=rep(57, nrow(Langren1644)), 
 labels=Langren1644$Name, srt=90, adj=c(-.1, .5), cex=0.8)
par(op)
}### Original implementation using ReadImages, now deprecated &amp; shortly to be removed
## Not run: 
if (require(ReadImages)) {
gimage &lt;- read.jpeg(system.file("images", "google-toledo-rome3.jpg", package="HistData"))
plot(gimage)

# pixel coordinates of Toledo and Rome in the image, measured from the bottom left corner
toledo.map &lt;- c(130, 59)
rome.map &lt;- c(505, 119)

# confirm locations of Toledo and Rome
points(rbind(toledo.map, rome.map), cex=2)

# set a scale for translation of lat,long to pixel x,y
scale &lt;- data.frame(x=c(130, 856), y=c(52,52))
rownames(scale)=c(0,30)
lines(scale)

xlate &lt;- function(x) {
130+x*726/30
}
points(x=xlate(Langren1644$Longitude), y=rep(57, nrow(Langren1644)), 
 pch=25, col="blue")
text(x=xlate(Langren1644$Longitude), y=rep(57, nrow(Langren1644)), 
 labels=Langren1644$Name, srt=90, adj=c(0, 0.5), cex=0.8)
}## End(Not run)### First attempt using ggplot2; temporarily abandonned.
## Not run: 
require(maps)
require(ggplot2)
require(reshape)
require(plyr)
require(scales)# set latitude to that of Toledo
Langren1644$Latitude &lt;- 39.68#x/long y/lat
bbox &lt;- c( 38.186, -9.184,
 43.692, 28.674 )
bbox &lt;- matrix(bbox, 2, 2, byrow=TRUE)borders &lt;- as.data.frame(map("world", plot = FALSE,
xlim = expand_range(bbox[,2], 0.2),
ylim = expand_range(bbox[,1], 0.2))[c("x", "y")])data(world.cities)
# get actual locations of Toledo &amp; Rome
cities &lt;- subset(world.cities,
name %in% c("Rome", "Toledo") &amp; country.etc %in% c("Spain", "Italy"))
colnames(cities)[4:5]&lt;-c("Latitude", "Longitude")mplot &lt;- ggplot(Langren1644, aes(Longitude, Latitude) ) +
geom_path(aes(x, y), borders, colour = "grey60") +
geom_point(y = 40) +
geom_text(aes(label = Name), y = 40.1, angle = 90, hjust = 0, size = 3)
mplot &lt;- mplot +
geom_segment(aes(x=-4.03, y=40, xend=30, yend=40))mplot &lt;- mplot +
geom_point(data = cities, colour = "red", size = 2) +
geom_text(data=cities, aes(label=name), color="red", size=3, vjust=-0.5) +
coord_cartesian(xlim=bbox[,2], ylim=bbox[,1])# make the plot have approximately aspect ratio = 1
windows(width=10, height=2)
mplot## End(Not run)
###########################################
# show variation in estimates across graphs
###########################################library(lattice)
graph &lt;- paste(Langren.all$Author, Langren.all$Year)
dotplot(Name ~ Longitude, data=Langren.all)dotplot( as.factor(Year) ~ Longitude, data=Langren.all, groups=Name, type="o")dotplot(Name ~ Longitude|graph, data=Langren.all, groups=graph)# why the gap?
gap.mod &lt;- glm(Gap ~ Year + Source + Latitude, family=binomial, data=Langren1644)
anova(gap.mod, test="Chisq")
</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-13846.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-13846.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-histdata-langren1644.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-13846.json';</script>