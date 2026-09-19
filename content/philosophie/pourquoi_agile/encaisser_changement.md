+++
title = "2. Encaisser le changement"
linkTitle = "Encaisser le changement"
description = "Cesser de traiter le changement comme un incident de parcours, et se doter des pratiques qui en rendent le coût acceptable."
weight = 40
+++

> [!ressource] Ressources
> - Extreme Programming Explained: **Embrace Change** — Kent Beck
> - Scaling Software Agility - p26
> - [Le coût du changement]({{< relref "philosophie/pourquoi_agile/produit_haute_qualite/qualite_logicielle/cout_changement" >}}) — la page qui détaille la courbe

## Le constat

> [!affirmation] Affirmation
>  Accueillir le changement à bras ouverts plutôt que de le craindre et le combattre.

> We do not assume that change will be small and manageable. Rather, we assume that change will be constant, and we deliver in small increments to better track change. [^1]

On sait que de nombreux paramètres sont imprévisibles lors du projet. Il s'agit donc de mieux
contrôler cette imprévisibilité sans la nier, en évitant d'être systématiquement obsédé par les
plans initiaux obsolètes.

Le sous-titre du livre fondateur de XP dit tout : *Embrace Change*. Non pas « tolérer » le changement, ni « gérer » le changement — **l'accueillir**, parce qu'un changement de besoin est une bonne nouvelle : il signifie que quelqu'un a appris quelque chose.

C'est le deuxième principe du [Manifeste]({{< relref "philosophie/philosophie_agile/manifeste" >}}) :

> Accueillez positivement les changements de besoins, même tard dans le projet. Les processus Agiles exploitent le changement **pour donner un avantage compétitif au client**.

## Pourquoi le changement faisait peur

Dans une conduite prédictive, le changement est un incident : il invalide une analyse déjà payée, oblige à rouvrir des phases closes, et fait dériver le plan. D'où les dispositifs conçus pour le décourager — comité de contrôle des changements, avenant contractuel, gel du périmètre.

Le problème n'est pas que ces dispositifs soient irrationnels. **Ils sont la réponse logique à un système où le changement coûte cher.** La véritable question est donc : pourquoi coûte-t-il cher ?

## Rendre le changement bon marché

C'est ici que l'agilité se distingue vraiment. Elle ne se contente pas de *déclarer* qu'on accueille le changement — elle s'attaque à son coût.

> [!definition] Le lien avec la qualité
> Un logiciel qu'on ne peut pas modifier sans tout casser rend le changement coûteux, quelle que soit la méthode employée. **L'accueil du changement est une propriété technique avant d'être une posture managériale.** C'est tout l'objet de la [courbe du coût du changement]({{< relref "philosophie/pourquoi_agile/produit_haute_qualite/qualite_logicielle/cout_changement" >}}) et de la [dette technique]({{< relref "philosophie/pourquoi_agile/produit_haute_qualite/qualite_logicielle/dette_technique" >}}).

Les pratiques qui font baisser ce coût sont, sans surprise, les [pratiques techniques de XP]({{< relref "frameworks/framework_xp/pratiques" >}}) :

- **Les tests automatisés** — sans filet, toute modification est un pari. Avec un filet, elle devient une opération courante.
- **Le refactoring continu** — maintenir la conception habitable au lieu de la laisser se dégrader.
- **L'intégration continue** — détecter en minutes plutôt qu'en semaines qu'un changement en a cassé un autre.
- **Les petites livraisons fréquentes** — un petit lot est plus facile à corriger, et surtout plus facile à abandonner.
- **La conception simple** — ne pas construire aujourd'hui les abstractions dont on suppose avoir besoin demain, car ce sont elles qui deviendront l'obstacle au vrai changement quand il arrivera.

⇒ Une équipe agile se dote de pratiques et d'outils qui lui facilitent l'accueil du changement.

> [!definition] Le cycle de vie qui correspond
> C'est l'aspect **incrémental** du développement qui porte cette raison : livrer par tranches utilisables permet d'ajuster les exigences à l'évolution de l'environnement, là où l'aspect *itératif* sert plutôt la qualité du produit. Voir [Les quatre cycles de vie]({{< relref "philosophie/pourquoi_agile/encaisser_incertitude/cycles_de_vie" >}}).

## Ce que cela change dans le contrat

Accueillir le changement a une conséquence contractuelle directe, résumée par la [croix de fer]({{< relref "philosophie/philosophie_agile/croix_de_fer" >}}) : si le coût et le délai sont fixés par des itérations régulières, alors **c'est le périmètre qui devient la variable d'ajustement**.

| Traditionnelle | Agile |
| --- | --- |
| Périmètre fixe, coût et délai estimés | Coût et délai fixes, périmètre ajusté |

C'est aussi ce que recouvre la troisième valeur du Manifeste, *la collaboration avec les clients plus que la négociation contractuelle* : voir [Engager le client]({{< relref "engager_client" >}}) et [Négociation et compromis]({{< relref "equipe_agile/modes_de_travail/negociation" >}}).

> [!danger] Le contresens fréquent
> « Accueillir le changement » ne signifie pas accepter n'importe quel changement à n'importe quel moment. Un changement en cours de Sprint remet en cause le [Sprint Goal]({{< relref "frameworks/framework_scrum/artefact_engagements/sprint_goal" >}}), c'est-à-dire l'engagement même de l'équipe. Le changement est accueilli **entre** les itérations, et l'itération courte est précisément ce qui rend cette attente supportable.

[^1]: Scaling Software Agility - p26
