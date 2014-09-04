---
title       : Intro a R
subtitle    : Primer paso
author      : Arturo Chian
job         : UNMSM
--- .nobackground .quote

<q>R es lo máximo.</q>

--- &interactive2 height:100

<textarea class='interactive' id='interactive{{slide.num}}' data-cell='{{slide.num}}' data-results='asis' style='display:none'>library(datasets);data(swiss);library(stats);library(graphics)
pairs(swiss,panel=panel.smooth,main='Swissdata',col=3+(swiss$Catholic>50))</textarea>

--- &interactive2 height:100

<textarea class='interactive' id='interactive{{slide.num}}' data-cell='{{slide.num}}' data-results='asis' style='display:none'>summary(lm(Fertility ~ . , data = swiss))$coefficients</textarea>

--- &interactive2 height:40

<textarea class='interactive' id='interactive{{slide.num}}' data-cell='{{slide.num}}' data-results='asis' style='display:none'>library(Hmisc);library(ggplot2)
swiss$Examination2<-cut2(swiss$Examination,g=2)
qplot(Agriculture, Fertility, data = swiss, geom = c("point", "smooth"),
method = "lm", shape=Examination2)</textarea>



--- .segue .nobackground

## Thank You



<style>iframe.uvcharts{height: 600px;}</style>



