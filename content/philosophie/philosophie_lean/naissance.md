+++
title = "Naissance du Lean"
description = "De l'atelier de tissage de Sakichi Toyoda au logiciel : comment le Toyota Production System est né d'une contrainte, puis a été renommé « Lean » par l'Occident."
weight = 5
+++

> [!ressource] Ressources
> - Taiichi Ohno, *Toyota Production System: Beyond Large-Scale Production* (1978, traduit en anglais en 1988)
> - [Toyota — Origines du TPS](https://global.toyota/en/company/vision-and-philosophy/production-system/)
> - [A Brief History of Lean](https://www.lean.org/explore-lean/a-brief-history-of-lean)
> - [Lean Thinking: A Look Back and a Look Forward](https://www.lean.org/the-lean-post/articles/lean-thinking-a-look-back-and-a-look-forward)

Le Lean n'a pas été conçu comme une méthode. Il est né d'une **contrainte** — celle d'un constructeur japonais trop pauvre pour copier l'Amérique — puis a été observé, nommé et exporté par des chercheurs occidentaux quarante ans plus tard.


## NUMMI

En 1984, General Motors et Toyota ouvrent une usine commune en Californie, **NUMMI**. GM y rouvre une usine qu'il avait fermée pour cause de conflits sociaux et de qualité désastreuse, avec en grande partie **les mêmes ouvriers** — et le système de production de Toyota.

En deux ans, l'usine devient l'une des meilleures du groupe. La démonstration est difficile à contester : le problème n'était pas les gens, c'était le système. Le site revient sur cet épisode à propos du [changement de culture organisationnelle]({{< relref "equipe_agile/culture/index" >}}).

## Le mot « Lean »

Le MIT lance un vaste programme de recherche comparative sur l'industrie automobile mondiale. En 1988, **John Krafcik** — jeune chercheur, ancien ingénieur de NUMMI — publie un article qui baptise ce qu'il observe : *lean production*, la production « au plus juste », par opposition à la production de masse.

Deux ans plus tard, **Womack, Jones et Roos** publient *The Machine That Changed the World* (1990), qui diffuse le terme dans le monde entier.

> [!definition] Un nom donné de l'extérieur
> Toyota n'a jamais appelé son système « Lean ». Le mot est une **étiquette occidentale** posée sur ce que des chercheurs ont su observer. Ce qu'ils ont bien décrit, ce sont les outils et les flux ; ce qui s'est perdu en route, c'est souvent la partie la moins visible — la formation quotidienne des gens à la résolution de problèmes, et le [respect des personnes]({{< relref "philosophie/philosophie_lean/lean_software_development/les_six_autres" >}}).

## 1996-2003 — Du plancher d'usine au logiciel

- **1996** — Womack et Jones publient *Lean Thinking* et généralisent hors de l'automobile, autour de cinq principes : identifier la **valeur**, cartographier la **chaîne de valeur**, créer le **flux**, le faire **tirer** par le client, viser la **perfection**.


> We described this thought process in The Machine That Changed the World (1990). In a subsequent volume, Lean Thinking (1996), Dan Jones and I distilled these lean principles even further to five:
>    - Specify the value desired by the customer.
>    - Identify the value stream for each product providing that value and challenge all of the wasted steps (generally nine out of ten) currently necessary to provide it.
>    - Make the product flow continuously through the remaining, value-creating steps.
>    - Introduce pull between all steps where continuous flow is impossible.
>    - Manage toward perfection so that the number of steps and the amount of time and information needed to serve the customer continually falls. [^1]


- **2001** — Toyota formalise en interne *The Toyota Way*, articulé autour de deux piliers : amélioration continue et respect des personnes. La même année, à l'autre bout du monde, dix-sept développeurs signent le [Manifeste Agile]({{< relref "philosophie/philosophie_agile/manifeste" >}}).
- **2003** — **Mary et Tom Poppendieck** publient *Lean Software Development: An Agile Toolkit* et transposent l'ensemble au développement logiciel. C'est l'objet du chapitre [Lean Software Development]({{< relref "philosophie/philosophie_lean/lean_software_development/index" >}}).

## La question que pose le Lean

Tout ce qui précède se résume à un déplacement de question, et c'est ce déplacement qui rend le Lean pertinent bien au-delà de l'automobile.

La gestion de projet classique demande : **comment planifier le travail, et comment tenir le plan ?** Le Lean ne répond pas à cette question — il en pose une autre :

> [!affirmation] La question du Lean
> **Comment améliorer continuellement le système qui transforme une idée en valeur pour le client ?**

La différence est de nature. La première question porte sur un projet, avec un début et une fin ; on y réussit en respectant des prévisions. La seconde porte sur un **système de création de valeur**, qui persiste d'un projet à l'autre ; on y progresse en réduisant, encore et encore, le temps et le gâchis entre l'idée et son usage.

### Sur un projet logiciel

Prenons une chaîne classique :

> Besoin → conception → développement → revue → tests → déploiement → utilisateur

Là où la conduite de projet planifie chaque étape et suit son avancement, le Lean regarde **ce qui circule entre elles**. Il pose alors ses questions :

| La question | Où elle est traitée |
| --- | --- |
| Qu'est-ce qui crée réellement de la valeur pour l'utilisateur ? | [Produire de la valeur]({{< relref "philosophie/pourquoi_agile/produire_valeur/index" >}}) |
| Où attend-on ? | [Value Stream Map]({{< relref "philosophie/philosophie_lean/value_stream_map" >}}) |
| Où accumule-t-on du travail ? | [Juste-à-temps et flux tiré]({{< relref "philosophie/philosophie_lean/toyota_production_system/just_in_time" >}}) |
| Où réalise-t-on du travail inutile ? | [Éliminer le gaspillage]({{< relref "philosophie/philosophie_lean/lean_software_development/elimine_gaspillage" >}}) |
| Pourquoi les défauts sont-ils découverts si tard ? | [Jidoka]({{< relref "philosophie/philosophie_lean/toyota_production_system/jidoka" >}}) |
| Comment raccourcir la boucle entre réalisation et feedback ? | [Livrer vite]({{< relref "philosophie/philosophie_lean/lean_software_development/les_six_autres" >}}) |

Aucune de ces questions ne porte sur la vitesse des gens. Toutes portent sur **le système dans lequel ils travaillent** — ce qui est exactement le principe d'[optimiser l'ensemble]({{< relref "philosophie/philosophie_lean/lean_software_development/les_six_autres" >}}).

> [!definition] Pourquoi cela dépasse le projet
> Un système ne s'améliore que s'il dure. C'est la raison pour laquelle le Lean s'accommode mal d'équipes constituées puis dissoutes à chaque affaire : il n'y a alors personne pour capitaliser sur ce qui a été appris. Voir [Projet VS Produit]({{< relref "philosophie/pourquoi_agile/produire_valeur/projet_vs_produit" >}}).


[^1]: https://www.lean.org/the-lean-post/articles/lean-thinking-a-look-back-and-a-look-forward