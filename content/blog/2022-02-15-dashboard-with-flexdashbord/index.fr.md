+++
title = "[projet] Construire un tableau de bord avec flexdashboard"
description = "Un projet de tableau de bord utilisé pour suivre l'évolution de la collecte de données lors d'une enquête."
author = "Bervelin Lumesa"
date = "2022-02-15"
tags = ["R", "Dashboard"]
categories = ["R", "Projects"]
comments = true
removeBlur = false
[[images]]
  src = "img/2019/03/dashboard.JPG"
  alt = "Tableau de bord"
  stretch = ""
+++

# Introduction

Un tableau de bord est un outil de pilotage permettant, grâce à son contenu, de suivre l'évolution d'un processus. Il mesure les performances afin de juger de l'état d'avancement (le chemin parcouru) et le chemin restant à parcourir pour accéder aux objectifs fixés. 

Dans l'industrie, il aide  par exemple à suivre les indicateurs associés au processus de production. Dans le domaine des enquêtes, un tableau de bord peut être utilisé lors de la collecte de données pour faire le suivi de la collecte grâce à un certain nombre d'indicateurs choisis. 
Il constitue de ce fait un puissant outil d'appui à la décision, en permettant de détecter des variations en temps réel (si possible).

Je partage avec vous le Code du tableau de bord que j'ai conçu et utilisé lors de l'opération de collecte de données dans le cadre de <a href = 'https://www.malariabehaviorsurvey.org' target ='_blank'>l'Equête Comportementale liée au Paludisme</a> en RDC en 2021 avec <a href = 'https://www.begis-congo.net' target ='_blank'>Begis Congo</a>.


# Construction du tableau de bord

Ce tableau de bord a été réalisé avec le language <a href = 'https://www.r-project.org' target ='_blank'>R</a> et son IDE <a href = 'https://www.rstudio.com' target ='_blank'>Rstudio</a>, avec le package flexdashbord qui est spécialisé pour la création des tableaux de bords. D'autres packages ont été utilisés comme : `haven` et `foreign` pour l'importation de données, `leaflet` pour la création de la carte, `tidyverse` pour la manipulation de données, `kableExtra` et `knitr` pour les tableaux.   

Ce tableau de bord est principalement composé de deux parties : une partie montre quelques indicateurs quels que _le nombre de ménages visitée_, _le nombre de femmes et hommes enquêtés_ et bien d'autres. La seconde donne une répartition spaciale des ménages enquêtés sur une carte intéractive, avec différentes couleurs pour chaque statut de ménage.

Pour plus de ressources, cliquez sur les liens suivants : 

- _<a href = 'https://pkgs.rstudio.com/flexdashboard/' target = '_blank'>flexdashboard</a>_
- _<a href = 'https://rstudio.github.io/flexdashboard/articles/examples.html' target = '_blank'>Example projects</a>_
- _<a href = 'https://www.paulamoraga.com/book-geospatial/sec-flexdashboard.html' target = '_blank'>Geospatial Health Data: Modeling and Visualization with R-INLA and Shiny</a>_

Tous les codes de ce post et bien d'autres peuvent être téléchargés sur <a href = 'https://www.github.com/bervelin-lumesa/mbs_drc_dashboard' target ='_blank'>Github</a>. 

Ce post vous a-t-il intéressé ? n'oubliez pas de le partager !

_TO KUTANI MBALA YA SIMA :)_


