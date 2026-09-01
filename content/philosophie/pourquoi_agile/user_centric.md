+++
title = "4. Remettre l'humain au centre"
linkTitle = "L'humain au centre (user-centric)"
description = "L'agilité replace deux catégories d'humains au centre du processus : celui qui utilise le produit, et ceux qui le construisent."
weight = 60
+++

> [!ressource] Ressources
> - [Le Manifeste Agile]({{< relref "philosophie/philosophie_agile/manifeste" >}}) — valeur 1 et principe 1
> - [Dimension humaine]({{< relref "equipe_agile/dimension_humaine" >}})
> - The New New Product Development Game — Takeuchi & Nonaka (1986)

Le mot *humain* désigne ici **deux populations distinctes**, et l'agilité les remet toutes les deux au centre. Les confondre est la source de beaucoup de malentendus : une organisation peut être très attentive à ses utilisateurs et très maltraitante pour ses équipes, ou l'inverse.

## L'utilisateur au centre du produit (*user-centric*)

Le premier principe du Manifeste ne parle pas de méthode, il parle de destinataire :

> Notre plus haute priorité est de satisfaire le client en livrant rapidement et régulièrement des fonctionnalités à grande valeur ajoutée.

Dans une conduite prédictive, l'utilisateur intervient deux fois : au début pour exprimer un besoin, à la fin pour recetter. Entre les deux, il est représenté par un document. **L'agilité remplace ce document par une présence continue.**

Ce que cela change concrètement :

- **On décrit le besoin du point de vue de celui qui l'éprouve.** C'est toute la raison d'être de la [user story]({{< relref "pratiques/user_stories/rediger_us/pourquoi_us" >}}), qui commence par *En tant que…* et non par *Le système doit…*. La formulation n'est pas cosmétique : elle interdit d'écrire une exigence sans nommer son bénéficiaire.
- **On préfère la conversation au document.** Les [3C]({{< relref "pratiques/user_stories/user_stories_mapping/les_3c" >}}) — Card, Conversation, Confirmation — posent que la carte n'est qu'un aide-mémoire, et que la compréhension réelle se construit en parlant.
- **On garde la vision d'ensemble du parcours.** Le [User Story Mapping]({{< relref "pratiques/user_stories/user_stories_mapping/index" >}}) reconstitue l'usage bout en bout, contre la tendance d'un backlog plat à faire perdre de vue ce que l'utilisateur cherche réellement à accomplir.
- **On mesure l'effet, pas le volume.** Livrer vingt fonctionnalités dont personne ne se sert n'est pas un succès : c'est la distinction [output vs outcome]({{< relref "philosophie/pourquoi_agile/produire_valeur/output_vs_outcome" >}}).

> [!affirmation] Affirmation
> Être *user-centric*, ce n'est pas demander à l'utilisateur ce qu'il veut. C'est comprendre ce qu'il essaie de faire — puis vérifier, en lui livrant quelque chose, qu'on avait bien compris.

## Les individus au centre du processus

La toute première valeur du Manifeste ne parle pas des utilisateurs, mais de ceux qui construisent :

> **Les individus et leurs interactions** plus que les processus et les outils

C'est l'affirmation la plus radicale du texte, et la plus souvent trahie. Elle pose qu'aucun processus ne rattrape une équipe qui ne se parle pas, et qu'à l'inverse une équipe qui se parle bien réussira avec un processus imparfait.

Trois conséquences documentées ailleurs sur ce site :

- **Un développeur n'est pas un exécutant.** Réduire l'équipe à une capacité de production revient à jeter l'essentiel de ce pour quoi on l'a recrutée : voir [Développeurs VS Exécutants]({{< relref "equipe_agile/roles_postures/developpeur_executant/index" >}}).
- **La sécurité psychologique conditionne la performance.** L'étude Aristote de Google l'a établi : ce qui distingue les équipes efficaces n'est pas *qui* en fait partie, mais la manière dont leurs membres interagissent. Voir [Psychological Safety]({{< relref "equipe_agile/culture/psychological_safety" >}}).
- **Le rythme doit être soutenable.** XP en fait une pratique à part entière : une équipe épuisée produit du travail qu'il faudra refaire.

> [!danger] Le contresens fréquent
> « L'humain au centre » est devenu un argument de communication commode. Il ne se vérifie pas dans les affiches, mais dans les arbitrages : que se passe-t-il quand tenir la date exige de sacrifier la [qualité]({{< relref "produit_haute_qualite" >}}) ou d'imposer des heures supplémentaires ? La réponse à cette question dit ce que l'organisation met réellement au centre.

## Pourquoi les deux vont ensemble

Ce n'est pas un hasard si le Manifeste tient les deux bouts. Une équipe qu'on empêche de comprendre l'usage réel de ce qu'elle produit ne peut pas être *user-centric* : elle n'a accès qu'à des spécifications. Inversement, mettre l'utilisateur au centre suppose de faire confiance aux gens qui lui parlent — donc de leur laisser [la propriété de leur processus]({{< relref "proprietaire_processus" >}}) et de [les engager avec le client]({{< relref "engager_client" >}}).

C'est ce que Takeuchi et Nonaka observaient déjà en 1986 dans les équipes produit les plus performantes, et qui a directement inspiré Scrum : des équipes **transcendantes** (portées par un objectif qui leur appartient), **autonomes** et **pluridisciplinaires**. Voir [Caractéristiques d'une bonne équipe]({{< relref "equipe_agile/constitution_equipe/index" >}}).
