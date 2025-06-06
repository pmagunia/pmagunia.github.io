---
title: R Dataset / Package HistData / MacdonellDF
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">MacdonellDF</span> data set which pertains to Macdonell's Data on Height and Finger Length of Criminals, used by Gosset (1908). The <span class="mono">MacdonellDF</span> data set is found in the <span class="mono">HistData</span> R package. You can load the <span class="mono">MacdonellDF</span> data set in R by issuing the following command at the console <span class="mono">data("MacdonellDF")</span>. This will load the data into a variable called <span class="mono">MacdonellDF</span>. If R says the <span class="mono">MacdonellDF</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("HistData")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-63790.csv">MacdonellDF R data set</a></span>. The size of this file is about 57,283 bytes.</p><h2>Macdonell's Data on Height and Finger Length of Criminals, used by Gosset (1908)</h2>
<h3>Description</h3>
<p>In the second issue of <em>Biometrika</em>, W. R. Macdonell (1902) published an extensive paper, <em>On Criminal Anthropometry and the Identification of Criminals</em> in which he included numerous tables of physical characteristics 3000 non-habitual male criminals serving their sentences in England and Wales. His Table III (p. 216) recorded a bivariate frequency distribution of <code>height</code> by <code>finger</code> length. His main purpose was to show that Scotland Yard could have indexed their material more efficiently, and find a given profile more quickly.</p>
<p>W. S. Gosset (aka "Student") used these data in two classic papers in 1908, in which he derived various characteristics of the sampling distributions of the mean, standard deviation and Pearson's r. He said, "Before I had succeeded in solving my problem analytically, I had endeavoured to do so empirically." Among his experiments, he randomly shuffled the 3000 observations from Macdonell's table, and then grouped them into samples of size 4, 8, ..., calculating the sample means, standard deviations and correlations for each sample.</p>
<h3>Usage</h3>
<pre>
data(Macdonell)
data(MacdonellDF)
</pre>
<h3>Format</h3>
<p><code>Macdonell</code>: A frequency data frame with 924 observations on the following 3 variables giving the bivariate frequency distribution of <code>height</code> and <code>finger</code>.</p>
<dl>
<dt><code>height</code></dt>
<dd>
<p>lower class boundaries of height, in decimal ft.</p>
</dd>
<dt><code>finger</code></dt>
<dd>
<p>length of the left middle finger, in mm.</p>
</dd>
<dt><code>frequency</code></dt>
<dd>
<p>frequency of this combination of <code>height</code> and <code>finger</code></p>
</dd>
</dl>
<p><code>MacdonellDF</code>: A data frame with 3000 observations on the following 2 variables.</p>
<dl>
<dt><code>height</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
<dt><code>finger</code></dt>
<dd>
<p>a numeric vector</p>
</dd>
</dl>
<h3>Details</h3>
<p>Class intervals for <code>height</code> in Macdonell's table were given in 1 in. ranges, from (4' 7" 9/16 - 4' 8" 9/16), to (6' 4" 9/16 - 6' 5" 9/16). The values of <code>height</code> are taken as the lower class boundaries.</p>
<p>For convenience, the data frame <code>MacdonellDF</code> presents the same data, in expanded form, with each combination of <code>height</code> and <code>finger</code> replicated <code>frequency</code> times.</p>
<h3>Source</h3>
<p>Macdonell, W. R. (1902). On Criminal Anthropometry and the Identification of Criminals. <em>Biometrika</em>, 1(2), 177-227. doi:10.1093/biomet/1.2.177 <a href="http://www.jstor.org/stable/2331487">http://www.jstor.org/stable/2331487</a></p>
<p>The data used here were obtained from:</p>
<p>Hanley, J. (2008). Macdonell data used by Student. <a href="http://www.medicine.mcgill.ca/epidemiology/hanley/Student/">http://www.medicine.mcgill.ca/epidemiology/hanley/Student/</a></p>
<h3>References</h3>
<p>Hanley, J. and Julien, M. and Moodie, E. (2008). Student's z, t, and s: What if Gosset had R? <em>The American Statistican</em>, 62(1), 64-69.</p>
<p>Gosett, W. S. [Student] (1908). Probable error of a mean. <em>Biometrika</em>, 6(1), 1-25. <a href="http://www.york.ac.uk/depts/maths/histstat/student.pdf">http://www.york.ac.uk/depts/maths/histstat/student.pdf</a></p>
<p>Gosett, W. S. [Student] (1908). Probable error of a correlation coefficient. <em>Biometrika</em>, 6, 302-310.</p>
<h3>Examples</h3>
<pre>
data(Macdonell)# display the frequency table
xtabs(frequency ~ finger+round(height,3), data=Macdonell)## Some examples by james.hanley@mcgill.caOctober 16, 2011
## http://www.biostat.mcgill.ca/hanley/
## See:http://www.biostat.mcgill.ca/hanley/Student/###############################################
##naive contour plots of height and finger ##
###############################################
 
# make a 22 x 42 table
attach(Macdonell)
ht &lt;- unique(height) 
fi &lt;- unique(finger)
fr &lt;- t(matrix(frequency, nrow=42))
detach(Macdonell)
dev.new(width=10, height=5)# make plot double wide
op &lt;- par(mfrow=c(1,2),mar=c(0.5,0.5,0.5,0.5),oma=c(2,2,0,0))dx &lt;- 0.5/12
dy &lt;- 0.5/12plot(ht,ht,xlim=c(min(ht)-dx,max(ht)+dx),
 ylim=c(min(fi)-dy,max(fi)+dy), xlab="", ylab="", type="n" )# unpack3000 heights while looping though the frequencies 
heights &lt;- c()
for(i in 1:22) {
for (j in 1:42) {
 f&lt;-fr[i,j]
 if(f&gt;0) heights &lt;- c(heights,rep(ht[i],f))
 if(f&gt;0) text(ht[i], fi[j], toString(f), cex=0.4, col="grey40" ) 
}
}
text(4.65,13.5, "Finger length (cm)",adj=c(0,1), col="black") ;
text(5.75,9.5, "Height (feet)", adj=c(0,1), col="black") ;
text(6.1,11, "Observed bin\nfrequencies", adj=c(0.5,1), col="grey40",cex=0.85) ;
# crude countour plot
contour(ht, fi, fr, add=TRUE, drawlabels=FALSE, col="grey60")
# smoother contour plot (Galton smoothed 2-D frequencies this way)
# [Galton had experience with plotting isobars for meteorological data]
# it was the smoothed plot that made him remember his 'conic sections'
# and ask a mathematician to work out for him the iso-density
# contours of a bivariate Gaussian distribution... dx &lt;- 0.5/12; dy &lt;- 0.05; # shifts caused by averagingplot(ht,ht,xlim=c(min(ht),max(ht)),ylim=c(min(fi),max(fi)), xlab="", ylab="", type="n")
 
sm.fr &lt;- matrix(rep(0,21*41),nrow &lt;- 21)
for(i in 1:21) {
for (j in 1:41) {
 smooth.freq&lt;-(1/4) * sum( fr[i:(i+1), j:(j+1)] ) 
 sm.fr[i,j]&lt;-smooth.freq
 if(smooth.freq &gt; 0 )
 text(ht[i]+dx, fi[j]+dy, sub("^0.", ".",toString(smooth.freq)), cex=0.4, col="grey40" )
 }
}
 
contour(ht[1:21]+dx, fi[1:41]+dy, sm.fr, add=TRUE, drawlabels=FALSE, col="grey60")
text(6.05,11, "Smoothed bin\nfrequencies", adj=c(0.5,1), col="grey40", cex=0.85) ;
par(op)
dev.new()# new default device#######################################
## bivariate kernel density estimate
#######################################if(require(KernSmooth)) {
MDest &lt;- bkde2D(MacdonellDF, bandwidth=c(1/8, 1/8))
contour(x=MDest$x1, y=MDest$x2, z=MDest$fhat,
xlab="Height (feet)", ylab="Finger length (cm)", col="red", lwd=2)
with(MacdonellDF, points(jitter(height), jitter(finger), cex=0.5))
}#############################################################
## sunflower plot of height and finger with data ellipses##
#############################################################with(MacdonellDF, 
{
sunflowerplot(height, finger, size=1/12, seg.col="green3",
xlab="Height (feet)", ylab="Finger length (cm)")
reg &lt;- lm(finger ~ height)
abline(reg, lwd=2)
if(require(car)) {
dataEllipse(height, finger, plot.points=FALSE, levels=c(.40, .68, .95))
}
})
############################################################
## Sampling distributions of sample sd (s) and z=(ybar-mu)/s
############################################################# note that Gosset used a divisor of n (not n-1) to get the sd.
# He also used Sheppard's correction for the 'binning' or grouping.
# with concatenated height measurements...mu &lt;- mean(heights) ; sigma &lt;- sqrt( 3000 * var(heights)/2999 )
c(mu,sigma)# 750 samples of size n=4 (as Gosset did)# see Student's z, t, and s: What if Gosset had R? 
# [Hanley J, Julien M, and Moodie E. The American Statistician, February 2008] # see also the photographs from Student's notebook ('Original small sample data and notes")
# under the link "Gosset' 750 samples of size n=4" 
# on website http://www.biostat.mcgill.ca/hanley/Student/
# and while there, look at the cover of the Notebook containing his yeast-cell counts
# http://www.medicine.mcgill.ca/epidemiology/hanley/Student/750samplesOf4/Covers.JPG
# (Biometrika 1907) and decide for yourself why Gosset, when forced to write under a 
# pen-name, might have taken the name he did!# PS: Can you figure out what the 750 pairs of numbers signify?
# hint: look again at the numbers of rows and columns in Macdonell's (frequency) Table III.
n &lt;- 4
Nsamples &lt;- 750y.bar.values &lt;- s.over.sigma.values &lt;- z.values &lt;- c()
for (samp in 1:Nsamples) {
y &lt;- sample(heights,n)
y.bar &lt;- mean(y)
s&lt;-sqrt( (n/(n-1))*var(y) ) 
z &lt;- (y.bar-mu)/s
y.bar.values &lt;- c(y.bar.values,y.bar) 
s.over.sigma.values &lt;- c(s.over.sigma.values,s/sigma)
z.values &lt;- c(z.values,z)
} 
op &lt;- par(mfrow=c(2,2),mar=c(2.5,2.5,2.5,2.5),oma=c(2,2,0,0))
# sampling distributions
hist(heights,breaks=seq(4.5,6.5,1/12), main="Histogram of heights (N=3000)")
hist(y.bar.values, main=paste("Histogram of y.bar (n=",n,")",sep=""))hist(s.over.sigma.values,breaks=seq(0,4,0.1),
main=paste("Histogram of s/sigma (n=",n,")",sep="")); 
z=seq(-5,5,0.25)+0.125
hist(z.values,breaks=z-0.125, main="Histogram of z=(ybar-mu)/s")
# theoretical
lines(z, 750*0.25*sqrt(n-1)*dt(sqrt(n-1)*z,3), col="red", lwd=1)
par(op)#####################################################
## Chisquare probability plot for bivariate normality
#####################################################mu &lt;- colMeans(MacdonellDF)
sigma &lt;- var(MacdonellDF)
Dsq &lt;- mahalanobis(MacdonellDF, mu, sigma)Q &lt;- qchisq(1:3000/3000, 2)
plot(Q, sort(Dsq), xlab="Chisquare (2) quantile", ylab="Squared distance")
abline(a=0, b=1, col="red", lwd=2)</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-63790.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-63790.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-histdata-macdonelldf.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-63790.json';</script>