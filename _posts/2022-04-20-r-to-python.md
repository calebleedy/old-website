---
title: Converting from R to Python
subtitle: I give a brief overview of how to accomplish routine R tasks in Python.
layout: default
date: 2022-04-20
keywords: R, Python, programming
published: true
---

After using the [R programming language](https://www.r-project.org/) for
several years, I needed to use an optimal transport function for a statistical
project. While the R
[transport](https://cran.r-project.org/web/packages/transport/index.html)
package is useful, it lacks the ability to apply an estimated optimal transport
function onto a new data set. Enter the
[Python Optimal Transport](https://pythonot.github.io/) module. This
well-maintained and well-documented module opened up the door for me to learn
[Python](https://www.python.org/).

Unfortunately, my fluency in R has not immediately translated over to Python.
In almost all of my projects, I have a similar need to read, clean, and modify
data. Yet, the documentation for this translation always seemed to escape me.
Here is my attempt to match in Python what I am familiar with in R:


R              | Python 
---------------|--------
dim(df)        | df.shape
class(df)      | type(df)


