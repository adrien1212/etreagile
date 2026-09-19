+++
title = "Comment augmenter la productivité"
weight = 30
+++

> [!ressource] Ressource
> - [DevEx: What Actually Drives Productivity](https://queue.acm.org/doi/10.1145/3595878)
> - [The SPACE of Developer Productivity](https://queue.acm.org/doi/10.1145/3454122.3454124)
> - Rethinking Productivity in Software Engineering

La question de la productivité des développeurs me fascine depuis longtemps. L'article [The SPACE of Developer Productivity](https://queue.acm.org/doi/10.1145/3454122.3454124) y apporte une réponse d'ensemble : ses auteurs commencent par démystifier la notion de productivité — notamment l'idée qu'elle se réduirait à une mesure unique — puis proposent de l'observer à trois échelles : l'individu, l'équipe et le système.

J'étais parvenu de mon côté à un découpage analogue, et cette convergence me conforte dans sa pertinence : distinguer ces trois niveaux permet de clarifier les leviers d'action propres à chacun.

L'objectif de cet article est donc d'approfondir chacune de ces échelles, en m'appuyant sur l'ensemble des ressources rassemblées sur ce site.

---

## Définir la productivité dans le développement logiciel

Une première partie de la réponse dans [mesurer la productivité ?]({{< relref "regard_critique/mesurer_productivite/index" >}})

## L'équipe, l'unité de performance

C'est au niveau de l'équipe que se joue l'essentiel des écarts de
productivité. Jeff Sutherland, dans *Scrum: The Art of Doing Twice the Work
in Half the Time*, rapporte une étude menée auprès d'étudiants de Yale
(cf. `equipe_agile/constitution_equipe/orientee_equipe`) :

> In the Yale study, the fastest students outpaced their slow compatriots by
> a ratio of 10:1. Ten times faster! [...] It actually didn't take the slow
> team ten weeks to do what the best team could do in one week. Rather, it
> took them two thousand weeks! That's how great the difference is between
> the best and the worst. So where should you focus your attention? At the
> level of the individual, where you might be able to get an improvement of
> ten times if you can magically make all your employees geniuses? Or at the
> team level, boosting productivity by an enormous magnitude even if you
> merely make your worst teams mediocre[^sutherland]

L'écart passe ainsi d'un facteur 10 entre individus à plusieurs ordres de
grandeur entre équipes. Le rendement d'un effort porté sur l'individu est
donc faible au regard de ce qu'offre le collectif — et il suffit, comme le
souligne Sutherland, de faire passer les plus mauvaises équipes à un niveau
médiocre pour obtenir un gain considérable.

Ce constat n'est pas récent. Driskell et Salas établissaient dès les années
1990 qu'une équipe fonctionnant comme une unité cohésive surpasse largement
une somme d'individus dès lors que la tâche est intensive en connaissances
et en résolution de problèmes[^driskell] — soit exactement la nature du
travail de développement logiciel.

> that teams working as a cohesive unit perform far better than collections of individuals (CITATION DE TT -> aller chercher dans article source)

Cette centralité de l'équipe se lit dans l'histoire des méthodes
elles-mêmes. Scrum revendique sa filiation avec *The New New Product
Development Game* de Takeuchi et Nonaka[^takeuchi], dont l'apport ne porte
pas sur un processus mais sur les caractéristiques des équipes qui
réussissent : auto-organisation, phases de développement qui se chevauchent
plutôt qu'elles ne se succèdent, apprentissage transverse, et un contrôle
managérial discret plutôt que directif. L'Extreme Programming, sans se
réclamer des mêmes sources, aboutit à des pratiques convergentes — propriété
collective du code, programmation en binôme — qui reposent toutes sur le
collectif et non sur la performance individuelle.

Voyons maintenant quelles actions concrètes peuvent être mise en place pour faciliter et augmenter la productivité d'une équipe

### Pluridsciplinarité et autonomie
Sutherland, reprenant les caractéristiques dégagées par Takeuchi et Nonaka,
retient trois traits des équipes qui réussissent. Deux d'entre eux
relèvent directement de ce qu'un collectif peut travailler lui-même.

#### L'autonomie

> The teams are self-organizing and self-managing, they have the power to
> make their own decisions about how they do their jobs, and are empowered
> to make those decisions stick.[^sutherland]

L'autonomie porte moins sur *ce que* l'équipe produit que sur la façon dont
elle s'organise pour le produire : choix des pratiques, répartition du
travail, arbitrages techniques. Elle suppose deux conditions distinctes,
qu'on confond souvent : disposer du pouvoir de décider, et disposer des
moyens matériels d'exécuter la décision. Une équipe à qui l'on reconnaît le
premier sans lui donner le second n'est autonome qu'en apparence.

Son effet sur la productivité passe principalement par la réduction du
délai de décision : chaque arbitrage qui doit remonter puis redescendre une
chaîne hiérarchique immobilise le travail en cours. L'autonomie supprime
ces temps d'attente, et ouvre par ailleurs un espace d'expérimentation dont
l'équipe est la mieux placée pour tirer parti.

#### La pluridisciplinarité

> The teams have all the skills needed to complete the project. Planning,
> design, production, sales, distribution. And those skills feed and
> reinforce each other.[^sutherland]

Il faut distinguer ici deux choses. Réunir les compétences nécessaires est
une décision de conception organisationnelle, qui échappe à l'équipe — nous
y reviendrons. En revanche, faire circuler ces compétences une fois
réunies est bien à sa main : une équipe formellement pluridisciplinaire
peut parfaitement reconstituer des silos en interne, si chacun s'en tient à
sa spécialité et n'est sollicité qu'à son tour.

C'est cette circulation que décrit un ingénieur de Canon cité par Takeuchi
et Nonaka :

> When all the team members are located in one large room, someone's
> information becomes yours, without even trying. You then start thinking in
> terms of what's best or second best for the group at large and not only
> where you stand.[^takeuchi]

Le mécanisme décrit est double : la connaissance se diffuse sans effort
délibéré, et le critère de décision se déplace de l'intérêt individuel vers
celui du collectif. C'est là que se joue la rupture avec le
fonctionnement en silos — non dans l'organigramme, mais dans la manière
dont l'information et la responsabilité se partagent au quotidien.

### Autres à aborder
- loi de little et WIP
- leadtime


## Le système 

Ce résultat déplace la question plutôt qu'il ne la résout. Si l'on peut
transformer une équipe en agissant sur son fonctionnement interne
— confiance, cohésion, rituels —, ces leviers atteignent vite une limite :
ils ne changent rien à ce que l'équipe a le droit de faire, ni à ce dont
elle dépend pour livrer.

Trois contraintes en particulier échappent à l'équipe et relèvent du système
qui l'entoure.

**Sa frontière.** La loi de Conway veut qu'un système reproduise la
structure de communication de l'organisation qui le produit. Une équipe ne
peut donc être réellement pluridisciplinaire et autonome que si le
découpage de l'architecture le permet. Décider où passent ces frontières
n'est pas au pouvoir de l'équipe : c'est une décision de conception
organisationnelle.

**Sa capacité à livrer sans attendre.** Un cycle time court n'est pas une
qualité que l'équipe se donne, c'est la conséquence d'un système où elle
dépend de peu d'acteurs pour mettre en production. Chaque dépendance
externe — validation, environnement partagé, équipe tierce — allonge le
délai indépendamment de la qualité du collectif.

**Le cadre dans lequel elle opère.** La culture d'entreprise détermine ce
qui est permis : droit à l'erreur, transparence sur les incidents, réel
mandat de décision. C'est la contrainte la plus lente à faire évoluer, et
celle sur laquelle une équipe isolée a le moins de prise.

Reste alors la question difficile : par quels moyens concrets agir sur ce
système ?


### Sa frontière

La [loi de Conway]({{< relref "equipe_agile/constitution_equipe/conway_law" >}}) est
souvent citée comme une curiosité. C'est en réalité une contrainte de conception.

> Any organization that designs a system (defined broadly) will produce a design
> whose structure is a copy of the organization's communication structure.

Son effet sur la productivité est indirect, mais il se mesure. Un découpage en
[silos techniques]({{< relref "equipe_agile/constitution_equipe/equipe_independante/silo" >}})
— une équipe frontend, une équipe backend, une équipe base de données — paraît
rationnel : chacun reste dans sa spécialité. Mais toute fonctionnalité un peu
large traverse les trois. Il faut alors coordonner trois plannings, et le délai
d'implémentation s'allonge d'autant.

Le mécanisme est décrit dans *Building Evolutionary Architecture* :

> Teams typically optimize for efficiency for their immediate tasks rather than
> the more abstract, strategic goals of the business, particularly when under
> schedule pressure. Instead of delivering an end-to-end feature value, teams
> often focus on delivering components that may or may not work well with each
> other.[^conway]

Chaque équipe optimise ce qu'on lui demande, et personne ne répond du résultat de
bout en bout. Le découpage ne crée pas seulement de l'attente : il déplace la
responsabilité hors de portée de ceux qui font le travail.

Le levier existe, mais il ne se situe pas dans l'équipe. Puisque l'architecture
reproduit l'organisation, on peut renverser la relation et structurer les équipes
à l'image de l'architecture visée.

> Change the communication patterns of the designers to encourage the desired
> software architecture.

*Accelerate* précise ce que cela suppose techniquement : une architecture
faiblement couplée, où chaque module est testable et déployable indépendamment,
ce qui augmente à la fois le débit et la stabilité du système. Le découpage en
*bounded contexts* et le déploiement indépendant ne sont pas des raffinements
d'architecte ; ce sont les conditions matérielles de l'autonomie décrite plus haut.

Avant d'en arriver à une réorganisation, un diagnostic plus modeste reste
possible. Strode et Huff distinguent trois types de
[dépendances]({{< relref "equipe_agile/constitution_equipe/equipe_independante/dependance_equipe" >}})
entre équipes : de connaissance, de tâche et de ressource. Toutes ne se
suppriment pas, et certaines se justifient. Mais on ne traite que ce qu'on a
nommé.

### Sa capacité à livrer sans attendre

La question à poser n'est pas « à quelle vitesse travaillons-nous ? » mais « où
passe le temps ? ». La [Value Stream Map]({{< relref "philosophie/philosophie_lean/value_stream_map" >}})
répond à la seconde en distinguant deux durées : le temps de traitement, pendant
lequel quelqu'un travaille effectivement sur l'élément, et le temps écoulé, qui
court de l'entrée à la sortie de l'étape, attentes comprises. L'écart entre les
deux est le temps passé en file d'attente. Le rapport entre ces deux durées donne l'efficacité du flux.

La conséquence est brutale pour qui cherche à améliorer la productivité en
demandant aux gens d'aller plus vite : cet effort porte sur les 10 % du temps où
l'on travaille, et laisse intacts les 90 % où l'on attend. Diviser par deux le
temps de développement d'une fonctionnalité qui met trois mois à sortir ne fait
gagner que quelques jours.

Reste à comprendre pourquoi ces files se forment. La réponse n'est pas le manque
de compétence, mais le taux d'occupation. C'est ce que le Lean affirme depuis
l'origine à propos du [flux tiré]({{< relref "philosophie/philosophie_lean/toyota_production_system/just_in_time" >}}) :
une équipe occupée à 100 % du temps n'est pas un objectif, c'est un symptôme. Le
[vocabulaire du Lean]({{< relref "philosophie/philosophie_lean/toyota_production_system/vocabulaire" >}})
le formule en termes de causalité : la surcharge (*muri*) est la cause, le
gaspillage (*muda*) n'en est que le symptôme. S'attaquer directement au second
donne peu de résultats.

Trois leviers en découlent, et aucun ne relève de la bonne volonté du collectif.

**Limiter le travail en cours.** Une
[limite de WIP]({{< relref "frameworks/framework_kanban/principes" >}}) réduit le
nombre de tâches menées simultanément, donc le multitâche. Son intérêt principal
est cependant ailleurs : elle introduit une tension qui rend les blocages
visibles. Quand le flux ralentit ou s'arrête, c'est le système qui signale un
problème, non une personne.

**Réduire la taille des lots.** Livrer vite n'est pas travailler plus, c'est
[réduire la taille des lots]({{< relref "philosophie/philosophie_lean/lean_software_development/les_six_autres" >}})
pour raccourcir la boucle de retour. Un petit lot traverse la chaîne plus vite,
échoue moins cher, et se corrige plus tôt.

**Rendre les files visibles.** Le
[management visuel]({{< relref "pratiques/planifier/pilotage/management_visuel" >}})
n'a pas pour objet de suivre l'avancement mais de montrer où le travail stagne.
*Accelerate* est explicite sur le fait que les deux premiers leviers ne produisent
leur effet qu'associés au troisième :

> The use of WIP limits and visual displays is well known in the Lean community.
> They are used to ensure that teams don't become overburdened. [...] It's only
> when they're combined with the use of visual displays and have a feedback loop
> from production monitoring tools back to delivery teams or the business that we
> see a strong effect. When teams use these tools together, we see a much
> stronger positive effect on software delivery performance.

Ces trois leviers ont un adversaire commun, et c'est le réflexe le plus naturel
de toute organisation : l'optimisation locale. Chaque service maximise son propre
indicateur — taux d'occupation, tickets fermés, budget tenu — et la performance de
bout en bout se dégrade sans que personne n'en soit responsable. Une équipe de
développement à pleine capacité produit plus de code, donc allonge la file
d'attente de la recette.

> [!affirmation] Affirmation
> Optimiser la productivité de chaque étape dégrade le résultat de l'ensemble.
> C'est la raison pour laquelle le [débit]({{< relref "regard_critique/mesurer_productivite/debit_vs_productivite" >}}),
> mesuré de bout en bout, est un meilleur indicateur que la productivité mesurée
> étape par étape.

### Une culture générative

Les deux contraintes précédentes se corrigent par des décisions de conception. La
troisième est d'une autre nature : elle détermine ce qu'il est permis de faire, et
elle ne se décrète pas.

Les travaux de Westrum, repris par *Accelerate*, distinguent trois
[types de culture]({{< relref "equipe_agile/culture/index" >}}) : politique,
bureaucratique et générative. La conclusion des auteurs est présentée comme un
résultat de recherche, non comme une opinion :

> The organization's culture (*culture d'entreprise*) predicts software delivery
> performance and the success of the company as a whole.

Deux mécanismes expliquent ce lien, et tous deux passent par le délai.

Le premier est la [latence de décision]({{< relref "equipe_agile/culture/decision_latency" >}}) :
le temps qui s'écoule entre le moment où une décision doit être prise et celui où
elle l'est effectivement.

> Most of those decisions are trivial and easy. But if you have a rigid,
> hierarchical process where decisions have to go up the chain to be approved and
> then flow back down, that journey takes a long time.

Pendant ce trajet, le travail est immobilisé. Ce n'est pas un coût de réflexion,
c'est un coût de structure.

Le second est la [sécurité psychologique]({{< relref "equipe_agile/culture/psychological_safety" >}}).
Une équipe qui craint les conséquences d'un signalement ne signale pas. Les
dépendances, les blocages et les défauts restent invisibles jusqu'à ce qu'ils
coûtent cher. À l'inverse, une culture de confiance réduit le délai de livraison
parce que les problèmes remontent tôt.

Reste la question laissée ouverte plus haut : par quels moyens concrets agir sur
un système que l'équipe ne contrôle pas ? La réponse la plus utile est
contre-intuitive. Elle vient de l'épisode NUMMI, où une usine reprise avec les
mêmes ouvriers est devenue en deux ans l'une des meilleures du groupe :

> Ce que mon expérience NUMMI m'a appris, c'est que la façon de changer la culture
> d'une organisation **n'est pas de commencer par changer la façon dont les gens
> pensent, mais plutôt de commencer par changer la façon dont les gens se
> comportent – ce qu'ils font**.

*Accelerate* aboutit au même ordre de causalité, en sens inverse de celui qu'on
suppose habituellement : ce ne sont pas les convictions qui produisent les
pratiques, ce sont les pratiques qui produisent la culture.

> If you want to improve your culture, implementing CD practices will help. By
> giving developers the tools to detect problems when they occur, the time and
> resources to invest in their development, and the authority to fix problems
> straight away, we create an environment where developers accept responsibility
> for global outcomes such as quality and stability.

On ne commence donc pas une transformation par une déclaration d'intention sur la
confiance ou l'autonomie. On la commence par des pratiques techniques qui
raccourcissent les boucles — intégration continue, déploiement automatisé, limites
de WIP, tableau visible — et la culture suit. C'est aussi le seul chemin qui soit
partiellement à la main d'une équipe : elle ne peut pas décréter son périmètre,
mais elle peut souvent automatiser sa chaîne.

Cela ne dispense pas le management de sa part. Une équipe qui produit à chaque
[rétrospective]({{< relref "philosophie/pourquoi_agile/proprietaire_processus" >}})
des actions qu'elle n'a pas le pouvoir d'appliquer ne fabrique pas de
l'amélioration, elle fabrique du cynisme.

## L'individu

Nous avons commencé par écarter le niveau individuel, en nous appuyant sur
l'étude de Yale : les écarts y sont d'un facteur dix, contre plusieurs ordres de
grandeur entre équipes. Ce raisonnement reste valable pour décider *où investir*.
Il ne conclut pas que ce niveau est sans objet.

Deux raisons de le traiter malgré tout. La première est que les auteurs de SPACE
en font une composante à équilibrer, et non une variable d'ajustement :

> While individual performance is important, contributing to the success of the
> team is also critical to measuring productivity. Measures of performance that
> balance the developer, team, and organization are important.

La seconde est que ce niveau est le seul que la personne concernée éprouve
réellement. Une équipe ne ressent rien ; un développeur, si.

> By remembering that developer productivity is personal, developers can leverage
> it to gain insights into their work so they can take control of their time,
> energy, and days. For example, research has shown that high productivity is
> highly correlated with feeling satisfied and happy with work. Finding ways to
> improve productivity is also about finding ways to introduce more joy, and
> decrease frustration, in a developer's day.

Le sens de la relation mérite d'être noté. La corrélation relevée va de la
satisfaction vers la productivité. Le confort du développeur n'est pas la
récompense d'une performance obtenue ; il en est une condition.

Il faut cependant nommer d'emblée la limite de ce niveau d'analyse. Presque tous
les leviers qui suivent sont **subis** par l'individu : il ne choisit ni son
outillage, ni le nombre de projets qu'on lui confie, ni la clarté des demandes
qu'il reçoit. Ce sont donc, pour l'essentiel, des leviers de management dont
l'individu est le bénéficiaire.

### L'expérience du développeur

La notion est définie sur ce site à propos de la distinction entre
[développeur et exécutant]({{< relref "equipe_agile/roles_postures/developpeur_executant/index" >}}) :

> [!definition] Developer Experience
> Developer Experience (DX) décrit les interactions et les sentiments qu'éprouve
> un développeur lorsqu'il travaille avec un corps de code afin d'atteindre un
> objectif spécifique.

Ce qui la compose est prosaïque : un ordinateur adéquat, une gestion de projet
organisée, un code que l'on peut modifier sans crainte. Rien qui figure dans un
plan de transformation.

L'intérêt de la notion tient à ce qu'elle rend cumulable. Quand l'environnement
n'est pas à la hauteur, les développeurs compensent, et cette compensation
s'accumule sous la forme d'une **dette de motivation**. Le mécanisme est celui de
la [dette technique]({{< relref "philosophie/pourquoi_agile/produit_haute_qualite/qualite_logicielle/dette_technique" >}}) :
on emprunte à une capacité future pour tenir un engagement présent, et le
remboursement est d'autant plus coûteux qu'il est différé.

C'est ce qui rend ce niveau invisible aux indicateurs habituels. Une équipe peut
afficher six mois de livraisons régulières tout en épuisant la santé de son code,
sa connaissance partagée et l'énergie de ses membres. Ces variables sont des
stocks et non des débits : elles ne se dégradent pas à l'échelle du trimestre,
mais à celle de l'année.

*Accelerate* vérifie que l'attention portée aux personnes n'est pas un supplément
d'âme :

> When leaders invest in their people and enable them to do their best work,
> employees identify more strongly with the organization and are willing to go
> the extra mile to help it be successful

### L'absence d'interruption

Le travail de développement suppose de tenir en mémoire un modèle du problème.
Une interruption détruit ce modèle, et le reconstituer coûte davantage que la
durée de l'interruption elle-même.

Le Lean range ce coût parmi les
[gaspillages]({{< relref "philosophie/philosophie_lean/lean_software_development/elimine_gaspillage" >}}),
sous le nom de changement de tâche :

> Lorsque les personnes sont affectées à plusieurs projets ou chaînes de valeur,
> elles doivent sans cesse changer de contexte et gérer les dépendances, ce qui
> ajoute du travail et du temps supplémentaire.

La mesure la plus citée sur ce point est ancienne : Clark et Wheelwright ont
observé en 1993 que le temps qu'un individu consacre à un travail à valeur ajoutée
diminue rapidement dès lors qu'il travaille sur plus de deux tâches.

Ce constat donne au niveau individuel son articulation avec le reste de l'article.
L'interruption n'est pas un défaut d'hygiène personnelle : c'est le symptôme, à
hauteur d'individu, d'un excès de travail en cours à hauteur de système. On ne la
traite donc pas en demandant aux gens de mieux se concentrer, mais en
[limitant le WIP]({{< relref "frameworks/framework_kanban/principes" >}}) et en
réduisant le nombre de projets simultanés. Le levier est le même que celui de la
partie précédente ; seul l'endroit où l'on en ressent l'effet a changé.

### L'autonomie de réalisation

L'autonomie a déjà été traitée au niveau de l'équipe. Elle a un pendant
individuel, que la page
[Agile qu'avec exécutants ?]({{< relref "regard_critique/agile_executants" >}})
formule comme une alternative entre deux styles de commandement :

> L'agilité consiste à adopter un commandement par objectif (voici l'effet
> souhaité) en lieu et place d'un commandement par ordre (voici la liste des
> actions à effectuer).

La différence n'est pas seulement affaire de confort. Un ordre transmet une
solution, un objectif transmet un problème. Dans le premier cas, l'intelligence de
celui qui exécute reste inemployée, et les défauts de la solution ne sont signalés
par personne, puisque personne ne se juge responsable de la solution. Dans le
second, elle est mobilisée.

La même page pose trois conditions, qui interdisent d'en faire une recette :

> - Il faut que le management adopte un style délégatif
> - Il faut que le collaborateur soit capable d'atteindre l'objectif fixé
> - Il faut que le collaborateur souhaite atteindre l'objectif fixé

La troisième est celle qu'on oublie. Tout le monde ne souhaite pas être acteur du
produit, et ce n'est pas nécessairement un défaut à corriger. Prescrire
l'autonomie à quelqu'un qui ne la demande pas produit de l'anxiété, pas de la
performance.

### La motivation

C'est le point le plus difficile à traiter honnêtement, parce que c'est celui où
la littérature de gestion produit le plus d'affirmations invérifiables.

Ce que l'on peut tenir se limite à deux éléments. D'abord la corrélation relevée
par SPACE entre satisfaction et productivité, citée plus haut. Ensuite le fait que
l'environnement pèse autant que l'outillage :

> While developer tools and workflows have a large impact on developer
> productivity, human factors such as environment and work culture have
> substantial impact too

#### Qu'est-ce qui nous motive ?

https://youtu.be/rrkrvAUbU9Y

Selon la Théorie de l'autodétermination (TAD) la motivation s'appuie sur trois besoins psychologiques :
- l'autonomie : que nous avons évoqué quelques paragraphe plus haut
- la compétence : le sentiment d'être bon dans ce que l'on fait
- l'appartenance sociale : le sentiment d'être connecté à d'autre personne

### La charge cognitive

Le dernier levier est le moins coûteux, et c'est sans doute pour cette raison
qu'on le néglige.

Une attente floue produit deux effets. Le premier est le retravail : on livre
autre chose que ce qui était attendu, et on recommence. Le second est plus
insidieux, et porte un nom.

> Work expands so as to fill the time available for its completion.[^parkinson]

La loi de Parkinson est généralement invoquée pour justifier des délais serrés.
Ce n'est pas son intérêt ici. Ce qu'elle décrit, c'est qu'en l'absence de critère
d'arrêt explicite, une tâche n'a pas de fin : on peut toujours peaufiner,
généraliser, anticiper un besoin futur. Le temps disponible devient alors le seul
critère d'arrêt, faute d'un meilleur.

C'est exactement la fonction de deux artefacts de Scrum dont l'intérêt est souvent
sous-estimé. La
[Definition of Done]({{< relref "frameworks/framework_scrum/artefact_engagements/definition_of_done" >}})
fournit le critère d'arrêt au niveau de la tâche : tests passés, critères
d'acceptation respectés, revue effectuée. Le
[Sprint Goal]({{< relref "frameworks/framework_scrum/artefact_engagements/sprint_goal" >}})
le fournit au niveau de l'itération, et sa première vertu revendiquée est
précisément la concentration :

> Concentration. Un objectif de sprint clair permet de décider ce qu'il est
> important d'aborder et ce qui ne l'est pas au cours du sprint.

Aucun des deux n'est un outil de contrôle. Ce sont des dispositifs qui déchargent
l'individu d'une décision qu'il n'a pas à prendre seul, et qui lui permettent de
savoir quand s'arrêter — ce qui est la condition pour commencer autre chose.




<!-- 

--- 


J'aime bien l'article [DevEx: What Actually Drives Productivity](https://spawn-queue.acm.org/doi/10.1145/3595878) et le schema sur les 3 axes



2. La théorie des files d'attente. Absente, et c'est probablement le modèle le plus explicatif du domaine. L'idée de Donald Reinertsen : le temps de cycle explose non-linéairement quand le taux d'utilisation approche 100%. Une équipe occupée à 95% a des délais catastrophiques comparée à une équipe occupée à 70%, même avec les mêmes compétences et le même outillage. Les leviers deviennent alors : réduire la taille des lots, limiter le travail en cours, rendre les files visibles. Rien de tout ça n'apparaît dans ton schéma, et rien de tout ça n'est intuitif si on raisonne en termes d'énergie ou de compétences individuelles.


3. Le temps, les stocks et la dette. Ton modèle est instantané. Or les variables décisives sont des stocks qui s'accumulent ou se dégradent : santé du code, connaissance partagée, capital de confiance, énergie des gens. Une équipe peut afficher six mois d'excellente « productivité » en détruisant sa capacité future. Sans boucle de rétroaction ni notion de stock, tu ne peux pas voir ça.

À ajouter dans le même esprit : la charge cognitive (Team Topologies), et le fait que les développeurs passent la majorité de leur temps à comprendre du code plutôt qu'à en écrire — une étude de terrain de Xia et al. (IEEE TSE, 2018) situe ça autour de 58%. Ça déplace complètement les leviers : la lisibilité et la documentation deviennent des variables de débit, pas de confort.



---

DRAFT


## Au niveau du système

## Au niveau de l'individu


Améliorer la productivité c'est 
- produire plus avec moins de ressource
- c'est produire la bonne chose (cf Output vs Outcome / build the right thing)

```
                    PRODUCTIVITÉ
                         │
          ┌──────────────┼──────────────┐
          │              │              │
          ▼              ▼              ▼
       INDIVIDU         ÉQUIPE        SYSTÈME

      énergie         collaboration     processus
      compétences     coordination      architecture
      attention       communication     tooling
      motivation      confiance         CI/CD
      autonomie       coût des interruptions     organisation
                      dream team                  La théorie des files d'attente
      clarté          entraide          silos (conway's law)
                      Output vs outcome
                      La diversité d'équipe. (pluridisciplinaire et autonomme)
          │              │              │
          └──────────────┼──────────────┘
                         ▼
                    VALEUR PRODUITE
```

Dans SPACE on peut lire myth2
> While individual performance is important, contributing to the success of the team is also critical to measuring productivity. Measures of performance that balance the developer, team, and organization are important.

Et myth 4
> By remembering that developer productivity is personal,7 developers can leverage it to gain insights into their work so they can take control of their time, energy, and days. For example, research has shown that high productivity is highly correlated with feeling satisfied and happy with work.12,20 Finding ways to improve productivity is also about finding ways to introduce more joy, and decrease frustration, in a developer’s day.

Et myth 5 : l'environnement est important
> While developer tools and workflows have a large impact on developer productivity, human factors such as environment and work culture have substantial impact too


Important : 
comme évoqué dans orientee_equipe
- ratio de 200
- that teams working as a cohesive unit perform far better than collections of individuals  (Team Topologie)





## Ce que je te proposerais à la place

Une chaîne avec boucle plutôt que trois colonnes :

Sélection (fait-on la bonne chose ?) → Flux (files, WIP, taille des lots, goulot) → Capacité (stocks : santé du code, compétences, énergie, connaissance partagée) → Feedback (temps de cycle, apprentissage marché) → retour sur Sélection.

Tes trois axes deviennent alors des niveaux d'analyse qui traversent chaque étape, ce qu'ils sont vraiment.


[^sutherland]: Jeff Sutherland, *Scrum: The Art of Doing Twice the Work in Half the Time*, chapitre 3 « Team »
[^driskell]: Driskell and Salas, "Collective Behavior and Team Performance," 277–288 — cité dans *Team Topologies*, chapitre 3
[^takeuchi]: Hirotaka Takeuchi et Ikujiro Nonaka, "The New New Product Development Game", *Harvard Business Review*, 1986
[^conway]: *Building Evolutionary Architecture*, p. 11-12

-->