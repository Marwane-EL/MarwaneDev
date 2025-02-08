---
title: GestioN'Air
publishDate: 2020-03-04 00:00:00
img: /assets/gestionAir.png
img_alt: Pearls of silky soft white cotton, bubble up under vibrant lighting
description: |
  Ce projet vise à modéliser et optimiser la gestion de l'espace aérien français en minimisant les risques de collision entre vols. Il repose sur la construction et l'analyse d'un graphe d'intersection de vols afin d'attribuer des niveaux de vol de manière optimale.
tags:
  - Java
  - IHM
  - Graphe
  - Optimisation
---

#### Présentation du projet

Le projet consiste à gérer l'espace aérien français en attribuant des niveaux de vol à un ensemble de vols entre plusieurs aéroports. Chaque vol est caractérisé par son aéroport de départ, son aéroport d'arrivée, son heure de départ et sa durée.

Deux vols sont considérés comme en situation de risque si :

- leurs trajectoires s'intersectent dans l'espace,
- leur écart temporel de passage à l'intersection est inférieur à 15 minutes.

Afin d'éviter ces conflits, les vols en risque doivent être assignés à des niveaux de vol différents. L'objectif est donc d'affecter les vols à un nombre limité de niveaux de vol (à hauteur de kmax) en minimisant les conflits.

#### Technologies utilisées

Les technologies utilisées pour ce projet incluent :

- **Java** : Langage principal pour la gestion des données et des algorithmes.
- **JavaSwing** : Utilisé pour concevoir l'interface graphique interactive.

#### Fonctionnalités

La plateforme proposera plusieurs fonctionnalités clés :

- Construction et visualisation du graphe d’intersection des vols.
- Lecture et chargement d’un graphe directement depuis un fichier au format graph-testX.txt.
- Coloration optimisée des graphes pour minimiser le nombre de conflits.
- Interface graphique permettant de :
- Charger une liste de 20 graphes d’évaluation et les colorier avec le moins de conflits possibles.
- Visualiser le graphe d’intersection des vols.
