---
title: 'Collecte de données mobile : Partage d''Expérience'
author: Bervelin
date: '2024-08-20'
slug: collecte-de-donn-es-mobile-partage-d-exp-rience
categories: []
tags: 
  - data collection
---

Mbote!

## Intro...

Depuis plusieurs années déjà, la collecte de données au moyen des tablettes ou smartphones est devenue monnaie courante, que ça soit pour des petites enquêtes ou pour des opérations de grandes envergures.

La conception des formulaires (le passage du questionnaire papier au formulaire électronique) obéit à un certain nombre de règles et de meilleures pratiques. Dans cet article, je vous partage mon expérience et quelques conseils qui pourront sans doute vous être utiles lors de vos projets en tant que Gestionnaire de données ou chargé de la conception du formulaire d'enquête.

## Du questionnaire papier au formulaire sur tablette

Dans la plupart des cas, le travail d'un Gestionnaire de données (Data Manager) ou le chargé de la conception du formulaire, dans le cadre d'une enquête statistique, commence lorsque l'outil de collecte de données (questionnaire papier) est finalisé. Sa tâche consiste alors à transformer l'outil en papier à un outil numérique (formulaire sur tablette ou smartphone) pour la collecte de données. Que faut-il considérer avant le choix de l'application de collecte de données ?

### Structure du questionnaire papier

Chaque questionnaire ayant ses particularités, je pense qu'il est important de commencer par comprendre celles-ci. Quels types de questions avons-nous (à répoonse unique, multiple, fermée, ouverte) ? Les questions concernent-elles une seule unité statistique ou plusieurs ? Comment identifier chaque questionnaire de façon unique ? Avons-nous un seul questionnaire ou plusieurs qu'il faudra lier ?

Les réponses à ces questions permettront de nous donner une idée générale du chemin à prendre pour aboutir à un résultat satisfaisant.

### Des questions aux variables

Lorsqu'on conçoit un formulaire (questionnaire sur tablette), il est important d'avoir à l'esprit qu'en régle générale, chaque question est répresentée par une variable (dans un fichier de données, un tableur Excel par exemple). Pour les questions à réponses multiples, chaque modalité de la variable devient une variable (colonne).

En absence d'un document définissant la façon de nommer les variables, la personne chargée de concevoir le formulaire doit réflechir en amont sur comment nommer les variables.

Personnellement, je réfechie toujours à la façon de nommer les variables avant de commencer à programmer.

### Pensez à l'analyste de données

Celui qui conçoit le formulaire n'est pas forcement celui qui analysera les données qui seront collectées. Il est donc important pour le gestionnaire de données de réflechir sur comment faciliter la tâche de celui/celle qui analysera les données. Ceci notamment à la manière de nommer les variables, l'inclusion ou non de structures de répétitions, le choix du type de variables. par exemple, au lieu de collecter une taille sous forme de `16 cm`, on la collectera sous forme de `16` en indiquant sur une note que "La taille est en centimètre". Le premier donnera le type chaîne de caractère et le second une variable numérique.

## Quelle application choisir ?

Actuellement, il existe beaucoup d'application permettant de collecter les données avec des tablettes ou smartphones. Il faut cependant avoir des critères qui permettent de jeter son dévolu sur un outil, plutôt qu'un autre. Ci-après je donne quelques critères que je considère pour choisir une application. La liste n'est pas exhaustive et ne devrait pas être considérée comme une référence.

### Familiarité avec l'outil

S'il m'est demandé de proposer un outil pour la collecte de données mobile, je choisirai sans doute celui avec lequel je suis famillier. Bien que cela ne soit pas le seul critère, mais il permet à la personne chargée de la conception de se focaliser directement sur les tâches, au lieu de se noyer dans la documentation pour comprendre le fonctionnement de l'outil. Il est aussi possible d'utiliser des parties d'un ancien projet sur lequel on a déjà travaillé et l'adapter.

Il m'arrive souvent d'utiliser quelques bouts de codes d'un ancien projet. Cela me permet de gagner du temps.

### Fonctionnalités offertes

Une application de collecte de données mobile est aussi choisie en fonction des fonctionnalités qu'elle offre. Cela peut être en terme de types de données qu'elle permet de collecter (Coordonnées GPS, Photo , vidéo, audio), la possibilité de synchronisation hors ligne ou de paramétrer l'accès par mot de passe. Pour des enquêtes ménages de grandes envergures ayant plusieurs questionnaires, on a souvent besoin d'avoir la possibilité de lier plusieurs formulaires et de partager les données entre ceux-ci. Par exemple après avoir collecté les données sur les noms et âges des membres d'un ménage, on peut alors enquêter chaque personne avec un foirmulaire individuel. On aura dans ce cas besoin de transférer tous les identifiants du ménage à chaque formulaire individuel.

### Disponibilité de la documentation

Ce point est très important dans la mesure où l'on peut avoir besoin d'aide durant le processus. Lors de la conception ou du deploiement d'un formulaire, on peut être buté à des problemes techniques qui nécessitent le recours à une documentation ou une communauté des utilisateurs. De ce fait, l'outil à choisir doit être bien documenté et cette documentation doit être accessible à moindre coût, ou gratuitement.

Je fais souvent des aller-retour vers des livres, Google ou ChatGPT pour chercher de l'aide.

### Budget disponible

Le budget disponible est déterminant dans le choix de l'outil. Ce coût est souvent lié au stockage des données dans le serveur plutôt qu'au coût d'acquisition de l'outil. Bien que ce point soit de la responsabilité de l'organisation qui pilote le projet, la personne chargée de la gestion de données doit disponibiliser ces informations pour aider les responsables dans le choix.

### Quels outils disponibles

| **Application**                                 | **Fonctions principales**                                                                                                                                                                          | **Avantages**                                                                                                                      | **Inconvénients**                                                                                                                                                                                                                                                                                        |
|-----------------|-------------------|-----------------|--------------------|
| **ODK (Open Data Kit)**                         | \- Création de formulaires personnalisés<br>- Collecte de données en ligne et hors ligne<br>- Exportation de données en formats variés (CSV, JSON, etc.)                                           | \- Open-source et gratuit<br>- Communauté active pour le support<br>- Flexibilité et personnalisable                               | \- Interface utilisateur basique<br>- Configuration initiale complexe (serveur)<br>-Pas de plan gratuit pour héberger les données                                                                                                                                                                        |
| **KoboToolbox**                                 | \- Création et déploiement facile de formulaires<br>- Collecte de données en ligne et hors ligne<br>- Outils d'analyse et de visualisation des données                                             | \- Gratuit et open-source<br>- Interface conviviale<br>- Support pour les situations d'urgence et humanitaires                     | \- Limitations dans la personnalisation avancée<br>- Dépendance à une connexion internet pour certaines fonctionnalités<br>- Capacités d'exportation limitées pour des ensembles de données très volumineux<br>-Plan gratuit pour héberger les données<br>-Pas de plan gratuit pour héberger les données |
| **SurveyCTO**                                   | \- Création et gestion avancée de formulaires<br>- Suivi et monitoring des données en temps réel<br>- Collecte de données en ligne et hors ligne<br>- Intégration avec des logiciels tiers         | \- Support technique robuste<br>- Sécurité des données avancée<br>- Personnalisation et flexibilité élevées                        | \- Coût d'utilisation élevé<br>- Complexité pour les utilisateurs débutants<br>- Certaines fonctionnalités avancées peuvent nécessiter une formation<br>-Plan gratuit pour héberger les données                                                                                                          |
| **CSPro (Census and Survey Processing System)** | \- Création de formulaires et de bases de données complexes<br>- Traitement et analyse des données<br>- Support multilingue<br>- Collecte de données en ligne et hors ligne                        | \- Gratuit et soutenu par des institutions gouvernementales<br>- Capacité à gérer des enquêtes complexes<br>- Support multilingue  | \- Interface utilisateur vieillissante<br>- Moins intuitif que les autres outils<br>-Paramétrage complexe pour le déploiement<br>- Courbe d'apprentissage plus raide pour les débutants                                                                                                                  |
| **CommCare**                                    | \- Création de formulaires dynamiques et interactifs<br>- Suivi longitudinal des données<br>- Intégration avec des systèmes de gestion de la santé<br>- Collecte de données en ligne et hors ligne | \- Conçu spécifiquement pour le secteur de la santé<br>- Interface utilisateur intuitive<br>- Support pour les workflows complexes | \- Coût d'utilisation pour certaines fonctionnalités<br>- Nécessite une formation pour les utilisateurs débutants<br>- Dépendance aux abonnements pour certaines fonctionnalités avancées                                                                                                                |

> [Apprenez à utiliser Kobotoolbox et ODK grâce à notre formation 100% ligne. Commencez maintenant!](https://www.fdtk.org/pv-collecte-de-donnees-mobile)

### Suivi de la collecte de données

Après avoir mis en place un système de collecte de données mobile, il est crucial de définir comment se fera la gestion de données au jour le jour. Cela revient à se poser des questions telles que :

-   Quelle est la qualité de données collectées ?
-   Quelle équipe commet le plus d'erreurs ?
-   Combien d'unités reste-il à enquêter ?
-   Quel est le taux de non-réponse ?
-   Où sont collectées les données ?
-   Etc...

Ces différentes questions nécessitent la mise en place d'un système (semi) automatique permettant de fournir des réponses en temps voulu pour faciliter la prise de décisions. Il doit conduire l'équipe de coordination à faire des feedbacks aux agents de terrain en vue d'améliorer la qualité de données. Ce point fera l'objet d'un autre article.

## Conclusion

La collecte de données mobile doit être préparée minitieusement pour être efficace. De la compréhension de la structure et des spécificités du questionnaire papier jusqu'au déploiement, en passant par le choix de la technologie et la programmation, rien ne doit être laissé au hasard. Une collecte de données mobile bien refléchie apportera toujours un gain de temps, de qualité, de ressources à l'organisation.

#### Besoin d'un expert pour appuyer votre projet de collecte de données ? [Contactez-moi! Je suis là pour vous accompagner.](mailto:lumesabervelin@gmail.com)

<br>

## Avez-vous trouvé cet article utile ? Pensez à le partager 🙌
