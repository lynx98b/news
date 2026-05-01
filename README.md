# Bonjour le monde

Journal quotidien des bonnes nouvelles, des cinq continents.
Articles existants, repris et résumés. Toutes les nouvelles citent leur source.

## Structure

```
.
├── index.html          → page d'accueil (charge l'édition du jour)
├── archives/           → toutes les éditions précédentes
│   ├── n000.html
│   └── n001.html
├── assets/
│   ├── style.css       → feuille de style partagée
│   └── img/            → photos téléchargées
└── data/
    └── editions.json   → index des éditions (alimente la nav)
```

## Fonctionnement

- `index.html` lit `data/editions.json` et charge la **première édition** de la liste (la plus récente).
- Les **numéros précédents** sont listés en pied de page.
- Chaque édition est un fichier HTML autonome dans `archives/`.

## Génération automatique

Skill Claude Code : `bonjour-le-monde-journaliste`
Lancement quotidien via cron, push automatique sur GitHub Pages.

## Licence

Articles : tous sourcés. Photos : libres de droits (Wikimedia / Pexels).
