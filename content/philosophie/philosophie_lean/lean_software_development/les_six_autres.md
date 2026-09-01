+++
title = "Les six autres principes"
description = "Créer des connaissances, intégrer la qualité, retarder l'engagement, livrer vite, respecter les personnes, optimiser l'ensemble."
weight = 20
+++

> [!ressource] Ressources
> - Mary et Tom Poppendieck, *Lean Software Development: An Agile Toolkit* (2003)
> - Mary et Tom Poppendieck, *Implementing Lean Software Development: From Concept to Cash* (2006)
> - [Lean Software Development — Poppendieck.llc](https://www.leanessays.com/)

Le premier principe, [éliminer le gaspillage]({{< relref "philosophie/philosophie_lean/lean_software_development/elimine_gaspillage" >}}), a sa propre page. Voici les six autres.

## Créer des connaissances

Un projet logiciel n'est pas une chaîne de production : c'est un **processus d'apprentissage**. Ce qu'on ne sait pas au départ — sur le besoin, sur la solution, sur la technologie — représente l'essentiel du risque.

Le principe consiste donc à organiser le travail pour apprendre vite et à peu de frais, plutôt que pour exécuter un plan :

- livrer tôt et souvent, pour transformer des hypothèses en observations ;
- écrire du code lisible, qui est le principal support de connaissance de l'équipe ;
- documenter les décisions structurantes et leur *pourquoi*, pas la mécanique du code ;
- traiter chaque incident comme une source d'information et non comme une faute.

C'est le même raisonnement que la raison [encaisser l'incertitude]({{< relref "philosophie/pourquoi_agile/encaisser_incertitude/index" >}}).

## Intégrer la qualité dès la conception

*Build quality in*. La qualité ne se contrôle pas à la fin, elle se construit pendant — parce qu'un défaut détecté tard coûte bien plus cher que le même défaut détecté tôt.

> [!affirmation] Affirmation
> Si vous trouvez régulièrement des défauts lors de la recette, votre problème n'est pas la recette : c'est le processus qui laisse les défauts arriver jusque-là.

C'est la transposition directe du [Jidoka]({{< relref "philosophie/philosophie_lean/toyota_production_system/jidoka" >}}) et du *poka-yoke*. En pratique : tests automatisés, intégration continue, revue par les pairs, [Definition of Done]({{< relref "frameworks/framework_scrum/artefact_engagements/definition_of_done" >}}) explicite. Voir aussi [la qualité vaut-elle le coût ?]({{< relref "philosophie/pourquoi_agile/produit_haute_qualite/qualite_logicielle/index" >}}).

## Retarder l'engagement

*Defer commitment*, ou la règle du **dernier moment responsable** : prendre une décision irréversible le plus tard possible, tant que ce report ne coûte rien.

L'idée n'est pas de procrastiner, mais de constater qu'une décision prise tard est prise avec plus d'information. Reste à distinguer :

- les décisions **réversibles** — à prendre vite, on corrigera ;
- les décisions **irréversibles** ou coûteuses à défaire (choix d'un schéma de données, d'un fournisseur, d'une architecture) — à retarder jusqu'au dernier moment utile.

En pratique : ne pas détailler tout le backlog à l'avance, garder les options ouvertes par une conception simple, et se méfier des abstractions construites pour un besoin supposé.

## Livrer aussi vite que possible

Livrer vite n'est pas travailler plus. C'est **réduire la taille des lots** pour raccourcir la boucle de retour.

> [!danger] Le contresens
> *Deliver fast* ne signifie ni heures supplémentaires, ni sacrifice de la qualité — les deux ralentissent durablement. Il s'agit de réduire le **délai entre la décision et la mise à disposition**, en éliminant les attentes du processus.

Le levier n'est presque jamais la vitesse de frappe des développeurs : c'est le temps passé en file d'attente, que rend visible la [Value Stream Map]({{< relref "philosophie/philosophie_lean/value_stream_map" >}}). C'est aussi ce que mesurent les [métriques DORA]({{< relref "pratiques/devops/dora/dora_core/metriques" >}}).

## Respecter les personnes

Avec l'amélioration continue, c'est l'un des deux piliers du *Toyota Way*. Le principe : **les décisions sur le travail appartiennent à ceux qui font le travail**, parce qu'eux seuls voient les problèmes réels.

Cela suppose des managers qui passent d'une chaîne de contrôle à une chaîne d'aide, et une organisation où signaler un problème ne se retourne pas contre celui qui le signale.

Le site développe ce point ailleurs : [rendre l'équipe propriétaire de son processus]({{< relref "philosophie/pourquoi_agile/proprietaire_processus" >}}), [sécurité psychologique]({{< relref "equipe_agile/culture/psychological_safety" >}}), [développeurs et non exécutants]({{< relref "equipe_agile/roles_postures/developpeur_executant/index" >}}).

## Optimiser l'ensemble

*See the whole*. Le principe le plus contre-intuitif, et celui que les organisations violent le plus systématiquement.

Optimiser chaque partie séparément **dégrade** le résultat global. Une équipe de développement à pleine capacité produit plus de code, donc allonge la file d'attente de la recette. Un service qui réduit ses coûts en externalisant crée des délais de coordination qui coûtent davantage.

> [!definition] Optimisation locale
> Chaque service maximise son propre indicateur — taux d'occupation, nombre de tickets fermés, respect de son budget — et la performance de bout en bout se dégrade, sans que personne n'en soit responsable.

Deux conséquences concrètes :

- **Mesurer le flux complet**, du besoin exprimé à la valeur livrée, et pas la productivité de chaque étape. Voir [Mesurer la productivité ?]({{< relref "regard_critique/mesurer_productivite/index" >}}).
- **Constituer des équipes qui couvrent tout le flux**, plutôt que des équipes par spécialité qui se passent le travail. Voir [équipe pluridisciplinaire]({{< relref "equipe_agile/constitution_equipe/pluridisciplinaire" >}}) et [silos]({{< relref "equipe_agile/constitution_equipe/equipe_independante/silo" >}}).

C'est sur ce point que le Lean se distingue le plus nettement de l'agilité telle qu'elle est souvent pratiquée : optimiser le développement ne sert à rien si la contrainte est ailleurs. Voir [Lean VS Agile]({{< relref "philosophie/philosophie_lean/lean_vs_agile" >}}).
