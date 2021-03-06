---
date: "2018-09-09T00:00:00Z"
draft: false
lastmod: "2018-09-09T00:00:00Z"
linktitle: From Gorilla to Tidy Data
summary: An introduction to data manipulation in R. We use tools from the tidyverse to process a dataset collected from Gorilla, an online experiment platform.
title: Tutorial summary
toc: true
type: docs
weight: 1
menu: gorilla-r
---

*********************

### Access the tutorial here: [https://emljames.github.io/GorillaR/index.html](https://emljames.github.io/GorillaR/index.html)

### Outline

The aim of this tutorial is to provide an introduction to data manipulation in R, primarily using tools from the *[tidyverse](https://www.tidyverse.org/)*. Given that lots of people are currently moving their data collection procedures online, we will use an output file from [Gorilla](https://gorilla.sc/) as an example. However, the tools should readily apply regardless of your data collection software.

In the first part of the tutorial, we will cover the basics of extracting the relevant data from your output files. In Part 2, we will cover some extra tips and tricks for monitoring sample size during online data collection, scaling up the tools to more complex datasets, and re-organising your data flexibly.


***********************

### Knowledge required

This introduction is aimed at beginners, with very little experience coding in R. 

However, it does assume that you can find your way around R Studio (i.e., familiar with the script and console, how to run one/several lines of code), and navigate your working directory to access your data. A basic understanding of functions and arguments will also help. Some recommended resources on this are:  

* [Data Carpentries](https://datacarpentry.org/r-socialsci/00-intro/index.html)
* [Introductory chapter in R for Data Science (Hadley Wickham)](https://r4ds.had.co.nz/workflow-basics.html)

If you prefer some light interactive activities, you can also try:  

* [DataCamp - R Onboarding](https://www.datacamp.com/onboarding/create_account?track_id=11)
* [Codeacademy - R](https://www.codecademy.com/learn/learn-r)

***********************

### What's this "tidyverse" you speak of? 

As with most programming tasks, there are multiple different ways of achieving the same thing. Within the R programming language, there are some clusters of approaches ("dialects" or "grammars", if you like). It's not essential to acknowledge the difference - mostly you will settle for whatever tools you can get to work! However, you will see when searching your issues on [StackExchange](https://stackexchange.com/) that many people provide alternative solutions, and will often refer to using *Base R*, the *tidyverse* (including *dplyr*, *tidyr* packages), and *data.table*. This document will focus on data manipulation using the *tidyverse*.

**What are the pros?**  

* Intuitive functions - they pretty much do what they say on the tin.  
* Readable and tidy - once you have understood a few key features (e.g., the pipe operator), it's relatively easy to read an existing script and gauge what's going on.   
* Efficient - you can carry out your data processing tasks in relatively few lines of code (as we will see here!)
* Wide usership - there is a huge amount of support available online.

**...and the cons?** 

* Coders transferring from different programming languages sometimes prefer base R operations, as they more directly relate to their existing knowledge.  
* Doesn't handle big data particularly well (the *data.table* package is better suited to this). But I really do mean big data here (i.e., sourced from rich naturally occurring datasets), most experimental data should be fine. 

For me, learning to use the *tidyverse* took me from years of copying and pasting random bits of code from the internet, to being able to sit down and write a data processing script from scratch. I hope you'll find it helpful too!

Ready? [Let's begin!](https://emljames.github.io/GorillaR/GorillaR_Part1.html)

***********************