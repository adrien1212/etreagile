+++
title = "Value Stream Map"
description = "La Value Stream Map cartographie la suite d'activités menant à la livraison, et rend visible le temps passé à attendre plutôt qu'à produire."
weight = 50
+++

> [!ressource] Ressources
> - Karen Martin et Mike Osterling, *Value Stream Mapping: How to Visualize Work and Align Leadership for Organizational Transformation* (2013)
> - Mike Rother et John Shook, *Learning to See* (1999)
> - [Lean Enterprise Institute — Value Stream Mapping](https://www.lean.org/lexicon-terms/value-stream-mapping/)

> [!definition] Définition
> - the sequence of activities an organization undertakes to deliver upon a customer request
> - (ou) the sequence of activities required to design, produce, and deliver a good or service to a customer, including the dual flows of information and material. [^1]

## Conséquence

De nombreuses équipes et organisations se trouvent dans des situations où les délais de déploiement sont de plusieurs mois. Avec des systèmes monolithiques étroitement couplés, souvent avec des environnements de test d'intégration rares, de longs délais pour les environnements de test et de production, une forte dépendance à l'égard des tests manuels et de multiples processus d'approbation requis.

![valuestreammap](valuestreammap.png)

## Comment on la lit

Une VSM se lit sur **deux lignes de temps**, et c'est tout son intérêt.

- Le **temps de traitement** (*process time*) : la durée pendant laquelle quelqu'un travaille effectivement sur l'élément.
- Le **temps écoulé** (*lead time*) : la durée totale, du moment où l'élément arrive à l'étape jusqu'au moment où il en sort — attentes comprises.

L'écart entre les deux est le temps passé **en file d'attente** : à attendre une validation, un environnement, une relecture, une disponibilité.

> [!definition] L'efficacité du flux
> On en tire un ratio : **efficacité = temps de traitement ÷ temps écoulé**.
>
> Sur la plupart des chaînes de livraison logicielle non optimisées, ce ratio se situe entre **5 % et 15 %**. Autrement dit, une demande passe l'écrasante majorité de sa vie à ne rien faire.

## Pourquoi c'est l'outil le plus utile du Lean

Parce qu'il déplace l'attention là où se trouve réellement le problème.

Devant un délai de livraison trop long, le réflexe est de demander aux gens de travailler plus vite. La VSM montre que cela porte sur les 10 % du temps où l'on travaille — et laisse intacts les 90 % où l'on attend. **Diviser par deux le temps de développement d'une fonctionnalité qui met trois mois à sortir ne fait gagner que quelques jours.**

C'est la traduction concrète du principe [optimiser l'ensemble]({{< relref "philosophie/philosophie_lean/lean_software_development/les_six_autres" >}}) : l'optimisation locale de chaque étape ne dit rien du délai de bout en bout.

## En pratique

1. **Choisir un élément représentatif** — une fonctionnalité type, pas un cas exceptionnel.
2. **Cartographier les étapes réelles**, pas le processus officiel. C'est le principe du [gemba]({{< relref "philosophie/philosophie_lean/toyota_production_system/vocabulaire" >}}) : on va voir comment le travail se fait vraiment.
3. **Noter les deux temps** à chaque étape, ainsi que les allers-retours (une correction après relecture est du retravail, pas une étape).
4. **Calculer le ratio**, et attaquer les plus grosses attentes — pas les plus grosses charges de travail.

Les métriques [DORA]({{< relref "pratiques/devops/dora/dora_core/metriques" >}}), en particulier le *lead time for changes*, mesurent en continu ce qu'une VSM photographie à un instant donné.

[^1]: Karen Martin and Mike Osterling "Value Stream Mapping: How to Visualize Work and Align Leadership for Organizational Transformation"
