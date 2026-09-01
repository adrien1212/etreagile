+++
title = "6. Engager le client pour produire le bon produit"
linkTitle = "Engager le client"
description = "Impliquer le client au quotidien dans la création plutôt qu'aux deux extrémités du projet, pour vérifier en continu qu'on construit le bon produit."
weight = 80
+++

> [!ressource] Ressources
> - [Le Manifeste Agile]({{< relref "philosophie/philosophie_agile/manifeste" >}}) — valeur 3 et principe 4
> - [Déclaration des droits]({{< relref "philosophie/philosophie_agile/droits" >}}) — Kent Beck

Avec l'agilité nous impliquons le client au quotidien dans le processus de création. En lui
fournissant rapidement des Minimum Viable Product nous nous assurons que :
- Le produit répond toujours aux attentes de l'utilisateur et des clients
- De minimiser le coût d'un changement de direction, voire de l'anticiper
- Le client a une visibilité
- ⇒ On évite ainsi le gaspillage d'argent

## Construire *avec* plutôt que *pour*

Le quatrième principe du Manifeste est d'une exigence rarement mesurée :

> Les utilisateurs ou leurs représentants et les développeurs doivent travailler ensemble **quotidiennement** tout au long du projet.

Quotidiennement — pas à un comité de pilotage mensuel. C'est ce que traduit la troisième valeur, *la collaboration avec les clients plus que la négociation contractuelle* : non pas que le contrat soit inutile, mais qu'un contrat ne dit jamais si le produit est le bon.

Dans une conduite prédictive, le client intervient pour signer un cahier des charges puis pour recetter. Entre les deux, l'écart entre ce qu'il a écrit et ce qu'il voulait ne peut pas être détecté — il n'apparaît qu'à la livraison, quand le corriger coûte le plus cher.

## Le bon produit, pas seulement le produit bien construit

Il y a deux façons d'échouer, et elles n'ont pas le même remède.

| | Question | Remède |
| --- | --- | --- |
| **Build the thing right** | Le produit est-il bien construit ? | [La qualité]({{< relref "produit_haute_qualite" >}}), les tests, la Definition of Done |
| **Build the right thing** | Est-ce le bon produit ? | L'engagement du client, le feedback, la mesure d'usage |

Une équipe peut exceller sur la première et se tromper entièrement sur la seconde. C'est même le scénario le plus coûteux : un logiciel irréprochable dont personne ne veut. Seul le client — ou l'usage réel — peut trancher la seconde question, et il ne peut le faire que devant quelque chose qui fonctionne.

## Comment on l'engage concrètement

- **La [Sprint Review]({{< relref "frameworks/framework_scrum/ceremonies/review" >}})** — non pas une démonstration où l'on présente, mais une session de travail où les parties prenantes influencent la suite. Le Scrum Guide est explicite : ce n'est pas un point d'avancement.
- **Les incréments livrés tôt** — chaque [incrément]({{< relref "frameworks/framework_scrum/artefacts/increment" >}}) est une question posée au client sous une forme qu'il peut réellement évaluer.
- **La conversation autour des stories** — les [3C]({{< relref "pratiques/user_stories/user_stories_mapping/les_3c" >}}) placent la compréhension partagée avant le document.
- **Le [MVP]({{< relref "regard_critique/mvp_et_pretotype" >}})** — livrer le minimum qui permette d'apprendre quelque chose, en gardant à l'esprit que le terme est aujourd'hui largement dévoyé.

> [!affirmation] En un mot
> Du **feedback** régulier

## Les obstacles réels

> [!danger] Le client absent
> Le principe suppose un client disponible. Dans les faits, il est souvent remplacé par un [Product Owner]({{< relref "frameworks/framework_scrum/responsabilites/product_owner" >}}) qui n'a ni le mandat de décider, ni l'accès aux utilisateurs finaux. Le rituel est alors respecté sans que la boucle de feedback existe : on présente à quelqu'un qui ne peut pas trancher.

Deux autres difficultés méritent d'être nommées :

- **Le client n'est pas l'utilisateur.** Celui qui paie et celui qui se sert du produit sont fréquemment deux personnes aux intérêts distincts. Engager le premier ne garantit pas d'être [centré sur le second]({{< relref "user_centric" >}}).
- **Le cadre contractuel peut interdire la collaboration.** Un forfait à périmètre fixe transforme chaque échange en négociation d'avenant. Voir [Négociation et compromis]({{< relref "equipe_agile/modes_de_travail/negociation" >}}) et la [croix de fer]({{< relref "philosophie/philosophie_agile/croix_de_fer" >}}).

Kent Beck avait anticipé cette tension en rédigeant une [déclaration des droits]({{< relref "philosophie/philosophie_agile/droits" >}}) réciproque : le client a le droit d'être informé et de changer d'avis, les développeurs ont le droit de connaître les priorités et de donner des estimations qu'on ne leur impose pas.