+++
title = "7. Produire de la valeur"
linkTitle = "Produire de la valeur"
description = "Ce qu'est la valeur dans un projet logiciel, pourquoi elle ne se confond pas avec le volume livré, et comment une équipe peut en discuter concrètement."
weight = 90
+++

> [!ressource] Ressources
> - [Value is What You Like](https://ronjeffries.com/xprog/articles/value-is-what-you-like/) — Ron Jeffries
> - [An Agile focus on value](https://agilealliance.org/an-agile-focus-on-value/) — Agile Alliance

Lorsqu'on parle d'Agile, on parle de créer de la valeur mais que cela signifie-t-il ?

## C'est quoi la valeur ?

Selon [Ron Jeffries](https://ronjeffries.com/xprog/articles/value-is-what-you-like/) :

> Choosing value is choosing what matters, to you.

La définition est volontairement décevante, et c'est son intérêt : **la valeur n'est pas une propriété du logiciel, c'est un jugement porté par quelqu'un.** Il n'existe donc pas de mesure objective de la valeur d'une fonctionnalité — seulement des points de vue qu'il faut expliciter.

Ce qui déplace la question. Elle ne devient pas *combien vaut cette story ?*, mais **pour qui, et pourquoi ?** Une story dont personne ne peut nommer le bénéficiaire n'a pas une valeur faible : elle a une valeur inconnue.

## Valeur n'est pas volume

C'est la confusion la plus coûteuse du métier. Livrer beaucoup et livrer ce qui compte sont deux choses différentes, et la première est bien plus facile à mesurer que la seconde — ce qui explique pourquoi on continue de la mesurer.

| | Ce qu'on compte | Ce qu'on ignore |
| --- | --- | --- |
| **Output** | Fonctionnalités livrées, story points, tickets fermés | Si quelqu'un s'en sert |
| **Outcome** | Changement de comportement obtenu chez l'utilisateur | — |

Voir [Output vs Outcome]({{< relref "philosophie/pourquoi_agile/produire_valeur/output_vs_outcome" >}}), et [Mesurer la productivité ?]({{< relref "regard_critique/mesurer_productivite/index" >}}) pour ce que cette confusion produit quand elle sert à évaluer des équipes.

> [!affirmation] Affirmation
> Une fonctionnalité livrée dont personne ne se sert n'a pas une valeur nulle : elle a une valeur négative. Il faudra la maintenir, la tester et la porter à chaque migration.

C'est aussi la première catégorie de gaspillage du [Lean Software Development]({{< relref "philosophie/philosophie_lean/lean_software_development/elimine_gaspillage" >}}) : les fonctionnalités superflues.

## Comment écrire la valeur ?

> In Ron Jeffries's [The Card, Conversation, Confirmation]({{< relref "pratiques/user_stories/user_stories_mapping/les_3c" >}}), he proposes that user stories are "social" instead of "documentary" requirements. Consider this an extension of that approach for a question-based, non-linear maturity assessment. It's more about your team's discussions on how to offer more value rather than the questions themselves. [^1]

Grâce aux 3C, l'équipe peut approfondir le sujet pour en développer une compréhension réellement profonde, ce qui facilite l'identification des leviers permettant de générer davantage de valeur.

Deux appuis concrets sur ce site :

- Le **V** d'[INVEST]({{< relref "pratiques/user_stories/rediger_us/stories_invest" >}}) — *Valuable* : une story doit avoir de la valeur pour un utilisateur ou un client, ce qui interdit les stories purement techniques formulées sans bénéficiaire.
- Le **[User Story Mapping]({{< relref "pratiques/user_stories/user_stories_mapping/index" >}})** — en reconstituant le parcours complet, il rend visible la tranche minimale qui a réellement de la valeur pour l'utilisateur, plutôt qu'un empilement de fonctionnalités isolées.

## La valeur se découvre, elle ne se décrète pas

Puisque la valeur est un jugement, elle ne peut pas être établie une fois pour toutes au moment de la priorisation du backlog. Elle est une **hypothèse** — que la [livraison au client]({{< relref "engager_client" >}}) confirme ou infirme.

C'est le lien direct avec les deux premières raisons de ce chapitre : si l'on savait à l'avance ce qui a de la valeur, il n'y aurait ni [incertitude]({{< relref "encaisser_incertitude" >}}) ni besoin d'[encaisser le changement]({{< relref "encaisser_changement" >}}). Priorisation et apprentissage sont le même mouvement.

## Trois angles pour creuser

- [Output vs Outcome]({{< relref "philosophie/pourquoi_agile/produire_valeur/output_vs_outcome" >}}) — la distinction entre ce qu'on livre et ce qu'on obtient, et pourquoi seule la seconde mesure la valeur.
- [Projet VS Produit]({{< relref "philosophie/pourquoi_agile/produire_valeur/projet_vs_produit" >}}) — un projet se termine à une date, un produit se termine quand plus personne ne s'en sert. Ce que ce basculement change pour les équipes et les budgets.
- [Feature > Activités]({{< relref "philosophie/pourquoi_agile/produire_valeur/feature_over_activites" >}}) — découper le travail par fonctionnalité plutôt que par phase, pour que de la valeur existe avant la fin.

[^1]: [An Agile focus on value](https://agilealliance.org/an-agile-focus-on-value/)
