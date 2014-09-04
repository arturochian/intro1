---
title       : Intro a R
subtitle    : Primer paso
author      : Arturo Chian
job         : UNMSM
--- .nobackground .quote

<q>R es lo máximo.</q>

--- &interactive2 height:100

<a class='example'>NVD3</a>

<textarea class='interactive' id='interactive{{slide.num}}' data-cell='{{slide.num}}' data-results='asis' style='display:none'>library(datasets);data(swiss);library(stats);library(graphics)
pairs(swiss,panel=panel.smooth,main="Swissdata",col=3+(swiss$Catholic>50))</textarea>

--- &interactive2 height:100

<a class='example'>NVD3</a>

<textarea class='interactive' id='interactive{{slide.num}}' data-cell='{{slide.num}}' data-results='asis' style='display:none'>summary(lm(Fertility ~ . , data = swiss))$coefficients</textarea>

--- &interactive2 height:40

<a class='example'>DataTable</a>

<textarea class='interactive' id='interactive{{slide.num}}' data-cell='{{slide.num}}' data-results='asis' style='display:none'>summary(lm(Fertility~Agriculture,data=swiss))$coefficients
swiss$Infant.Mortality2<-cut2(swiss$Infant.Mortality,g=2)
qplot(Agriculture, Fertility, data = swiss, geom = c("point", "smooth"),
method = "lm", shape=Infant.Mortality2)</textarea>



--- .segue .nobackground

## Thank You



<style>iframe.uvcharts{height: 600px;}</style>



