+++
title = "Valeurs, Principes et Pratiques"
description = "Les valeurs, principes et pratiques de XP tels que Kent Beck les articule dans Extreme Programming Explained."
weight = 15
+++

C'est dans la seconde édition de son livre *Extreme Programming Explained* que Kent Beck définit un ensemble de valeurs, de principes et de pratiques qui forment la philosophie de XP.

![XP Bridge Values Principles and Practices](xp_bridge.png)

- Valeurs == ce qu’on souhaite amener
- Principes == les lignes directrices dans un domaine spécifique
- Pratiques == ce qu’on fait au quotidien 

|  Aspect   |                                                                                              Description                                                                                              |                                                             Exemples dans XP                                                              |
| :-------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------: |
|  Valeurs  | Croyances fondamentales et générales qui donnent une direction et un sens à l’équipe. Elles définissent pourquoi l’équipe adopte une certaine façon de travailler : elles servent d’"étoile polaire". |                                    Communication, Simplicité, Feedback (Rétroaction), Courage, Respect                                    |
| Principes |                 Lignes  directrices concrètes issues des valeurs. Les principes traduisent les  valeurs en concepts que l’équipe peut suivre pour guider ses décisions  quotidiennes.                 |                 Retour rapide, Simplicité assumée, Changement incrémental, Acceptation du changement, Travail de qualité                  |
| Pratiques |                Méthodes  ou activités spécifiques appliquées régulièrement par l’équipe. Elles  permettent de mettre en œuvre les principes, et donc aussi les valeurs,  au quotidien.                | Programmation  en binôme, Développement dirigé par les tests (TDD), Intégration  continue, Petites livraisons fréquentes, Refactorisation |

## Valeurs
> Values need to be made explicit because they give meaning to practices. Without them, practices can turn into tedious, dull tasks with no purpose. Whether communication is valuable for someone can be known by the practices also, writing a document 5 pages long instead of 15 minute conversation.

## Principes
> [!ressource] Ressources
> - Extreme Programming Explained (first edition) - chapitre 8
> - [Principles of XP - Martin Fowler](https://martinfowler.com/bliki/PrinciplesOfXP.html)


> Practices are situation dependent. If the situation changes, you choose different practices to meet those conditions. Your values do not have to change in order to adapt to a new situation. Some new principles may be called when you change domains

Les principes sont le pont qui relie les valeurs aux pratiques.
- E.g. en suivant le principe d'humanité alors pour l'exemple précédent on s'engage sur une conversation orale qui répond au besoin de connexion humaine, de compréhension et d'échange de connaissances.

### Principes fondamentaux
- Rapid Feedback
- Assume Simplicity
- Incremental Change
- Embracing Change
- Quality Work

### Principes secondaires
- Teach Learning
- Small Initial Investment
- Play to Win
- Concrete Experiments
- Open, honest Communication
- Work with people's instincts - not against them
- Accepted Responsibility
- Local Adaptation
- Travel Light
- Honest Measurement

<embed src="/static/pdf/xp/XP-first-edition-chap8.pdf" width="100%" height="1000px"/>

## Pratiques

> [!ressource] Ressources
> - [What is Extreme Programming? (Practices)](https://ronjeffries.com/xprog/what-is-extreme-programming/)

Voir [Circle of Life]({{< relref "frameworks/framework_xp/circle_of_life" >}})

<!--
DANS SECONDE EDITION IL Y A + DE PRATIQUES

> [!ressource] Ressources
> - Extreme Programming Explained (first edition) - chapitre 10

- The Planning Game — Déterminer rapidement le périmètre de la prochaine version en combinant les priorités métier et les estimations techniques. Lorsque la réalité remet en cause le plan, celui-ci est mis à jour.

- Small releases — Mettre rapidement en production un système simple, puis publier de nouvelles versions à intervalles très courts.

- Metaphor — Guider tout le développement à l’aide d’une histoire simple et partagée expliquant le fonctionnement global du système.

- Simple design — Concevoir le système de la manière la plus simple possible à chaque instant. Toute complexité supplémentaire est supprimée dès qu’elle est identifiée.

- Testing — Les programmeurs écrivent continuellement des tests unitaires, qui doivent tous réussir pour que le développement puisse continuer. Les clients écrivent des tests permettant de vérifier que les fonctionnalités sont terminées.

- Refactoring — Restructurer le système sans modifier son comportement afin de supprimer les duplications, d’améliorer la compréhension du code, de le simplifier ou de le rendre plus flexible.

- Pair programming — Tout le code destiné à la production est écrit par deux programmeurs travaillant ensemble sur un même poste.

- Collective ownership — N’importe quel membre de l’équipe peut modifier n’importe quelle partie du code, à tout moment.

- Continuous integration — Intégrer et compiler le système plusieurs fois par jour, chaque fois qu’une tâche est terminée.

- 40 hour week — Ne pas dépasser 40 heures de travail par semaine en règle générale. Ne jamais faire d’heures supplémentaires deux semaines consécutives.

- On-site customer — Intégrer à l’équipe un véritable utilisateur, présent à temps plein et disponible pour répondre aux questions.

- Coding standards — Tous les programmeurs écrivent le code conformément à des règles communes qui mettent l’accent sur la communication et la lisibilité du code.
-->