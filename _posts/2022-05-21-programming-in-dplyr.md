---
title: Programming in the Tidyverse
subtitle: I explain how to use strings in R functions along with Tidyverse packages.
layout: default
date: 2022-05-21
keywords: R, programming, tidyverse
published: true
---

# The Tidyverse

One of the main features of using the `R` programming language is the presence
of packages like `dplyr`, `readr`, `tidyr`, `ggplot2` and others. Collectively
known as the *Tidyverse*, these packages often make interactive use with `R`
much better. With SQL-like syntax, these packages make it easy to read
previously written code and use the split-apply-combine procedure 
{% cite wickham2019advanced %} that often belies data analysis. For example, we
can count the number of cars in the `mtcars` data set by cylinder size (`cyl`):

{% highlight r %}

library(dplyr)

mtcars %>%
  group_by(cyl) %>%
  summarize(Count = n())

{% endhighlight %}


Notice that to benefit interactive use Tidyverse functions take symbols instead
of strings as input. In the previous example, this is demonstrated by the fact
that we group by `cyl` instead of `"cyl"`. This is helpful for interactive use
but it makes programming challenging because it is more difficult to reason
about the output.

<!-- Add R code -->

# Base R Functions

Unlike Tidyverse functions, base R functions make it easier to work with
strings:

<!-- Add R code -->

Furthermore, writing functions is encouraged when working with data as one can
use them within a data pipeline. However, to use strings as arguments one has
to use:

<!-- Add R code -->

# Bonus: Why not pass data as a function argument?
