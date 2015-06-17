---
title       : Regression analysis on mtcars dataset
subtitle    : Showcase
author      : Ismay Pérez Sánchez
job         : Coursera student
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap, quiz, mathjax]
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Background

It would be helpful if you are involved in the Data Science Specialization course and you already took the 7th course (Regression Models).  
Any way, if you didn't, it could be fun and even interesting for those taking that course in the present or later.  

About the data used
* The data was extracted from the 1974 Motor Trend US magazine.  
* It is available as an R package (datasets). No need to download, it comes with RStudio bundle intallation.
* If you want to verify the information locally you can deploy it in your R environment with the following:
  1. `library(datasets)`    load the package in your environment
  2. `data(mtcars)`         prepare a variable named *mtcars* with the data frame
  3. `?mtcars`              could help you to grasp what means each variable

---

## How to use my shiny [application](https://mooc-only.shinyapps.io/project)

1. Analyse the correlation between the potential predictors and MPG (miles per gallon).
2. Select candidates.
3. Verify $R^2$ to see the model coverage of the data variability. 
4. Check in the predictors table which of them have a significant influence in the model.
5. Verify in the plots if the residuals obtained are the expected for a good model.
6. Repeat from steps 2-5 until the result please you or you can't find any improvement.

--- &radio

## Hints about correlationship

Which predictor is more correlated with MPG ?

1. drat: 0.681
2. _wt: -0.868_
3. am: 0.6

*** .hint
Remember that the sign only mean that one covariate increase or decrease respect to other, nothing else.
*** .explanation
wt (Weight) is the most correlated predictor because it has the highest absolute value.

---

## Related with the original problem

In the Regression Models' course project, one of the original objetives was to determine which kind of transmition was the best respect the distance covered. Here, I present some information (using rCharts) where anyone could start to look for the answer.



<iframe src="assets/img/transmission_boxplot.html" width=50% height=50%></iframe>

