+++
title = "Pourquoi le Lean ?"
description = "Réduire le gaspillage, limiter les surcoûts liés à la non-qualité : les raisons de s'intéresser au Lean en développement logiciel."
weight = 20
+++

> [!ressource] Ressources
> - [Lean vs TPS](https://www.allaboutlean.com/tps-and-lean/)
> - [Difference between Toyota Production System (TPS) and Lean](https://www.linkedin.com/pulse/difference-between-toyota-production-system-tps-lean-boris-hodak/)

On s’intéresse au Lean pour les raisons suivantes

> [!definition] TPS ou Lean ?
> Les deux ressources ci-dessus portent sur une distinction utile, détaillée dans [Naissance du Lean]({{< relref "philosophie/philosophie_lean/naissance" >}}) : le **TPS** est le système réel de Toyota, le **Lean** est le nom que l'Occident lui a donné en 1988.
>
> La conséquence est pratique : le Lean qu'on achète en formation est une **modélisation** du TPS, et il en manque souvent la partie la plus difficile à exporter — le [respect des personnes]({{< relref "philosophie/philosophie_lean/lean_software_development/les_six_autres" >}}) et la formation quotidienne à la résolution de problèmes.

## Réduire le gaspillage
> [!affirmation] Affirmation
>  Les managers créent de la valeur, mais également du gaspillage
- Regarder les éléments qui ont permis à l’équipe de créer de la valeur
- Regarder les éléments qui ont empêché l’équipe de créer de la valeur

### Surcoût et non-qualité

Il y a un lien étroit entre l’augmentation du coût du logiciel et sa non-qualité. Corriger, maintenir, recommencer des "bêtises" vont entraîner des surcoûts.

Il est très difficile de l’éliminer complètement, il y aura toujours des erreurs mais l’objectif
est de minimiser ce taux. Ainsi avec Lean, on va essayer de comprendre notre process de
travail afin de l’améliorer et d’être plus efficace.

- Pourquoi ici on a mis 1 mois tandis que sur une fonctionnalité similaire on a mis 1
semaine ?
- Quels sont les gaspillages qui nous ont empêchés de recommencer.

> L’approche Lean cherche à faire mieux avec ce qu’on a.

Cette amélioration par petits pas, menée par ceux qui font le travail, porte un nom : le **kaizen**. Voir [Vocabulaire du Lean]({{< relref "philosophie/philosophie_lean/toyota_production_system/vocabulaire" >}}).

## Responsabiliser à la résolution de problème
> [!affirmation] Affirmation
>  On veut responsabiliser les développeurs (et non-exécutant) à la résolution de problème
>  tout en satisfaisant les clients et en étant rentable.

Pour ce faire on va :
- dire aux gens ce qui est nécessaire pour le client maintenant en créant un flux [tiré]({{< relref "philosophie/philosophie_lean/toyota_production_system/just_in_time" >}}) (Kanban).
- et ce flux permet de soulever les problèmes (e.g. WIP max atteinte)
- 
⇒ Les équipes deviennent donc autonomes pour soulever le problème et essayer de le résoudre (le rôle des managers est d’accompagner les équipes à surmonter ce problème).

> [!definition] Définition
> Au final le Lean se décrit ainsi :
> - Le *Pourquoi ?* : satisfaire les clients
> - Le *Comment ?* : développer les gens à la résolution de problème pour faire face à des situations inattendues
> - Le *Quoi ?* : mise en place d’outils à flux tiré pour visualiser les problèmes avec des managers qui passent d’une chaine de contrôle à une chaine d’aide
