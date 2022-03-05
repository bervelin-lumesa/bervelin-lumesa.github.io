+++
title = "[project]Build a dashboard with flexdashboard"
description = "A dashboard project used to monitor data collection in a survey"
author = "Bervelin Lumesa"
date = "2022-02-15"
tags = ["R", "Dashboard"]
categories = ["R", "Projects"]
comments = true
removeBlur = false
[[images]]
  src = "img/2019/03/dashboard.JPG"
  alt = "dashboard"
  stretch = ""
+++

# Introduction

A dashboard is a management tool allowing, thanks to its content, to follow the evolution of a process. It measures performance in order to judge the state of progress (the path traveled) and the path remaining to be traveled to reach the objectives set.

In industry, for example, it helps to monitor indicators associated with the production process. In the area of surveys, a dashboard can be used during data collection to track collection through a number of selected indicators.
It therefore constitutes a powerful decision-support tool, allowing to detect variations in real time (if possible).

I share with you the R codes of the dashboard I designed and used during the data collection operation as part of the <a href = 'https://www.malariabehaviorsurvey.org' target ='_blank'>Malaria Behavioral Survey</a> in the DRC in 2021 with <a href = 'https://www.begis-congo.net' target ='_blank'>Begis Congo</a>.

# Dashboard construction

This dashboard was created with the <a href = 'https://www.r-project.org' target ='_blank'>R</a> language and its IDE <a href = 'https://www.rstudio.com' target ='_blank'>Rstudio</a>, with the `flexdashbord` package which is specialized for creating dashboards. Some other packages were used : `haven` and `foreign` for data import, `leaflet` for the map, `tidyverse` for data manipulation, `kableExtra` and `knitr` for beautiful tables. 

This dashboard is mainly composed of two parts: the first one shows some indicators such as _the number of households visited_, _the number of women and men surveyed_ and many others. The second gives a spatial distribution of the households surveyed on an interactive map, with different colors for each household status.

For more reading, check the following links : 

- _<a href = 'https://pkgs.rstudio.com/flexdashboard/' target = '_blank'>flexdashboard</a>_
- _<a href = 'https://rstudio.github.io/flexdashboard/articles/examples.html' target = '_blank'>Example projects</a>_
- _<a href = 'https://www.paulamoraga.com/book-geospatial/sec-flexdashboard.html' target = '_blank'>Geospatial Health Data: Modeling and Visualization with R-INLA and Shiny</a>_

All the code of this project and others can be downloaded in <a href = 'https://www.github.com/bervelin-lumesa/mbs_drc_dashboard' target ='_blank'>Github</a>. 

Was this post helpful ? Don't forget to share it !

_TO KUTANI MBALA YA SIMA :)_
