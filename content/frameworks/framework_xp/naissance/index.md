+++
title = "Naissance de XP"
description = "XP naît en 1996 sur le projet C3 de Chrysler, d'une idée simple : pousser au maximum les pratiques dont on sait déjà qu'elles fonctionnent."
weight = 5
+++

> [!ressource] Ressources
> - Extreme Programming Explained: Embrace Change - Kent Beck (première édition)
> - Scaling Software Agility - C3 The essence of XP
> - [XP Revisited - Ron Jeffries](https://ronjeffries.com/articles/018-01ff/xp-revisited-1/)
> - [Extreme Programming: A gentle introduction](http://www.extremeprogramming.org/)

## Le problème de départ : le coût du changement

XP ne naît pas d'une insatisfaction vis-à-vis de la gestion de projet, mais d'un constat technique.

Dans une approche classique, plus le projet avance, plus une modification coûte cher. Cette courbe justifie à elle seule de tout spécifier avant de construire — et donc le [cycle en cascade]({{< relref "naissance_agile/methodologie_waterfall/index" >}}). Le pari de XP est que cette courbe n'est pas une fatalité : avec les bonnes pratiques de conception et de programmation, on peut la garder suffisamment plate pour que le changement reste abordable jusqu'à la fin.

Tout le reste de XP découle de ce pari. Voir [Coût du changement]({{< relref "philosophie/pourquoi_agile/produit_haute_qualite/qualite_logicielle/cout_changement" >}}).

## Le projet C3 chez Chrysler

XP se formalise sur un projet réel : **C3**, pour *Chrysler Comprehensive Compensation System*, un système de paie développé en Smalltalk.

Le projet est en difficulté lorsque **Kent Beck est appelé en 1996**, initialement pour des problèmes de performance. Il finit par reprendre la conduite du projet, fait venir **Ron Jeffries** comme coach à plein temps, et met en place — en les nommant — les pratiques qui formeront XP. Le système entre en production en **1997** et paie plusieurs milliers de salariés du groupe.

C'est de cette expérience que sort *Extreme Programming Explained*, publié en **1999**.

> [!danger] Le projet a été arrêté
> C3 est **annulé en 2000**, sans avoir été étendu à l'ensemble des salariés du groupe. Il serait malhonnête de raconter la naissance de XP sans le dire.
>
> Ce qui a été abandonné, c'est le projet — pas les pratiques. Elles ont survécu à leur terrain d'origine et irriguent aujourd'hui le développement moderne, le craft et le DevOps. Mais ce dénouement rappelle qu'un bon jeu de pratiques techniques ne protège pas d'un arbitrage budgétaire ou politique.

## Pourquoi « extreme » ?

Le nom prête à confusion : on y entend souvent une radicalité, voire une provocation. L'idée de Beck est plus simple, et beaucoup plus utile à retenir.

XP n'invente presque aucune pratique. Il prend des pratiques dont la profession sait déjà qu'elles fonctionnent, et **pousse les curseurs au maximum** : si c'est bon, pourquoi le faire à petite dose ?

| Ce que la profession sait déjà | Le curseur poussé à fond |
| :--- | :--- |
| La relecture de code améliore la qualité | On relit **en permanence** → programmation en binôme |
| Les tests détectent les régressions | On teste **avant même d'écrire le code** → TDD |
| Intégrer tôt évite les mauvaises surprises | On intègre **plusieurs fois par jour** → intégration continue |
| Une conception soignée facilite l'évolution | On conçoit **en continu** → conception simple et refactoring |
| Les itérations courtes réduisent le risque | On livre **toutes les une à deux semaines** → petites livraisons |
| Le client sait ce qu'il veut, en partie | Il est **dans la pièce** → client sur site |

Lu ainsi, XP cesse d'être une liste de douze règles à mémoriser : c'est une même décision appliquée six fois. Voir [Pratiques]({{< relref "frameworks/framework_xp/pratiques" >}}).

## XP précède le Manifeste

Dernier point de repère chronologique, souvent inversé : XP (1995-1999) et [Scrum]({{< relref "frameworks/framework_scrum/naissance/index" >}}) (1993-1995) sont **antérieurs** au Manifeste Agile de 2001. Kent Beck et Ron Jeffries en sont d'ailleurs deux des signataires.

L'agilité ne les a pas produits : ce sont eux qui l'ont produite. Voir [XP, Scrum,... précèdent Agile]({{< relref "naissance_agile/framework_avant_agile" >}}).

## XP influence
> [!ressource] Ressources
> - [Pourquoi Extreme Programming est moins populaire que Scrum ?](https://youtu.be/T1d8bfez5yA)

L'Extreme Programming est une méthode agile qui a beaucoup influencé le Scrum et l'approche Devops. Si l'Extreme Programming ne fait plus parler de lui, il est au final de plus en plus présent par bien des aspects au sein de nos organisations.
- XP et Scrum fonctionnent sur les mêmes principes : *incrémental*, *itératif*, *adaptatif*
- Malgré des philosophies différentes, XP a posé les bases du développement logiciel "moderne" en définissant un ensemble de pratiques.