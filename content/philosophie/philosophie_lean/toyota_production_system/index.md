+++
title = "Toyota Production System"
description = "Le Toyota Production System, ses deux piliers — Jidoka et juste-à-temps — et les fondations sur lesquelles ils reposent."
weight = 15
+++

> [!ressource] Ressources
> - Taiichi Ohno, *Toyota Production System: Beyond Large-Scale Production* (1978)
> - [Le site officiel Toyota — Toyota Production System](https://global.toyota/en/company/vision-and-philosophy/production-system/)
> - Jeffrey Liker, *The Toyota Way* (2004)

## D'où cela vient

Le TPS est l'œuvre de **Taiichi Ohno**, ingénieur puis directeur chez Toyota, à partir des années 1950. Le contexte compte pour comprendre le système : le Japon d'après-guerre manque de capitaux, de matières premières et de place. Toyota ne peut pas copier Ford, dont le modèle repose sur de très grandes séries et donc sur des stocks importants.

Ohno construit alors un système qui fait de cette contrainte un principe : **produire en petites quantités, sans stock, et rendre tout problème immédiatement visible**. Ce qui était une nécessité économique s'est révélé être un avantage — c'est ce que les chercheurs occidentaux découvriront trente ans plus tard.

Le détail de cette histoire, du métier à tisser de 1924 jusqu'à l'invention du mot « Lean » en 1988, est raconté dans [Naissance du Lean]({{< relref "philosophie/philosophie_lean/naissance" >}}).

![TPS](tps.png)

## Les deux piliers

TPS est basé sur deux principaux piliers conceptuels :

- [Jidoka]({{< relref "philosophie/philosophie_lean/toyota_production_system/jidoka" >}}) : (Autonomation), signifiant « automatisation avec une touche d'humain ». **On arrête dès qu'un problème apparaît**, pour ne jamais transmettre un défaut à l'étape suivante.
- [Juste-à-temps]({{< relref "philosophie/philosophie_lean/toyota_production_system/just_in_time" >}}) : dans le sens de « faire ce qui est nécessaire, seulement lorsque c'est nécessaire, et seulement dans la quantité qui est nécessaire ».

> [!definition] Pourquoi deux piliers et pas un
> Les deux se tiennent mutuellement. Le juste-à-temps supprime les stocks, donc **plus rien n'amortit un défaut** : un problème arrête aussitôt toute la chaîne. Sans Jidoka pour traiter les problèmes à la source, le juste-à-temps serait intenable. Inversement, sans juste-à-temps, les stocks masqueraient les problèmes et le Jidoka n'aurait jamais rien à détecter.
>
> C'est l'image classique du Lean : **baisser le niveau de l'eau pour faire apparaître les rochers**. Le stock, c'est l'eau.

## Les fondations

On représente souvent le TPS comme une maison : les deux piliers portent le toit (qualité, coût, délai), mais ils reposent sur des fondations sans lesquelles ils s'effondrent.

| Fondation | Ce qu'elle apporte |
| --- | --- |
| **Standardisation** | Sans standard, il n'y a pas d'écart observable — donc rien à améliorer |
| **Heijunka** (lissage) | Répartir la charge pour éviter les à-coups, qui produisent surcharge et gaspillage |
| **Kaizen** (amélioration continue) | Le mécanisme par lequel les standards évoluent |
| **Respect des personnes** | Ce sont ceux qui font le travail qui détectent et résolvent les problèmes |

Ces termes, et quelques autres qu'on rencontre partout dans la littérature agile, sont réunis dans la page [Vocabulaire du Lean]({{< relref "philosophie/philosophie_lean/toyota_production_system/vocabulaire" >}}).

> [!affirmation] Affirmation
> Reprendre les outils du TPS sans ses fondations donne ce que l'Institut Lean France appelle du fordisme déguisé : de l'optimisation imposée d'en haut, sans les gens qui font le travail.
