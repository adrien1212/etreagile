+++
title = "3. Livrer un produit de haute qualité"
linkTitle = "Produit de haute qualité"
description = "La qualité n'est pas ce qu'on sacrifie pour aller vite : c'est ce qui permet d'aller vite longtemps."
weight = 50
+++

> [!ressource] Ressources
> - [La qualité vaut-elle le coût ?]({{< relref "philosophie/pourquoi_agile/produit_haute_qualite/qualite_logicielle/index" >}}) — le chapitre dédié
> - Accelerate: The Science of Lean Software and DevOps
> - Clean Agile - Robert C. Martin

L'agilité vise à livrer un produit de haute qualité, répondant aux besoins réels et évolutifs du client.

## De quelle qualité parle-t-on ?

Le mot recouvre deux réalités qu'il faut distinguer, sous peine de discussions sans fin avec les parties prenantes.

| | Qui la constate | Exemples |
| --- | --- | --- |
| **Qualité externe** | L'utilisateur, le client | Le produit fait ce qu'on attend, ne plante pas, est agréable et rapide |
| **Qualité interne** | Les développeurs seuls | Lisibilité du code, couverture de tests, propreté de la conception |

La qualité externe se négocie : on peut décider de livrer une fonctionnalité rudimentaire pour valider une hypothèse. **La qualité interne, elle, ne se négocie pas** — non par vertu, mais par intérêt : c'est elle qui détermine le [coût du changement]({{< relref "philosophie/pourquoi_agile/produit_haute_qualite/qualite_logicielle/cout_changement" >}}) de demain.

> [!affirmation] Affirmation
> Sacrifier la qualité interne pour tenir une date, c'est emprunter à un taux qu'on ne connaît pas. C'est la définition même de la [dette technique]({{< relref "philosophie/pourquoi_agile/produit_haute_qualite/qualite_logicielle/dette_technique" >}}).

## Comment ?

- **Livraison de valeur continue** : priorité aux fonctionnalités essentielles, évitant les besoins initiaux non prioritaires.
- **Feedback permanent** : présentation régulière de versions intermédiaires pour ajuster le produit aux attentes.
- **Tests et qualité** : détection et correction immédiates des défauts à chaque itération.
- **Refactoring** : amélioration continue du code pour préserver sa lisibilité et supprimer les duplications.
- **Approche adaptative** : évaluation régulière du processus pour garantir l'évolutivité et la qualité finale.

À quoi s'ajoute un dispositif proprement agile : la **[Definition of Done]({{< relref "frameworks/framework_scrum/artefact_engagements/definition_of_done" >}})**. Elle rend la qualité *explicite et non négociable* en la sortant du jugement individuel : un incrément est terminé ou il ne l'est pas, et « terminé » a été défini à l'avance par l'équipe.

## Qualité et vitesse ne s'opposent pas

C'est l'intuition la plus contre-intuitive de l'agilité, et c'est aussi la mieux établie empiriquement.

Le programme de recherche **DORA**, synthétisé dans *Accelerate*, a montré par l'analyse statistique que les organisations les plus rapides sont aussi les plus fiables : le débit (fréquence de déploiement, délai de livraison) et la stabilité (taux d'échec des changements, temps de restauration) **progressent ensemble** au lieu de s'échanger.

> [!definition] Ce que cela réfute
> L'arbitrage « on peut avoir vite ou bien, choisissez » n'est pas une loi de la nature. C'est le symptôme d'un système de livraison mal outillé. Voir [Accelerate]({{< relref "pratiques/devops/accelerate/index" >}}) et les [métriques DORA]({{< relref "pratiques/devops/dora/dora_core/metriques" >}}).

## La qualité n'est pas qu'une affaire de méthode

Un framework de gestion de projet ne produit pas du code de qualité. Scrum ne dit rien sur la manière d'écrire un test. C'est précisément le reproche adressé au *[Flaccid Scrum]({{< relref "regard_critique/abandonner_agile/flaccid_scrum" >}})* : des équipes qui adoptent les cérémonies sans les pratiques techniques, et qui ralentissent après quelques mois sous le poids de leur propre code.

> [!definition] Important
> Agile combine la gestion d'équipe/projet avec l'excellence technique (en savoir plus [ici]({{< relref "philosophie/philosophie_agile/viser_excellence" >}}))

C'est aussi la raison d'être du mouvement [Software Craftsmanship]({{< relref "pratiques/software_craftsmanship/index" >}}), né en 2008 pour remettre l'excellence technique au centre — là où l'agilité, occupée par ses conférences et ses certifications, l'avait laissée de côté.
