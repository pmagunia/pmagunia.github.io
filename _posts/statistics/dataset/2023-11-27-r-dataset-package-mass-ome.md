---
title: R Dataset / Package MASS / OME
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">OME</span> data set which pertains to Tests of Auditory Perception in Children with OME. The <span class="mono">OME</span> data set is found in the <span class="mono">MASS</span> R package. You can load the <span class="mono">OME</span> data set in R by issuing the following command at the console <span class="mono">data("OME")</span>. This will load the data into a variable called <span class="mono">OME</span>. If R says the <span class="mono">OME</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("MASS")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-52585.csv">OME R data set</a></span>. The size of this file is about 34,018 bytes.</p><h2>Tests of Auditory Perception in Children with OME</h2>
<h3>Description</h3>
<p>Experiments were performed on children on their ability to differentiate a signal in broad-band noise. The noise was played from a pair of speakers and a signal was added to just one channel; the subject had to turn his/her head to the channel with the added signal. The signal was either coherent (the amplitude of the noise was increased for a period) or incoherent (independent noise was added for the same period to form the same increase in power).</p>
<p>The threshold used in the original analysis was the stimulus loudness needs to get 75% correct responses. Some of the children had suffered from otitis media with effusion (OME).</p>
<h3>Usage</h3>
<pre>
OME
</pre>
<h3>Format</h3>
<p>The <code>OME</code> data frame has 1129 rows and 7 columns:</p>
<dl>
<dt><code>ID</code></dt>
<dd>
<p>Subject ID (1 to 99, with some IDs missing). A few subjects were measured at different ages.</p>
</dd>
<dt><code>OME</code></dt>
<dd>
<p><code>"low"</code> or <code>"high"</code> or <code>"N/A"</code> (at ages other than 30 and 60 months).</p>
</dd>
<dt><code>Age</code></dt>
<dd>
<p>Age of the subject (months).</p>
</dd>
<dt><code>Loud</code></dt>
<dd>
<p>Loudness of stimulus, in decibels.</p>
</dd>
<dt><code>Noise</code></dt>
<dd>
<p>Whether the signal in the stimulus was <code>"coherent"</code> or <code>"incoherent"</code>.</p>
</dd>
<dt><code>Correct</code></dt>
<dd>
<p>Number of correct responses from <code>Trials</code> trials.</p>
</dd>
<dt><code>Trials</code></dt>
<dd>
<p>Number of trials performed.</p>
</dd>
</dl>
<h3>Background</h3>
<p>The experiment was to study otitis media with effusion (OME), a very common childhood condition where the middle ear space, which is normally air-filled, becomes congested by a fluid. There is a concomitant fluctuating, conductive hearing loss which can result in various language, cognitive and social deficits. The term ‘binaural hearing’ is used to describe the listening conditions in which the brain is processing information from both ears at the same time. The brain computes differences in the intensity and/or timing of signals arriving at each ear which contributes to sound localisation and also to our ability to hear in background noise.</p>
<p>Some years ago, it was found that children of 7–8 years with a history of significant OME had significantly worse binaural hearing than children without such a history, despite having equivalent sensitivity. The question remained as to whether it was the timing, the duration, or the degree of severity of the otitis media episodes during critical periods, which affected later binaural hearing. In an attempt to begin to answer this question, 95 children were monitored for the presence of effusion every month since birth. On the basis of OME experience in their first two years, the test population was split into one group of high OME prevalence and one of low prevalence.</p>
<h3>Source</h3>
<p>Sarah Hogan, Dept of Physiology, University of Oxford, via Dept of Statistics Consulting Service</p>
<h3>Examples</h3>
<pre>
# Fit logistic curve from p = 0.5 to p = 1.0
fp1 &lt;- deriv(~ 0.5 + 0.5/(1 + exp(-(x-L75)/scal)),
 c("L75", "scal"),
 function(x,L75,scal)NULL)
nls(Correct/Trials ~ fp1(Loud, L75, scal), data = OME,
start = c(L75=45, scal=3))
nls(Correct/Trials ~ fp1(Loud, L75, scal),
data = OME[OME$Noise == "coherent",],
start=c(L75=45, scal=3))
nls(Correct/Trials ~ fp1(Loud, L75, scal),
data = OME[OME$Noise == "incoherent",],
start = c(L75=45, scal=3))# individual fits for each experimentaa &lt;- factor(OME$Age)
ab &lt;- 10*OME$ID + unclass(aa)
ac &lt;- unclass(factor(ab))
OME$UID &lt;- as.vector(ac)
OME$UIDn &lt;- OME$UID + 0.1*(OME$Noise == "incoherent")
rm(aa, ab, ac)
OMEi &lt;- OMElibrary(nlme)
fp2 &lt;- deriv(~ 0.5 + 0.5/(1 + exp(-(x-L75)/2)),
"L75", function(x,L75) NULL)
dec &lt;- getOption("OutDec")
options(show.error.messages = FALSE, OutDec=".")
OMEi.nls &lt;- nlsList(Correct/Trials ~ fp2(Loud, L75) | UIDn,
 data = OMEi, start = list(L75=45), control = list(maxiter=100))
options(show.error.messages = TRUE, OutDec=dec)
tmp &lt;- sapply(OMEi.nls, function(X)
{if(is.null(X)) NA else as.vector(coef(X))})
OMEif &lt;- data.frame(UID = round(as.numeric((names(tmp)))),
 Noise = rep(c("coherent", "incoherent"), 110),
 L75 = as.vector(tmp), stringsAsFactors = TRUE)
OMEif$Age &lt;- OME$Age[match(OMEif$UID, OME$UID)]
OMEif$OME &lt;- OME$OME[match(OMEif$UID, OME$UID)]
OMEif &lt;- OMEif[OMEif$L75 &gt; 30,]
summary(lm(L75 ~ Noise/Age, data = OMEif, na.action = na.omit))
summary(lm(L75 ~ Noise/(Age + OME), data = OMEif,
 subset = (Age &gt;= 30 &amp; Age &lt;= 60),
 na.action = na.omit), cor = FALSE)# Or fit by weighted least squares
fpl75 &lt;- deriv(~ sqrt(n)*(r/n - 0.5 - 0.5/(1 + exp(-(x-L75)/scal))),
 c("L75", "scal"),
 function(r,n,x,L75,scal) NULL)
nls(0 ~ fpl75(Correct, Trials, Loud, L75, scal),
data = OME[OME$Noise == "coherent",],
start = c(L75=45, scal=3))
nls(0 ~ fpl75(Correct, Trials, Loud, L75, scal),
data = OME[OME$Noise == "incoherent",],
start = c(L75=45, scal=3))# Test to see if the curves shift with age
fpl75age &lt;- deriv(~sqrt(n)*(r/n -0.5 - 0.5/(1 +
exp(-(x-L75-slope*age)/scal))),
c("L75", "slope", "scal"),
function(r,n,x,age,L75,slope,scal) NULL)
OME.nls1 &lt;-
nls(0 ~ fpl75age(Correct, Trials, Loud, Age, L75, slope, scal),
data = OME[OME$Noise == "coherent",],
start = c(L75=45, slope=0, scal=2))
sqrt(diag(vcov(OME.nls1)))OME.nls2 &lt;-
nls(0 ~ fpl75age(Correct, Trials, Loud, Age, L75, slope, scal),
data = OME[OME$Noise == "incoherent",],
start = c(L75=45, slope=0, scal=2))
sqrt(diag(vcov(OME.nls2)))# Now allow random effects by using NLME
OMEf &lt;- OME[rep(1:nrow(OME), OME$Trials),]
OMEf$Resp &lt;- with(OME, rep(rep(c(1,0), length(Trials)),
t(cbind(Correct, Trials-Correct))))
OMEf &lt;- OMEf[, -match(c("Correct", "Trials"), names(OMEf))]## Not run: ## these fail in R on most platforms
fp2 &lt;- deriv(~ 0.5 + 0.5/(1 + exp(-(x-L75)/exp(lsc))),
 c("L75", "lsc"),
 function(x, L75, lsc) NULL)
try(summary(nlme(Resp ~ fp2(Loud, L75, lsc),
 fixed = list(L75 ~ Age, lsc ~ 1),
 random = L75 + lsc ~ 1 | UID,
 data = OMEf[OMEf$Noise == "coherent",], method = "ML",
 start = list(fixed=c(L75=c(48.7, -0.03), lsc=0.24)), verbose = TRUE)))try(summary(nlme(Resp ~ fp2(Loud, L75, lsc),
 fixed = list(L75 ~ Age, lsc ~ 1),
 random = L75 + lsc ~ 1 | UID,
 data = OMEf[OMEf$Noise == "incoherent",], method = "ML",
 start = list(fixed=c(L75=c(41.5, -0.1), lsc=0)), verbose = TRUE)))## End(Not run)</pre>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-52585.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-52585.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-mass-ome.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-52585.json';</script>