<div align="center">

# AstroBlog

Des récits, des tutoriels et des expérimentations front-end propulsés par Astro.

</div>

## ✨ Aperçu

- Pages statiques générées avec [Astro 5](https://astro.build/)
- Mise en page responsive (Hero, grille d’articles, pages Markdown)
- Thème clair/sombre persistant, géré côté client
- Styles modulaires en Sass (tokens, base, layout, composants)
- Support complet des métadonnées pour les articles (OpenGraph, description, etc.)

## 📁 Structure

```
root/
├── public/              # Assets statiques servis tels quels
├── src/
│   ├── components/      # Header, Navigation, cartes, etc.
│   ├── layouts/         # BaseLayout, layout Markdown custom
│   ├── pages/           # Pages Astro + articles Markdown
│   ├── scripts/         # JS côté client (si nécessaire)
│   └── styles/          # Sass (tokens, base, layout, components)
├── package.json
└── astro.config.mjs
```

## 🛠️ Commandes

| Commande              | Action                                      |
| --------------------- | ------------------------------------------- |
| `npm install`         | Installe les dépendances                    |
| `npm run dev`         | Lance le serveur de dev sur `localhost:4321`|
| `npm run build`       | Génère la version production (`dist/`)      |
| `npm run preview`     | Prévisualise la build production            |

## 📝 Contenu

- `src/pages/blog.astro` : index des articles, triés par date ISO
- `src/pages/posts/*.md` : contenu éditorial (frontmatter complet)
- `src/layouts/MarkDownPostLayout.astro` : template dédié aux articles (Hero + SEO)

## 🌗 Thème

Le bouton de bascule applique un attribut `data-theme="light"` sur `<html>` et persiste le choix via `localStorage`. Les couleurs, ombres et espacements proviennent de `src/styles/tokens/_variables.scss`.

## ✅ Bonnes pratiques

- Encodage UTF-8 pour tous les fichiers afin de préserver les accents
- Dates en format ISO (`YYYY-MM-DD`) pour éviter toute ambigüité
- Accessibilité : libellés ARIA explicites et texte alternatif cohérent

## 📄 Licence

Projet pédagogique. Reprenez ce modèle librement en créditant AstroBlog.
