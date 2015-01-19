--- 
title       : Determining Average MPG from Transmission and Number of Cylinders
subtitle    : From the mtcars dataset
author      : jamayn02
job         : Developing Data Products Assignment
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]     # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
--- bg:green

## Introduction

This app is used to determine the MPG of cars from the mtcars dataset, extracted from the 1974 Motor Trend US magazine, based input from the user. Below shows the structure of the mtcars dataset:


```r
str(mtcars)
```

```
## 'data.frame':	32 obs. of  11 variables:
##  $ mpg : num  21 21 22.8 21.4 18.7 18.1 14.3 24.4 22.8 19.2 ...
##  $ cyl : num  6 6 4 6 8 6 8 4 4 6 ...
##  $ disp: num  160 160 108 258 360 ...
##  $ hp  : num  110 110 93 110 175 105 245 62 95 123 ...
##  $ drat: num  3.9 3.9 3.85 3.08 3.15 2.76 3.21 3.69 3.92 3.92 ...
##  $ wt  : num  2.62 2.88 2.32 3.21 3.44 ...
##  $ qsec: num  16.5 17 18.6 19.4 17 ...
##  $ vs  : num  0 0 1 1 0 1 0 1 1 1 ...
##  $ am  : num  1 1 1 0 0 0 0 0 0 0 ...
##  $ gear: num  4 4 4 3 3 3 3 4 4 4 ...
##  $ carb: num  4 4 1 1 2 1 4 2 2 4 ...
```

--- bg:red

## User Instructions

The user must input the transmission type from the choices below:

* Manual
* Auto

Additionally, the user must enter the number of cylinders from a drop down menu, consisting of the following choices:

* 4
* 6
* 8


---bg:orange

## Example

If the user chose the **manual** transmission type and the number of cylinders as **6**, the app will subset the dataset based on these criteria and calculate the average MPG.  The result for this example is shown below:


```
## [1] 20.57
```

---bg:yellow

## Example

Also, the app will display all cars that fit the criteria chosen by the user, along with the MPG for each car.  In this example, the app would display:


```
##                mpg
## Mazda RX4     21.0
## Mazda RX4 Wag 21.0
## Ferrari Dino  19.7
```

