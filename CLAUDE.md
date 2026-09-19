# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Nature du dépôt

Fork de **Quartz v5** (`upstream` = `jackyzha0/quartz`) utilisé pour publier le cours « Être Agile »
sur etreagile.fr. Deux natures de travail y cohabitent :

- `content/` — le cours lui-même, ~235 pages Markdown en français. C'est là que se fait l'essentiel du travail.
- `quartz/` — le moteur de site amont (TypeScript / Preact). Toute modification ici complique les merges
  avec `upstream` : préférer `quartz.config.yaml` et `quartz/styles/custom.scss` pour personnaliser.

Branche principale : `v5` (et non `main`).

## Commandes

```bash
npx quartz build --serve     # build + serveur local avec hot-reload — usage quotidien
npx quartz build             # build de production vers public/
npx quartz plugin install    # installe les plugins de quartz.lock.json dans .quartz/plugins/ (non versionné)
npm run check                # tsc --noEmit + prettier --check — ce que la CI exécute
npm run format               # prettier --write
npm run test                 # tsx --test
npx tsx --test quartz/<chemin>/<fichier>.test.ts   # un seul fichier de test
```

Node ≥ 22. `npm run docs` sert la documentation Quartz amont (`docs/`), pas le site.

## Architecture

**Configuration déclarative.** Tout passe par `quartz.config.yaml` (v5 — il n'y a pas de
`quartz.config.ts` comme en v4) :

- `configuration:` — titre, `locale: fr-FR`, `baseUrl`, typographie et couleurs clair/sombre.
- `plugins:` — liste de paquets `@quartz-community/*` avec `enabled`, `order`, `options`, `layout`.
  Activer ou désactiver une fonctionnalité = basculer `enabled` ici, pas éditer du code.
- `layout:` — positions des composants par type de page (`content`, `folder`, `tag`, `404`…).

**Pipeline de build.** `quartz/bootstrap-cli.mjs` → `quartz/build.ts` → transformers / filters /
emitters fournis par les plugins ; rendu par les composants Preact de `quartz/components/`.

**Plugins dont dépendent les conventions du contenu :**

- `ox-hugo` — résout les shortcodes `{{< relref >}}`.
- `obsidian-flavored-markdown` — callouts et wikilinks.
- `note-properties` — configuré en `delimiters: +++`, `language: toml`, d'où le front-matter TOML.

**Déploiement.** `.github/workflows/deploy.yaml` : push sur `v5` → build → GitHub Pages. Les autres
workflows (`ci.yaml`, `build-preview.yaml`, `deploy-preview.yaml`…) sont gardés par
`if: github.repository == 'jackyzha0/quartz'` et ne tournent donc pas sur ce fork.

## Conventions de contenu (`content/`)

Front-matter **TOML** entre `+++` (pas YAML, malgré le défaut de Quartz) :

```toml
+++
title = "Framework XP"
description = "…"   # sert aussi aux métadonnées OG
weight = 10         # ordre dans l'explorer
comments = true
+++
```

- **Liens internes** : `[Texte]({{< relref "dossier/page" >}})` — jamais de wikilink `[[…]]` ni de
  chemin `.md`. ~440 occurrences dans le contenu.
- **Structure** : un dossier = un chapitre, avec son `index.md`. Images dans le sous-dossier
  `images/` du chapitre, référencées en relatif : `![Alt](fichier.png)`.
- **PDF** : fichier sous `quartz/static/pdf/…`, intégré par
  `<embed src="/static/pdf/…" width="100%" height="500px"/>`.
- **Callouts maison**, définis uniquement dans `quartz/styles/custom.scss` : `[!ressource]`
  (liste des sources, en tête de page), `[!affirmation]`, `[!definition]` — en plus des standards
  `[!danger]`, `[!warning]`, `[!note]`, `[!example]`.
- Contenu rédigé en français ; les citations d'ouvrages restent dans leur langue d'origine (anglais).
- `MANQUES.md` (non versionné) est l'analyse éditoriale des lacunes du recueil — utile pour situer
  le travail en cours.

## Travail rédactionnel

L'auteur rédige lui-même. Sur les pages de `content/`, proposer des pistes, des plans, des angles ou
des formulations ; ne pas produire de texte fini à coller sans qu'il l'ait explicitement demandé.
