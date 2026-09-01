+++
title = "Le contexte : à quoi l'agilité répond"
description = "Les hypothèses du cycle en cascade, pourquoi elles ont cessé de tenir avec l'essor d'Internet, et ce que disent les chiffres du CHAOS Report."
weight = 10
+++

L'agilité n'est pas née d'une envie de faire autrement. Elle est née d'un constat d'échec, dans un contexte industriel précis. Cette page pose ce décor ; les pages suivantes détaillent chacune des raisons qui en découlent.

## Cascade

> [!danger] Définition
>  Le cycle en cascade se caractérise par des phases séquentielles, qui se succèdent après la
>  validation des livrables de la phase précédente.

La méthodologie Waterfall a largement été utilisée pour créer des logiciels. Elle suppose :

- une connaissance parfaite avant même de commencer
- que tout au long du développement le périmètre reste inchangé
- qu'on ne changera pas de direction au cours du développement
- les changements sont supposés être minimes
- de tout planifier en amont

La méthode Waterfall avait pour but de garantir que le produit final correspond à ce qui avait
été spécifié au départ. Cette approche fonctionnait bien sur des applications complexes et
monolithiques qui exigeaient de la discipline et des résultats clairs (année 70).

> [!ressource] Ressources
> - À lire d'abord : [Le modèle en Cascade]({{< relref "naissance_agile/methodologie_waterfall/index" >}}) — ce que Royce a réellement écrit, et pourquoi le modèle qu'on lui attribue n'est pas le sien
> - [Pourquoi Waterfall échoue ?]({{< relref "naissance_agile/methodologie_waterfall/echec_waterfall" >}})

Remarquons que ces cinq hypothèses ne sont pas *fausses en soi*. Elles décrivent parfaitement un projet dont le besoin est stable et connu — et [il en existe encore]({{< relref "naissance_agile/methodologie_waterfall/quand_waterfall" >}}). Le problème est qu'on les a appliquées à des projets où elles ne tenaient plus.

## Le pivot vers la philosophie Agile

Le développement massif d'Internet a permis l'émergence de nombreuses petites entreprises
qui créaient des applications web. Les équipes de développement de ces sociétés commençaient à remettre en question la méthodologie Waterfall et cherchaient des moyens d'être plus efficaces.

Ayant une structure organisationnelle et un projet moins complexe qu'une entreprise "Legacy System", elles pouvaient donc être à l'écoute et **répondre plus rapidement aux besoins du client.**

Les développeurs ont commencé à rejeter la planification de bout en bout et les spécifications
prédéfinies. Nous sommes à la naissance de l'agilité :
- Un produit ne peut pas être entièrement spécifié au départ.
- L'économie est trop dynamique : l'adaptation du processus s'impose.
- Accepter les changements d'exigences, c'est donner un avantage compétitif au client.

Ce sont exactement les deux premières raisons de ce chapitre : [encaisser l'incertitude]({{< relref "encaisser_incertitude" >}}) et [encaisser le changement]({{< relref "encaisser_changement" >}}).

> [!affirmation] Affirmation
> Ce qui a changé, ce n'est pas la difficulté de construire un logiciel. C'est la vitesse à laquelle le besoin auquel il répond se périme.

## Quelques chiffres

Une étude menée en 1995 nous révèle que :
- 16 % des logiciels sont finis dans les temps et le budget alloué
- 31 % sont abandonnés
- 53 % dépassent le coût et/ou le délai

C'est dans un contexte de gaspillage et de transformation du numérique qu'en 2001 une
équipe d'experts se réunit afin de rédiger le [Manifeste Agile]({{< relref "philosophie/philosophie_agile/manifeste" >}}).

Depuis, The Standish Group publie annuellement le CHAOS Report qui regroupe un ensemble
de statistiques sur les projets informatiques. Par exemple en 2015, on dénombrait 29 % des projets finis en temps/budget, 19 % abandonnés et 52 % connaissaient des dépassements de
coût/délais.

> [!warning] À lire avec prudence
> Le CHAOS Report est régulièrement critiqué : sa définition du « succès » repose sur le respect du triangle *périmètre / coût / délai*, c'est-à-dire précisément le critère prédictif que l'agilité conteste. Un projet livré en retard mais qui a trouvé son marché y est compté comme un échec. Ces chiffres décrivent donc bien un malaise réel, mais ils le mesurent avec la règle de l'ancien monde. Voir à ce sujet [Output vs Outcome]({{< relref "philosophie/pourquoi_agile/produire_valeur/output_vs_outcome" >}}).
