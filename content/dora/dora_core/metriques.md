+++
title = "Métriques"
description = "Les métriques DORA : fréquence de déploiement, délai de livraison, taux d'échec des changements, temps de restauration et fiabilité."
weight = 10
+++

> [!ressource] Ressources
> - [Les DORA Metrics en 2024, c’est pas comme dans Accelerate en 2018](https://youtu.be/oKg470VioJ8)
> - [Les DORA Metrics, oui mais pour quoi faire ?](https://substack.jp-lambert.com/p/les-dora-metrics-oui-mais-pour-quoi?r=46wwe&triedRedirect=true)

## Deployments Frequency
> 2018 et 2024 identiques

## Lead Time for Change (LTC)
> 2018 renommé en *Change Lead Time* (CLT) 2024

## Change Failure Rate (CFR)
> 2018 renommé en *Change Fail Percentage* (CLT) 2024

## Mean Time To Restore (MTTR)
> 2018 et devient Failed Deployment Recovery Time (FDRT) 2024

- FDRT se concentre sur la capacité d'une équipe à gérer les échecs lors des déploiements et à voir en combien de temps nous revenons dans un état stable (uniquement rollback à une v-1)
- Le MTTR était plus global en incluant toutes les causes d'incidents (bugs, problème infrastructure)
