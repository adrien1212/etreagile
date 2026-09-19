+++
title = "PRD, vision et US"
description = "Quand l'agent implémente ce qu'on écrit, INVEST et les 3C cessent d'être des conseils. Pourquoi un agent ne converse pas, et ce que cela exige des user stories."
weight = 30
+++

> [!ressource] Ressources
> - User Story Mapping - Jeff Patton
> - [Essential XP: Card, Conversation, Confirmation - Ron Jeffries](https://ronjeffries.com/xprog/articles/expcardconversationconfirmation/)
> - [Spec-Driven Development: The Waterfall Strikes Back - Marmelab](https://marmelab.com/blog/2025/11/12/spec-driven-development-waterfall-strikes-back.html)
> - [Spec-Driven Development Isn't Waterfall Unless You're Using It That Way - Yuval Yeret](https://yuvalyeret.com/blog/spec-driven-development-isnt-waterfall-unless-youre-using-it-that-way/)

Si [écrire du code devient bon marché]({{< relref "ouvertures/agile_et_ia/spec_driven_development/index" >}}), alors la qualité du produit ne dépend plus de la qualité du code : elle dépend de la **qualité de ce qu'on a demandé**. Le livrable de l'humain devient la spécification.

Encore faut-il savoir de quelle spécification on parle. Vision, PRD et user story ne sont pas interchangeables, et les confondre est la première erreur.

## Trois niveaux, trois usages

> [!definition] PRD (Product Requirements Document)
> Document décrivant **ce qu'un produit ou une fonctionnalité doit faire et pourquoi** : problème visé, utilisateurs, règles métier, cas limites, critères de réussite. Il ne décrit **pas** comment le construire.

Les outils SDD réintroduisent une hiérarchie que nous connaissons déjà sous le nom d'[oignon de la planification]({{< relref "pratiques/planifier/niveau_planification/index" >}}) :

| Niveau | Artefact SDD | Question à laquelle il répond |
| --- | --- | --- |
| [Vision]({{< relref "pratiques/planifier/niveau_planification/vision" >}}) | `constitution`, principes du projet | Pourquoi ce produit existe, ce qu'on ne fera jamais |
| PRD | `spec.md` | Quel problème, pour qui, avec quelles règles |
| User story | stories issues du PRD | Quelle tranche de valeur, livrable seule |
| Tâche | `tasks.md` | Quelles activités techniques |

Le mouvement est le même que dans un [Product Backlog]({{< relref "frameworks/framework_scrum/artefacts/product_backlog" >}}) [affiné progressivement]({{< relref "pratiques/planifier/niveau_planification/index" >}}) : on part du vague pour aller vers le précis. Ce qui change, c'est qu'**à chaque niveau, ce qui n'est pas écrit n'existe pas**.

## La tension : un agent ne converse pas

C'est le point qui heurte le plus directement notre cours, et il ne faut pas l'esquiver.

Toute notre approche des [récits utilisateur]({{< relref "pratiques/user_stories/index" >}}) repose sur une thèse forte de Jeff Patton et Ron Jeffries : la user story **n'est pas une spécification**. Les [3C]({{< relref "pratiques/user_stories/user_stories_mapping/les_3c" >}}) posent que la [carte]({{< relref "pratiques/user_stories/user_stories_mapping/les_3c#la-carte" >}}) est volontairement pauvre, qu'elle n'est qu'un *support pour se rappeler de la conversation*, et que la compréhension naît de la [Conversation]({{< relref "pratiques/user_stories/user_stories_mapping/les_3c#la-conversation" >}}) :

> Shared documents aren't shared understanding

Or **un agent ne participe à aucune conversation**. Il ne dispose que de ce qui est écrit. Toute la connaissance tacite qui circulait à l'oral — les cas limites évidents, le contexte métier, les « ça va de soi » — devient invisible pour lui. Et ce qui est invisible est *inventé* : le projet BMAD résume le risque en une phrase, *les assistants de code transforment les assomptions non dites en code*.

> [!affirmation] Affirmation
> La Conversation ne disparaît pas : elle reste entre humains. Ce qui change, c'est qu'il faut désormais **en transcrire le résultat**.
>
> Ce n'est pas un retour au cahier des charges exhaustif : c'est la **Confirmation** qui devient l'artefact central, parce qu'elle est la seule des 3C que l'agent peut exécuter.

Autrement dit, le déplacement se fait à l'intérieur des 3C, de la Carte vers la [Confirmation]({{< relref "pratiques/user_stories/user_stories_mapping/les_3c#la-confirmation" >}}) : la liste de critères d'acceptation cesse d'être un aide-mémoire pour devenir le **contrat de vérification** du travail de l'agent. C'est aussi ce qui relie cette page à notre réflexion sur la [documentation vivante]({{< relref "regard_critique/pas_de_documentation" >}}) : la Confirmation automatisée *est* la documentation.

## Pourquoi INVEST se durcit

[INVEST]({{< relref "pratiques/user_stories/rediger_us/stories_invest" >}}) était une grille de bonnes pratiques : une story qui la respectait mal se rattrapait en réunion. Ce filet disparaît. Reprenons les six critères.

**[I]({{< relref "pratiques/user_stories/rediger_us/stories_invest#indépendante" >}}) — Indépendante : le critère le plus menacé.** Un LLM optimise la cohérence technique, pas la livraison incrémentale : livré à lui-même, il produit un découpage **horizontal** (une couche technique partagée d'abord, les stories ensuite) plutôt que **vertical**. Nous l'avons observé en direct dans [l'exemple SDD]({{< relref "ouvertures/agile_et_ia/spec_driven_development/exemple_sdd" >}}), avec une phase *Foundational* explicitement bloquante. Le rôle humain est de **contester ce découpage**.

**[N]({{< relref "pratiques/user_stories/rediger_us/stories_invest#négociable" >}}) — Négociable : le critère qui perd son interlocuteur.** Une story négociable présuppose quelqu'un avec qui négocier. Un agent ne négocie pas : il implémente ce qui est écrit, y compris une bêtise. La négociation doit donc avoir lieu **avant l'écriture**, entre humains. Le danger est net : si personne ne l'assume, la story redevient un **contrat**, et nous retombons dans la spécification-contrat que le Manifeste combattait.

**[V]({{< relref "pratiques/user_stories/rediger_us/stories_invest#valuable" >}}) — Valuable : le critère le plus souvent trahi par les outils.** Voir la section suivante.

**[E]({{< relref "pratiques/user_stories/rediger_us/stories_invest#estimable" >}}) — Estimable : le critère qui change de sens.** Estimer l'effort *humain* d'une story perd sa signification quand c'est un agent qui l'implémente. Ce qui reste utile, c'est l'usage qu'en fait le [débat No Estimates]({{< relref "regard_critique/estimer" >}}) : *si l'équipe n'arrive pas à estimer, c'est que la story est trop grosse ou mal comprise*. L'estimation devient un **détecteur de flou**, plus qu'une prévision.

**[S]({{< relref "pratiques/user_stories/rediger_us/stories_invest#small" >}}) — Small : le critère qui protège du tunnel.** C'est la taille du lot qui distingue le SDD d'un [retour au Waterfall]({{< relref "naissance_agile/methodologie_waterfall/definition" >}}). Rien n'empêche techniquement de demander à une IA un PRD couvrant six mois — sauf la discipline.

**[T]({{< relref "pratiques/user_stories/rediger_us/stories_invest#testable" >}}) — Testable : le critère qui devient le mécanisme de contrôle.** C'est le seul moyen de vérifier le travail de l'agent sans relire chaque ligne, d'où l'importance renouvelée du [TDD]({{< relref "frameworks/framework_xp/pratiques" >}}) et d'une [Definition of Done]({{< relref "frameworks/framework_scrum/artefact_engagements/definition_of_done" >}}) explicite. Une story non testable n'est plus « perfectible » : elle est **invérifiable**.

> [!affirmation] Affirmation
> INVEST et les 3C ne changent pas de contenu. Ils changent de statut : ils passent de **conseils de qualité** à **conditions de fonctionnement**.

## Le contre-exemple : la fausse user story

Les outils SDD génèrent des éléments étiquetés « User Stories » qui n'en sont pas. Marmelab relève cet exemple, produit par un toolkit :

> [!danger] Ceci n'est pas une user story
> *« As a system administrator, I want the referred by relationship to be stored in the database. »*

Passons-la à la grille :

- **Valuable ?** Non. Stocker une relation en base n'a aucune valeur pour personne. C'est un moyen, pas une fin.
- **Le rôle est faux.** L'« administrateur système » ne veut rien de tel ; il a été choisi parce qu'il fallait remplir la case *En tant que*.
- **Le `afin de` a disparu.** C'est le seul segment qui porte le pourquoi, et c'est celui qu'on supprime en premier.
- **C'est une tâche déguisée.** Le contenu relève du modèle de données, donc de `data-model.md`, pas d'une story.

La même intention, correctement formulée :

> *En tant que responsable marketing, je veux savoir par quel client un nouvel inscrit a été recommandé, afin de récompenser ceux qui nous amènent du monde.*

Le stockage en base n'a pas disparu : il est **redescendu au niveau où il appartient**, la tâche technique. Et la story exprime maintenant un bénéfice discutable, arbitrable, priorisable.

> [!affirmation] Affirmation
> Le test le plus rapide reste celui de la [valeur]({{< relref "philosophie/pourquoi_agile/produire_valeur/index" >}}) : si personne ne peut expliquer à qui la story profite, ce n'est pas une story.

Pourquoi les outils commettent-ils systématiquement cette erreur ? Parce qu'un LLM a lu des milliers de tickets Jira mal écrits, et qu'il reproduit la **forme** (`En tant que… je veux… afin de…`) sans la **fonction** (exprimer un bénéfice utilisateur). Le gabarit est trivial à imiter ; l'intention ne l'est pas.

C'est ce qui rend le [User Story Mapping]({{< relref "pratiques/user_stories/user_stories_mapping/index" >}}) plus utile que jamais : il part des utilisateurs et de leurs activités, donc il **impose** l'ancrage dans la valeur d'usage, là où une génération descendante depuis un PRD technique produit des tâches déguisées.

## Ce que l'humain garde

Si l'agent écrit le code, découpe les tâches et rédige même des brouillons de stories, que reste-t-il ?

- **Choisir le problème.** Aucun outil ne dira quel problème mérite d'être résolu. C'est le travail de découverte produit, et c'est devenu le vrai goulot d'étranglement.
- **Arbitrer la valeur.** Décider ce qu'on ne fera pas.
- **Contester le plan.** Le découpage proposé par l'agent est plausible, pas pertinent. Le relire *contre* INVEST est une compétence, pas une formalité.
- **Écrire la Confirmation.** Les critères d'acceptation sont le seul endroit où l'exigence de qualité devient exécutable.
- **Mesurer l'[outcome]({{< relref "philosophie/pourquoi_agile/produire_valeur/output_vs_outcome" >}}).** Si produire est bon marché, livrer beaucoup ne prouve plus rien.

> [!affirmation] Affirmation
> Nous n'écrivions pas les spécifications parce que la conversation suffisait entre humains. Nous devons les écrire maintenant, non parce que l'agilité avait tort, mais parce qu'un des participants ne sait pas écouter.

