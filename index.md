---
title       : Interactive Visualizations
subtitle    : rCharts, UseR 2014
author      : Ramnath Vaidyanathan (@ramnath_vaidya)
job         : McGill University
--- .nobackground .quote

<q>rCharts is an R package to create, customize and share interactive visualizations by leveraging javascript libraries.</q>

--- #rchartssite



--- &interactive2 height:100

<a class='example'>NVD3</a>

<textarea class='interactive' id='interactive{{slide.num}}' data-cell='{{slide.num}}' data-results='asis' style='display:none'>hair_eye_male <- subset(as.data.frame(HairEyeColor), Sex == 'Male')
library(rCharts)
n1 <- nPlot(Freq ~ Hair, group = 'Eye', data = hair_eye_male, type = 'multiBarChart')
n1</textarea>

--- &interactive2 height:100

<a class='example'>NVD3</a>

<textarea class='interactive' id='interactive{{slide.num}}' data-cell='{{slide.num}}' data-results='asis' style='display:none'>hair_eye_male <- subset(as.data.frame(HairEyeColor), Sex == 'Male')
library(rCharts)
n1 <- nPlot(Freq ~ Hair, group = 'Eye', data = hair_eye_male, type = 'multiBarChart')
n1$chart(color = c('brown', 'blue', '#594c26', 'green'))
n1</textarea>

--- &interactive2 height:40

<a class='example'>DataTable</a>

<textarea class='interactive' id='interactive{{slide.num}}' data-cell='{{slide.num}}' data-results='asis' style='display:none'>library(rCharts)
dTable(MASS::survey)</textarea>



--- .segue .nobackground

## Thank You



<style>iframe.uvcharts{height: 600px;}</style>



