---
title: R Dataset / Package gap / crohn
layout: page
permalink: /dataset/:slug
---
<div id="dataset-info">
<p>On this R-data statistics page, you will find information about the <span class="mono">crohn</span> data set which pertains to Crohn's disease data. The <span class="mono">crohn</span> data set is found in the <span class="mono">gap</span> R package. You can load the <span class="mono">crohn</span> data set in R by issuing the following command at the console <span class="mono">data("crohn")</span>. This will load the data into a variable called <span class="mono">crohn</span>. If R says the <span class="mono">crohn</span> data set is not found, you can try installing the package by issuing this command <span class="mono">install.packages("gap")</span> and then attempt to reload the data with the <span class="mono">library()</span> command. If you need to download R, you can go to the <a href="https://www.r-project.org">R project website</a>. You can download a CSV (comma separated values) version of the <span class="mono"><a href="../assets/data/csv/dataset-21865.csv">crohn R data set</a></span>. The size of this file is about 171,419 bytes.</p><h2>Crohn's disease data</h2>
<h3>Description</h3>
<p>The data set consist of 103 common (&gt;5% minor allele frequency) SNPs genotyped in 129 trios from an European-derived population. These SNPs are in a 500-kb region on human chromosome 5q31 implicated as containing a genetic risk factor for Crohn disease.</p>
<p>The positions, names and haplotype blocks reported are as follows,</p>
<pre>
274044 IGR1118a_1 BLOCK 1
274541 IGR1119a_1 *
286593 IGR1143a_1 *
287261 IGR1144a_1 *
299755 IGR1169a_2 *
324341 IGR1218a_2 *
324379 IGR1219a_2 *
358048 IGR1286a_1 BLOCK 1
366811 TSC0101718
395079 IGR1373a_1 BLOCK 2
396353 IGR1371a_1 *
397334 IGR1369a_2 *
397381 IGR1369a_1 *
398352 IGR1367a_1 BLOCK 2
411823 IGR2008a_2
411873 IGR2008a_1 BLOCK 3
412456 IGR2010a_3 *
413233 IGR2011b_1 *
415579 IGR2016a_1 *
417617 IGR2020a_15*
419845 IGR2025a_2 *
424283 IGR2033a_1 *
425376 IGR2036a_2 *
425549 IGR2036a_1 BLOCK 3
433467 IGR2052a_1 BLOCK 4
435282 IGR2055a_1 *
437682 IGR2060a_1 *
438883 IGR2063b_1 *
443565 IGR2072a_2 *
443750 IGR2073a_1 *
445337 IGR2076a_1 *
447791 IGR2081a_1 *
449895 IGR2085a_2 *
455246 IGR2096a_1 *
463136 IGR2111a_3 BLOCK 4
482171 IGR2150a_1 BLOCK 5
485828 IGR2157a_1 *
495082 IGR2175a_2 *
506266 IGR2198a_1 *
506890 IGR2199a_1 BLOCK 5
507208 IGR2200a_1 BLOCK 6
508338 IGR2202a_1 *
508858 IGR2203a_1 *
510951 IGR2207a_1 *
518478 IGR2222a_2 BLOCK 6
519387 IGR2224a_2 BLOCK 7
519962 IGR2225a_1 *
520521 IGR2226a_3 *
522600 IGR2230a_1 *
525243 IGR2236a_1 * 
529556 IGR2244a_4 *
532363 IGR2250a_4 *
545062 IGR2276a_1 *
553189 IGR2292a_1 *
570978 IGR3005a_1 *
571022 IGR3005a_2 *
576586 IGR3016a_1 *
577141 IGR3018a_2 *
577838 IGR3019a_2 *
578122 IGR3020a_1 *
579217 IGR3022a_1 *
579529 IGR3023a_1 *
579818 IGR3023a_3 *
582651 IGR3029a_1 *
582948 IGR3029a_2 *
583131 IGR3030a_1 *
587836 IGR3039a_1 *
590425 IGR3044a_1 *
590585 IGR3045a_1 *
594115 IGR3051a_1 *
594812 IGR3053a_1 *
598805 IGR3061a_1 *
601294 IGR3066a_1 *
608759 IGR3081a_1 *
610447 IGR3084a_1 *
611177 IGR3086a_1 BLOCK 7
613488 IGR3090a_1
616241 IGR3096a_1 BLOCK 8
616763 IGR3097a_1 *
617299 IGR3098a_1 *
626881 IGR3117a_1 *
633786 IGR3131a_1 *
635072 IGR3134a_1 *
637441 IGR3138a_1 BLOCK 8
648564 IGR3161a_1
649061 IGR3162a_1 BLOCK 9
649903 IGR3163a_1 *
657234 IGR3178a_1 *
662077 IGR3188a_1 *
662819 IGR3189a_2 *
676688 IGRX100a_1 BLOCK 9
683387 IGR3230a_1 BLOCK 10
686249 IGR3236a_1 *
692320 IGR3248a_1 *
718291 IGR3300a_2 *
730313 IGR3324a_1 *
731025 IGR3326a_1 *
738461 IGR3340a_1 BLOCK 10
871978 GENS021ex1_2 BLOCK 11
877571 GENS020ex3_3 *
877671 GENS020ex3_2 *
877809 GENS020ex3_1 *
890710 GENS020ex1_1 BLOCK 11
</pre>
<p>However it has been updated after the paper was published (posted on <a href="http://www.broad.mit.edu/humgen/IBD5/haplodata.html">http://www.broad.mit.edu/humgen/IBD5/haplodata.html</a>)</p>
<p>An example use of the data is with the following paper, Kelly M. Burkett, Celia M. T. Greenwood, BradMcNeney, Jinko Graham. Gene genealogies for genetic association mapping, with application to Crohn's disease. Fron Genet 2013, 4(260) doi: 10.3389/fgene.2013.00260</p>
<h3>Usage</h3>
<pre>data(crohn)</pre>
<h3>Format</h3>
<p>A data frame containing 387 rows and 212 columns</p>
<h3>Source</h3>
<p>MJ Daly, JD Rioux, SF Schaffner, TJ Hudson, ES Lander (2001) High-resolution haplotype structure in the human genome Nature Genetics 29:229-232</p>
<p>Dataset imported from <a href="https://www.r-project.org">https://www.r-project.org</a>.</p></div>
<p id="dataset-attachments">Attachments: <code><a target="_blank" href="/assets/data/csv/dataset-21865.csv">csv</a></code>, <code><a target="_blank" href="/assets/data/json/dataset-21865.json">json</a></code></p>
<div id="dataset-iframe">
{% highlight html %}
<iframe src="https://pmagunia.com/iframe/r-dataset-package-gap-crohn.html" width="100%" height="100%" style="border:0px"></iframe>
{% endhighlight %}
</div>
<div id="grid"></div>
<script>let json_file = 'dataset-21865.json';</script>