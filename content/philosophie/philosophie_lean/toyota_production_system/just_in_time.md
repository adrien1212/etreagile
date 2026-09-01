+++
title = "Just-in-time"
description = "Le juste-à-temps : produire ce qui est nécessaire, au moment où c'est nécessaire, et dans la quantité nécessaire — et le flux tiré qui le rend possible."
weight = 20
+++

> [!ressource] Ressources
> - [Comprendre le TPS #2 : le JAT (ou Juste-à-temps)](https://blog.toyota-forklifts.fr/tps-jat-juste-a-temps-production-demande)
> - Taiichi Ohno, *Toyota Production System: Beyond Large-Scale Production* (1978)
> - Donald Reinertsen, *The Principles of Product Development Flow* (2009)

> [!definition] Définition
> Faire ce qui est nécessaire, seulement lorsque c'est nécessaire, et seulement dans la quantité qui est nécessaire.

Le juste-à-temps est le second pilier du TPS, avec le [Jidoka]({{< relref "philosophie/philosophie_lean/toyota_production_system/jidoka" >}}). Son objectif n'est pas d'aller plus vite : c'est de **ne rien produire qui ne soit immédiatement utile**.

## Flux poussé, flux tiré

Toute la différence tient là, et c'est le mécanisme le plus mal compris du Lean.

| | Flux poussé (*push*) | Flux tiré (*pull*) |
| --- | --- | --- |
| **Ce qui déclenche le travail** | Une prévision, un plan | Une demande réelle de l'étape suivante |
| **Ce qui règle le rythme** | La capacité de chaque poste | La consommation en aval |
| **Ce qui s'accumule** | Du stock entre les étapes | Rien : on ne produit que sur appel |
| **En cas de problème** | On continue, le stock absorbe | Tout s'arrête, le problème est visible |

En **flux poussé**, chaque étape produit à son rythme maximal et pousse le résultat vers la suivante. Chacun est occupé en permanence, ce qui donne une impression d'efficacité — mais le travail s'entasse entre les postes, et un défaut peut se répliquer des centaines de fois avant d'être détecté.

En **flux tiré**, rien n'est produit tant que l'aval n'en a pas besoin. C'est le rôle historique du *kanban* : une étiquette qui remonte de l'étape suivante pour dire « j'ai consommé, refais-en un ». Le mot a donné son nom au [framework Kanban]({{< relref "frameworks/framework_kanban/index" >}}).

> [!affirmation] Affirmation
> En flux tiré, une équipe occupée à 100 % du temps n'est pas un objectif — c'est un symptôme. Cela signifie qu'elle produit sans attendre la demande, donc qu'elle constitue du stock.

## Ce que cela donne en développement logiciel

Le « stock » d'une équipe logicielle est invisible, ce qui le rend redoutable. Il prend la forme de :

- spécifications écrites et pas encore développées ;
- code écrit et pas encore intégré ;
- fonctionnalités terminées et pas encore mises en production ;
- tickets en attente de revue.

Tout cela est du travail déjà payé qui ne rapporte encore rien, et qui **se périme** : plus une spécification attend, plus le besoin qu'elle décrit a eu le temps de changer. C'est le premier gaspillage identifié par les Poppendieck, le [travail partiellement terminé]({{< relref "philosophie/philosophie_lean/lean_software_development/elimine_gaspillage" >}}).

Trois pratiques agiles sont des applications directes du juste-à-temps :

- **La limitation du travail en cours** — la [limite de WIP]({{< relref "frameworks/framework_kanban/principes" >}}) de Kanban est littéralement un mécanisme de flux tiré : on ne démarre une tâche que si une place se libère.
- **Le refinement au dernier moment responsable** — on détaille une [user story]({{< relref "pratiques/user_stories/rediger_us/quand_us" >}}) juste avant de la prendre, pas six mois avant.
- **Le déploiement continu** — livrer par petits lots fréquents plutôt que d'accumuler des fonctionnalités pour une grosse mise en production.

## Pourquoi cela va avec le Jidoka

Supprimer le stock a une conséquence brutale : **il n'y a plus rien pour amortir un problème**. Un défaut n'est plus absorbé par un tampon, il arrête immédiatement le flux.

C'est voulu. Le juste-à-temps ne se contente pas de réduire les coûts de stockage : il **rend les problèmes impossibles à ignorer**. Mais cela n'est tenable que si l'organisation sait les traiter à la source — ce qui est exactement l'objet du Jidoka.

> [!danger] L'erreur classique
> Adopter le juste-à-temps pour réduire les stocks, sans se doter des moyens de résoudre les problèmes qu'il fait apparaître. On obtient alors une chaîne qui s'arrête sans arrêt, et l'on conclut que « le Lean ne marche pas chez nous ». En logiciel : baisser les limites de WIP sans traiter les blocages que cela révèle.
