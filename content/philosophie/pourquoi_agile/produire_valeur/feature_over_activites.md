+++
title = "Feature > Activités"
description = "Découper le travail par fonctionnalité plutôt que par activité, pour livrer de la valeur en continu au lieu de la reporter à la fin."
weight = 30
+++

> [!ressource] Ressources
> - [Manage Your Goals Instead of Activities](http://www.agile-process.org/byfeature.html)

L'approche *By Feature* s'oppose à l'approche traditionnelle qui consiste à commencer la phase suivante (e.g le codage) une fois la phase précédente terminée (e.g. le design).

## Les deux façons de découper

Face à un travail trop gros pour être fait d'un bloc, il n'existe que deux façons de le couper.

**Par activité (découpage horizontal)** — on regroupe le travail par nature : toute l'analyse, puis toute la conception, puis tout le développement, puis tous les tests. C'est le découpage du [cycle prédictif]({{< relref "philosophie/pourquoi_agile/encaisser_incertitude/cycles_de_vie" >}}), et il est intuitif : chaque phase rassemble des gens du même métier, qui font la même chose en même temps.

**Par fonctionnalité (découpage vertical)** — on prend un besoin utilisateur et on le traverse de bout en bout : son analyse, sa conception, son code, ses tests. Puis on passe au suivant.

> [!affirmation] Affirmation
> Le découpage horizontal produit des livrables intermédiaires que personne ne peut utiliser. Le découpage vertical produit à chaque étape quelque chose dont quelqu'un peut se servir.

## Pourquoi l'activité retarde toute la valeur

Un découpage par activité a une propriété redoutable : **aucune valeur n'existe avant la toute fin**. Un document de conception complet ne rend service à aucun utilisateur ; une base de données entièrement modélisée non plus. La première chose utilisable apparaît quand la dernière phase se termine.

Trois conséquences en découlent :

- **Le feedback arrive trop tard.** Si l'analyse s'est trompée, on l'apprend à la recette — au moment où corriger coûte le plus cher. C'est exactement ce que l'agilité cherche à éviter en [encaissant l'incertitude]({{< relref "philosophie/pourquoi_agile/encaisser_incertitude/index" >}}) par le feedback.
- **On ne peut rien arrêter.** Un travail découpé par phases est indivisible : impossible de livrer 60 % du périmètre, car ces 60 % ne forment rien d'utilisable. En vertical, on peut s'arrêter après n'importe quelle tranche.
- **On produit du stock.** Des spécifications écrites et non encore codées sont du travail payé qui ne rapporte rien, et qui se périme. Le [Lean]({{< relref "philosophie/philosophie_lean/lean_software_development/elimine_gaspillage" >}}) y voit deux gaspillages : le travail partiellement fait et les fonctionnalités superflues.

## Ce que cela demande

Le découpage vertical est plus exigeant. Chaque tranche doit rester **fine tout en restant utile**, ce qui est difficile : la tentation est de livrer « l'écran sans le back-end », qui est encore un découpage horizontal déguisé.

Deux appuis sur ce site :

- Le **S** d'[INVEST]({{< relref "pratiques/user_stories/rediger_us/stories_invest" >}}) — *Small* — et surtout son **V**, *Valuable* : une tranche qui n'apporte de valeur à personne n'est pas une tranche verticale.
- Le [User Story Mapping]({{< relref "pratiques/user_stories/user_stories_mapping/index" >}}), qui rend visible la première ligne horizontale du parcours : la tranche minimale qui permet à l'utilisateur d'aller au bout de son objectif.

Cela suppose enfin une [équipe pluridisciplinaire]({{< relref "equipe_agile/constitution_equipe/pluridisciplinaire" >}}) : on ne peut pas traverser une fonctionnalité de bout en bout si les compétences nécessaires sont réparties dans des [silos]({{< relref "equipe_agile/constitution_equipe/equipe_independante/silo" >}}) distincts. Le découpage du travail et le découpage des équipes sont le même sujet — c'est la [loi de Conway]({{< relref "equipe_agile/constitution_equipe/conway_law" >}}).
