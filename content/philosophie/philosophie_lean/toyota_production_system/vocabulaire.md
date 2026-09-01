+++
title = "Vocabulaire du Lean"
description = "Muda, mura, muri, kaizen, gemba, PDCA : les quelques termes japonais qu'on rencontre partout dans la littérature Lean et agile."
weight = 30
+++

> [!ressource] Ressources
> - Taiichi Ohno, *Toyota Production System: Beyond Large-Scale Production* (1978)
> - Jeffrey Liker, *The Toyota Way* (2004)
> - [Lean Enterprise Institute — Lean Lexicon](https://www.lean.org/lexicon-terms/)
> - Mike Rother, *Toyota Kata* (2009)

Quelques termes reviennent constamment dès qu'on lit du Lean — y compris dans la littérature agile, qui les emploie souvent sans les définir. En voici l'essentiel.

## Les trois M : muda, mura, muri

C'est la distinction la plus utile du Lean, et la plus souvent oubliée. On parle beaucoup du gaspillage ; on parle rarement de ce qui le **produit**.

| Terme | Traduction | Exemple en développement logiciel |
| --- | --- | --- |
| **Muda** | Le gaspillage | Une fonctionnalité que personne n'utilise, un ticket qui attend trois semaines en revue |
| **Mura** | L'irrégularité, la variabilité | Un sprint calme suivi d'un sprint en urgence ; des mises en production groupées en fin de mois |
| **Muri** | La surcharge | Une équipe à 120 % de capacité, des astreintes permanentes, trois projets en parallèle par personne |

> [!affirmation] Affirmation
> **Mura et muri sont les causes ; muda est le symptôme.** Une équipe surchargée (*muri*) fait des erreurs qu'il faudra corriger (*muda*). Une charge en dents de scie (*mura*) oblige à dimensionner pour le pic, donc à sous-utiliser le reste du temps (*muda*).

C'est pourquoi s'attaquer directement au gaspillage donne souvent peu de résultats : on traite l'effet. La limitation du travail en cours ([WIP]({{< relref "frameworks/framework_kanban/principes" >}})) est efficace précisément parce qu'elle agit sur le *muri*, et le lissage (*heijunka*) sur le *mura*.

Ohno avait par ailleurs identifié **sept gaspillages** dans l'industrie (surproduction, attente, transport, sur-traitement, stock, mouvement, défauts) ; les Poppendieck en ont proposé une transposition au logiciel, détaillée dans [Éliminer le gaspillage]({{< relref "philosophie/philosophie_lean/lean_software_development/elimine_gaspillage" >}}).

## Kaizen — l'amélioration continue

*Kai* (changement) + *zen* (bon) : le changement pour le mieux. Le kaizen désigne l'amélioration **par petits pas, continue, et menée par ceux qui font le travail** — par opposition au *kaikaku*, la transformation brutale décidée d'en haut.

Deux caractéristiques qu'on oublie souvent :

- **Le kaizen suppose un standard.** On ne peut améliorer que ce qui est stabilisé : sans façon de faire décrite, il n'y a pas d'écart mesurable, donc rien à améliorer. Standardiser n'est pas le contraire de l'amélioration, c'en est le préalable.
- **Le kaizen appartient à l'équipe.** Une amélioration décidée par un service méthodes n'est pas du kaizen. Voir [Rendre l'équipe propriétaire de son processus]({{< relref "philosophie/pourquoi_agile/proprietaire_processus" >}}).

En agilité, le rendez-vous qui porte ce rôle est la [rétrospective]({{< relref "frameworks/framework_scrum/ceremonies/retrospective" >}}).

## Gemba — le terrain

Le *gemba*, c'est « le lieu réel », là où le travail se fait. La pratique associée est le **genchi genbutsu** : *aller voir par soi-même*.

Le principe est simple et rarement appliqué : on ne comprend pas un problème depuis un tableau de bord ou un rapport. Il faut aller là où il se produit, observer, et parler à ceux qui font le travail.

Transposé au logiciel : lire les logs de production plutôt que le résumé d'incident, regarder un utilisateur se servir du produit plutôt que lire son verbatim, s'asseoir à côté de l'équipe plutôt que consulter l'avancement du board.

## PDCA — la boucle d'amélioration

Le cycle **Plan – Do – Check – Act**, hérité de Walter Shewhart et popularisé par **W. Edwards Deming**, est la mécanique du kaizen :

1. **Plan** — formuler une hypothèse d'amélioration
2. **Do** — l'essayer, en petit
3. **Check** — constater l'écart entre ce qu'on attendait et ce qu'on observe
4. **Act** — adopter, ajuster, ou abandonner

> [!definition] Une nuance de Deming
> Deming préférait la forme **PDSA**, où *Study* remplace *Check* : « vérifier » suggère de contrôler la conformité, alors qu'il s'agit d'**étudier** ce qui s'est passé et pourquoi. C'est cette variante que reprend la [démarche Kanban]({{< relref "frameworks/framework_kanban/demarche/index" >}}).

On reconnaîtra ici l'empirisme des [trois piliers de Scrum]({{< relref "frameworks/framework_scrum/piliers/index" >}}) : transparence, inspection, adaptation.

## Les 5 pourquoi

Méthode attribuée à Ohno pour remonter d'un symptôme à sa cause racine : devant un problème, demander « pourquoi ? » cinq fois de suite.

> La machine s'est arrêtée. *Pourquoi ?* Un fusible a sauté par surcharge. *Pourquoi ?* Le roulement était mal lubrifié. *Pourquoi ?* La pompe de lubrification ne fonctionnait pas correctement. *Pourquoi ?* Son axe était usé. *Pourquoi ?* Il n'y avait pas de filtre et des copeaux métalliques sont entrés.

Sans les cinq pourquoi, on remplace le fusible — et le problème revient. Le chiffre cinq n'a rien de magique : il signifie simplement qu'on s'arrête généralement trop tôt.

## Deux mots qu'on croise aussi

- **Heijunka** — le lissage de la charge, pour éviter les à-coups (*mura*). En logiciel : livrer en continu plutôt qu'en grosses mises en production espacées.
- **Kata** — la routine d'apprentissage. Popularisé par Mike Rother dans *Toyota Kata* (2009), qui soutient que ce qui rend Toyota difficile à copier n'est pas ses outils, mais la manière dont ses managers entraînent quotidiennement leurs équipes à résoudre des problèmes.
