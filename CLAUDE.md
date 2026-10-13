# CLAUDE.md

Site du mariage de Laly & Vincent — page unique statique (HTML/CSS/JS, aucun framework, aucun build).

## Documentation du produit

Avant toute modification, lire les documents du dossier `docs/` :

1. [`docs/01-prd.md`](docs/01-prd.md) — ce que fait le produit, fonction par fonction.
2. [`docs/02-app-flow.md`](docs/02-app-flow.md) — les pages (sections) et ce qui se passe au clic.
3. [`docs/03-design.md`](docs/03-design.md) — couleurs, polices, allure de chaque page.
4. [`docs/04-trd.md`](docs/04-trd.md) — la stack et les services utilisés.
5. [`docs/05-backend.md`](docs/05-backend.md) — les données personnelles, leur emplacement, les accès.
6. [`docs/06-plan.md`](docs/06-plan.md) — ce qui a été construit et ce qu'il reste à construire, dans l'ordre.

## Règle impérative

**N'implémenter aucune fonctionnalité absente de `docs/01-prd.md`.**

Si une demande porte sur une fonctionnalité qui n'est pas listée dans le PRD : ne pas coder. Le signaler, et proposer de mettre à jour `docs/01-prd.md` en premier (avec confirmation de Laly ou Vincent) avant d'écrire le moindre code.

## Repères pratiques

- `index.html` : tout le site (markup, styles, script).
- `assets/` : images.
- Code d'accès de la galerie photo et lien de l'album : variables `PHOTO_CODE` et `ALBUM_URL` tout en bas du `<script>` de `index.html`.
- Aucune étape de build : toute modification de `index.html` est live dès le `push` sur `main` (déploiement automatique GitHub Pages).
