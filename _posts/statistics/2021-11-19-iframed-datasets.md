---
title: Using Picostat IFRAMES to Embed Datasets on Webpages
author: pmagunia
layout: page
permalink: /statistics/:slug.html
redirect_from: /iframed-datasets.html
---
<a href="https://www.picostat.com">Picostat</a> is a web application I created with Drupal 7/8/9. It has support for embedding custom datasets in webpages after they have been imported. If the dataset has been imported correctly there will be an IFRAME tag below the grid which you can copy and paste the dataset onto webpages that have support for IFRAMEs. The tag looks something like this:

{% highlight xml %}
<iframe src="https://embed.picostat.com/openintro-statistics-dataset-starbucks.html" frameBorder="0" width="100%" height="307px" />
{% endhighlight %}

Sharing the dataset like with this method allows users to have an Excel-like view of the data.

There is also a basic filter near the top of the columns that allows users to subset the data.

Here is a screenshot of the Picostat site:

<img src="/assets/images/picostat.png" alt="Picostat Screnshot of a statistics dataset." style="width:100%; height: auto;"/>
The embedded dataset would appear like this in webpages like this one:
<iframe src="https://embed.picostat.com/openintro-statistics-dataset-starbucks.html" frameBorder="0" width="100%" height="307px"></iframe>


