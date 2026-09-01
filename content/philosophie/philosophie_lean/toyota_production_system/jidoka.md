+++
title = "Jidoka"
description = "Le Jidoka consiste à arrêter le travail dès qu'un problème apparaît, pour construire la qualité dans le produit plutôt que la contrôler après."
weight = 10
+++


> [!ressource] Ressources
> - [Comprendre le TPS #1 : le Jidoka (ou mise en évidence des obstacles)](https://blog.toyota-forklifts.fr/comprendre-tps-jidoka)
> - [Le jidoka appliqué au domaine logiciel](https://leblogdulean.com/2023/07/06/le-jidoka-applique-au-domaine-logiciel-pas-de-craftmanship-sans-respect/)
> - [Le lean sans le Jidoka n’est que du fordisme](https://www.institut-lean-france.fr/le-lean-sans-le-jidoka-nest-que-du-fordisme/)

## Principes
Le principe du Jidoka consiste à arrêter le travail dès qu’un problème survient afin d’éviter toute production d’éléments défectueux. Cette approche repose sur la détection d’anomalie au sein même des processus permettant ainsi de construire la qualité dans le produit.
- Le premier axe consiste à régler les problèmes qualité au plus tôt
![detecter au plus tôt](detecter_tot.png)

- Le second axe consiste à revenir voire supprimer la non-qualité à la source

![jidoka principes](jidoka_principes.png)

## Les deux outils du Jidoka

Le principe « arrêter dès qu'un problème survient » suppose deux choses très concrètes : un moyen de signaler, et un moyen d'empêcher.

### L'andon — signaler l'arrêt

L'**andon** est le dispositif qui permet à n'importe quel opérateur d'alerter, voire d'arrêter la chaîne : à l'origine un cordon à tirer au-dessus du poste, aujourd'hui un bouton et un tableau lumineux.

Ce qui compte n'est pas le dispositif, c'est ce qu'il implique : **la personne la moins gradée de l'atelier a le pouvoir d'arrêter la production de l'usine entière**, et on attend d'elle qu'elle le fasse. Tirer le cordon n'est pas un aveu d'échec, c'est le comportement demandé.

> [!affirmation] Affirmation
> L'andon est un test de culture avant d'être un outil. Dans une organisation où signaler un problème expose celui qui le signale, personne ne tire le cordon — et les défauts continuent d'avancer. Voir [Psychological Safety]({{< relref "equipe_agile/culture/psychological_safety" >}}) et la [typologie de Westrum]({{< relref "equipe_agile/culture/index" >}}).

En développement logiciel, l'équivalent le plus direct est la **build cassée qui bloque la chaîne d'intégration** : tant qu'elle n'est pas réparée, plus personne ne livre, et la réparer devient la priorité de l'équipe.

### Le poka-yoke — empêcher l'erreur

Le **poka-yoke** (« détrompeur »), formalisé par **Shigeo Shingo**, consiste à concevoir les choses de telle sorte que l'erreur soit **impossible**, ou immédiatement visible. La prise USB-C qui s'insère dans les deux sens, la pompe à gasoil dont l'embout n'entre pas dans un réservoir à essence.

Le raisonnement est important : plutôt que de demander aux gens d'être plus attentifs — ce qui ne marche jamais durablement — on change le dispositif pour que l'inattention ne produise plus de défaut.

En logiciel, on en fait tous les jours sans le nommer :

- un **typage strict** qui rend un état invalide non représentable ;
- une **contrainte en base de données** plutôt qu'une vérification applicative qu'on oubliera ;
- un **test automatisé** qui échoue avant que le défaut n'atteigne la production ;
- un **linter** ou une revue obligatoire en *pipeline* plutôt qu'une consigne dans un document.

> [!definition] Le lien avec la qualité
> C'est exactement l'idée d'**intégrer la qualité dès la conception** plutôt que de la contrôler après coup — le troisième principe du [Lean Software Development]({{< relref "philosophie/philosophie_lean/lean_software_development/les_six_autres" >}}), et le fond du [Software Craftsmanship]({{< relref "pratiques/software_craftsmanship/index" >}}).

## Ne pas oublier le côté humain

« Développer les gens avant de produire des pièces », c'est l'aphorisme du Lean Management. 

> [!danger] Définition
>  Jidoka signifie *automatisation avec une touche d'humain*

> Personne ne comprend mieux les humains que les humains eux-mêmes, et le Jidoka est la clé pour en apprendre plus sur vos clients et créer des produits et services toujours meilleurs. [Le lean sans le Jidoka n’est que du fordisme](https://www.institut-lean-france.fr/le-lean-sans-le-jidoka-nest-que-du-fordisme/)

Les managers obsédés par l’excellence opérationnelle s’imaginent que le but de l’automatisation est d’éliminer les coûts liés aux « ressources humaines ». Ils rêvent de systèmes automatiques que leurs clients puissent utiliser sans avoir à parler à qui que ce soit. Puis, ils ne comprennent pas pourquoi les clients dénigrent leur offre, cherchent des alternatives et fuient leur marque le plus vite possible. En effet, pour chaque appareil/logiciel, il existe deux dimensions qui dépendent de facteurs humains :
- Le produit : L’outil mécanique que vous pouvez utiliser de façon autonome pour obtenir ce que vous désirez.
- Le service : La personne à qui vous souhaitez parler lorsque vous rencontrez des problèmes avec la machine.

Le service est essentiel, n’importe quel produit possède une composante de service qui lui est également rattachée. Il faut donc quelqu’un pour aider l’utilisateur pour :
- Utiliser la machine de la bonne façon pour obtenir les bons résultats en fonction du niveau de complexité de son utilisation.
- Réparer la machine lorsqu’elle tombe en panne.
- Améliorer la machine et trouver des modèles plus intelligents, plus simples à utiliser et plus esthétiques.

**L’intention du jidoka est de développer la part humaine d’un produit**

## Dans le monde logiciel ?
Si l’on s’intéresse au développement logiciel dans le monde moderne, en particulier dans le domaine des services numériques, il est marqué par une double exigence : 
- celle de l’automatisation, tirée par les contraintes de lead time 
- et celle de l’excellence des compétences, tirée par la complexité des domaines. 
  
On trouve deux expressions clés, celle de *DevOps* et de *software craftsmanship*, qui expriment cette complémentarité et tension.

On remarque également que de nombreux principes peuvent être appliqués au monde logiciel :
- le coût de découverte d'un bug en production est plus élevé que lors de la phase de développement
- l'amélioration continue et le partage sont des éléments essentiels pour la constitution d'équipes Agile
