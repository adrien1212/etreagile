+++
title = "1. Encaisser l'incertitude"
linkTitle = "Encaisser l'incertitude"
description = "Accepter qu'on ne peut pas tout savoir au départ d'un projet, et organiser le travail pour apprendre au lieu de deviner."
weight = 30
+++

> [!ressource] Ressources
> - [The New Methodology - The Unpredictability of Requirements](https://www.martinfowler.com/articles/newMethodology.html#TheUnpredictabilityOfRequirements)
> - [The New Methodology - Is Predictability Impossible?](https://www.martinfowler.com/articles/newMethodology.html#IsPredictabilityImpossible)
> - Scaling Software Agility - p26

## Le constat

> [!affirmation] Affirmation
>  Il s'agit d'accepter une réalité et de comprendre que dans le développement logiciel tout
>  n'est pas prévisible.

Deux incertitudes, et non une seule, pèsent sur un projet logiciel.

**L'incertitude sur le besoin** — on ne sait pas exactement ce qu'il faut construire :

> We do not assume that we, or our customers, can fully understand all the requirements, or that anyone can possibly understand them all up front. [^1]

**L'incertitude sur la solution** — même en connaissant le besoin, on ne sait pas exactement combien coûtera sa réalisation :

> We do not assume that we can develop new, state-of-the-art, unproven, innovative, and risk-laden software projects on a fixed-functionality and fixed-schedule basis. Indeed, we assume that we cannot. Instead, we assume that we can deliver the most important features to our customer earlier, rather than later, than the customer might have expected. In so doing, we can get immediate feedback on whether we are building the right solution. [^1]

Chaque projet est une nouvelle expérience où il est très difficile de se mettre d'accord une
fois pour toutes avec le client.

## Incertitude n'est pas risque

Ces deux mots sont souvent employés l'un pour l'autre, alors qu'ils n'appellent pas la même réponse.

| | Définition | Réponse |
| --- | --- | --- |
| **Risque** | Un événement identifié, dont on peut estimer la probabilité et l'impact | On l'anticipe : plan de secours, provision, assurance |
| **Incertitude** | On ne sait pas encore quelles sont les questions à poser | On l'explore : on apprend, on mesure, on ajuste |

Le réflexe prédictif consiste à traiter toute incertitude comme un risque : puisqu'on ne sait pas, on planifie davantage et on spécifie plus finement. C'est l'erreur. **On ne réduit pas une incertitude en écrivant un document plus long, on la réduit en produisant quelque chose et en l'observant.**

## Comment l'agilité s'y prend

Là où avec Waterfall on spécifiait l'ensemble du produit dès le début, avec Agile nous savons qu'il est impossible d'éliminer toute l'incertitude dès le début du projet. On l'accepte, puis on la fait décroître **par le travail réel** plutôt que par l'analyse préalable.

![reduire incertitude](reduire_incertitude.png)

> We need an honest feedback mechanism which can accurately tell us what the situation is at frequent intervals. The key to this feedback is iterative development [^2]

Trois leviers concrets :

- **L'itération** — chaque cycle court transforme une hypothèse en fait observé. C'est le sens du cycle de vie itératif, détaillé dans [Les quatre cycles de vie]({{< relref "philosophie/pourquoi_agile/encaisser_incertitude/cycles_de_vie" >}}).
- **L'empirisme** — décider à partir de ce qui est constaté, pas de ce qui était prévu. C'est très exactement le fondement des [trois piliers de Scrum]({{< relref "frameworks/framework_scrum/piliers/index" >}}) : transparence, inspection, adaptation.
- **La réduction de la taille des lots** — plus le lot livré est petit, plus tôt arrive l'information, et moins coûteuse est l'erreur.

En acceptant l'incertitude, on accepte également l'idée du changement :
- dans le périmètre du besoin
- dans la planification
- dans l'organisation de l'équipe

⇒ On s'adapte aux imprévus. En s'appuyant sur le **feedback**, **l'expérience** et le **constat**. Nous
optons pour une **démarche itérative et d'amélioration continue**.

## Ce que cela change pour l'estimation

Si l'incertitude est réelle, alors une estimation donnée en début de projet ne peut pas être un engagement — c'est une hypothèse datée, qui doit être révisée à mesure qu'on apprend.

C'est la raison pour laquelle l'agilité [estime en taille relative plutôt qu'en heures]({{< relref "pratiques/user_stories/user_story_points/pourquoi_usp" >}}), et pourquoi la question *[a-t-on seulement besoin d'estimer ?]({{< relref "regard_critique/estimer" >}})* reste ouverte.

> [!danger] Le contresens fréquent
> « Accepter l'incertitude » n'autorise pas à ne rien prévoir. C'est l'inverse : parce que l'avenir est incertain, on planifie **plus souvent**, à des horizons différents, plutôt qu'une seule fois au début. Voir [Les 5 niveaux de planification]({{< relref "pratiques/planifier/niveau_planification/index" >}}) et [A-t-on besoin de planifier ?]({{< relref "regard_critique/planifier/index" >}}).

## Pour aller plus loin

Le mécanisme par lequel on absorbe l'incertitude porte un nom : le **cycle de vie**. Deux pages le détaillent.

- [Les quatre cycles de vie]({{< relref "philosophie/pourquoi_agile/encaisser_incertitude/cycles_de_vie" >}}) — prédictif, itératif, incrémental, et leur combinaison. Ce qui distingue *refaire* de *ajouter*, et pourquoi confondre les deux coûte cher.
- [Le cycle de vie Agile]({{< relref "philosophie/pourquoi_agile/encaisser_incertitude/cycle_de_vie_agile" >}}) — comment les frameworks combinent les deux, sous forme d'itérations de durée fixe (Scrum) ou de flux continu (Kanban).

[^1]: Scaling Software Agility - p26
[^2]: [The New Methodology](https://www.martinfowler.com/articles/newMethodology.html#IsPredictabilityImpossible)
