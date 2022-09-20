---
title: This is a test of RMarkdown in Jekyll
subtitle: This is a test of a subtitle
layout: default
date: 2022-04-01
keywords: R, programming
published: true
---

# Introduction

This is my intro.


{% highlight r %}
library(dplyr)
library(ggplot2)
{% endhighlight %}

We loaded some R packages. Here are some plots.


{% highlight r %}
ggplot(mtcars, aes(x = mpg, y = cyl)) +
  geom_point()
{% endhighlight %}

![center](/images/2022-04-01-testing-rmd/plots-1.png)
