+++
title = "Comment augmenter la productivité"
weight = 30
+++

# BROUILLON

> [!ressource] Ressource
> - [DevEx: What Actually Drives Productivity](https://spawn-queue.acm.org/doi/10.1145/3595878)
> - [The SPACE of Developer Productivity](https://spawn-queue.acm.org/doi/10.1145/3454122.3454124)
> - Rethinking Productivity in Sof tware Engineering

C'est une question qui m'a toujours fasciner. Grâce à ce receuil de ressource je commence à pouvoir y répondre avec une approche théorique.
D'autres personnes ont essayé d'y répondre 

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
      autonomie       interruptions     organisation
                                        La théorie des files d'attente
      clarté          entraide          silos (conway's law)
                      Output vs outcome
          │              │              │
          └──────────────┼──────────────┘
                         ▼
                    VALEUR PRODUITE
```

Important : 
comme évoqué dans orientee_equipe
- ratio de 200
- that teams working as a cohesive unit perform far better than collections of individuals  (Team Topologie)


J'aime bien l'article [DevEx: What Actually Drives Productivity](https://spawn-queue.acm.org/doi/10.1145/3595878) et le schema sur les 3 axes



2. La théorie des files d'attente. Absente, et c'est probablement le modèle le plus explicatif du domaine. L'idée de Donald Reinertsen : le temps de cycle explose non-linéairement quand le taux d'utilisation approche 100%. Une équipe occupée à 95% a des délais catastrophiques comparée à une équipe occupée à 70%, même avec les mêmes compétences et le même outillage. Les leviers deviennent alors : réduire la taille des lots, limiter le travail en cours, rendre les files visibles. Rien de tout ça n'apparaît dans ton schéma, et rien de tout ça n'est intuitif si on raisonne en termes d'énergie ou de compétences individuelles.


3. Le temps, les stocks et la dette. Ton modèle est instantané. Or les variables décisives sont des stocks qui s'accumulent ou se dégradent : santé du code, connaissance partagée, capital de confiance, énergie des gens. Une équipe peut afficher six mois d'excellente « productivité » en détruisant sa capacité future. Sans boucle de rétroaction ni notion de stock, tu ne peux pas voir ça.

À ajouter dans le même esprit : la charge cognitive (Team Topologies), et le fait que les développeurs passent la majorité de leur temps à comprendre du code plutôt qu'à en écrire — une étude de terrain de Xia et al. (IEEE TSE, 2018) situe ça autour de 58%. Ça déplace complètement les leviers : la lisibilité et la documentation deviennent des variables de débit, pas de confort.


## Ce que je te proposerais à la place

Une chaîne avec boucle plutôt que trois colonnes :

Sélection (fait-on la bonne chose ?) → Flux (files, WIP, taille des lots, goulot) → Capacité (stocks : santé du code, compétences, énergie, connaissance partagée) → Feedback (temps de cycle, apprentissage marché) → retour sur Sélection.

Tes trois axes deviennent alors des niveaux d'analyse qui traversent chaque étape, ce qu'ils sont vraiment.