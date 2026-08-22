+++
title = "Comment planifier ?"
description = "La règle d'or de l'estimation agile : estimer la taille et en déduire la durée grâce à la vélocité, plutôt qu'estimer directement le temps."
weight = 30
+++

> [!definition] Règle d'or Agile
> A key tenet of Agile estimating and planning is that **we estimate size but derive duration** [^1]

## Exemple
Illustrons la règle suivante, vous souhaitez transporter un tas de sable d'un point A à un point B.
- vous pourriez estimer directement qu'il vous faudra 5h
- Mais, une seconde approche consisterait à estimer la taille (size) du tas de sable en mètres cubes (e.g 20m^3) puis de déterminer la taille de la brouette (e.g 1m^3) et le temps de trajet entre A et B pour en dériver la durée

![estimating size](planifier/comment_planifier/images/estimating_size.png)

## Pourquoi la seconde approche ?
Les deux approches semblent similaires mais la deuxième devient intéressante une fois qu'on a notre Vélocité. En effet via l'estimation de la taille (en story point par exemple) et avec une Vélocité connue nous pouvons facilement en dériver la durée.

La dernière question est donc, *Comment déterminer la valeur en story point des premières features ?*. 
- Une stratégie consiste à prendre la feature la plus petite et l'estimer à 1 SP.
- Puis d'estimer les autres features en fonction de cette première feature (*x* fois plus complexe)

> [!affirmation] Affirmation
> Les points indiquent simplement le degré d’effort que chaque US représente PAR RAPPORT aux autres. 5 points représentent plus de travail que 3 points, 8 points représentent plus de travail que 5 points. ([ici]({{< relref "user_stories/user_story_points/facteurs_us/index.md" >}}))


[^1]: Agile Estimating & Planning p39