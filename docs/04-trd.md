# TRD — Stack et services

## Frontend

- HTML5 + CSS3 (styles en ligne + un bloc `<style>` global) + JavaScript vanilla (ES5/ES6).
- Aucun framework, aucun bundler, aucun gestionnaire de paquets : pas de `package.json`, pas de `node_modules`, pas d'étape de build.
- Un seul fichier `index.html` à la racine, plus un dossier `assets/` pour les images.

## Hébergement et déploiement

- **Hébergement** : GitHub Pages.
- **Dépôt** : `vincentmatray-69600/site-mariage`, branche `main`, contenu servi depuis la racine.
- `.nojekyll` présent : désactive le traitement Jekyll de GitHub Pages (site statique pur).
- **Déploiement** : automatique à chaque `push` sur `main`, via l'action GitHub "pages build and deployment". Pas de CI personnalisée, pas d'étape de test automatisé.
- **Domaine** : pas de nom de domaine personnalisé — le site reste sur `https://vincentmatray-69600.github.io/site-mariage/`.

## Ce qui n'existe pas

- Pas de backend, pas de serveur applicatif.
- Pas de base de données.
- Pas d'API.
- Pas d'authentification ni de compte utilisateur.
- Pas d'outil d'analytics ni de tracking (cohérent avec `confidentialite` dans le site : aucun cookie déposé).

## Services externes liés

Services non intégrés au site (pas d'appel API, pas de clé, pas de SDK) : simples liens sortants ou polices chargées.

| Service | Rôle | Intégration |
|---|---|---|
| Google Fonts | Police Fraunces + Work Sans | `<link>` vers `fonts.googleapis.com` / `fonts.gstatic.com`, chargement asynchrone |
| Google Calendar | Bouton "Ajouter à mon agenda" | Lien `calendar.google.com/calendar/render?...` pré-rempli |
| Google Maps | Boutons "Itinéraire" | Liens `google.com/maps/search/?...` |
| Google Forms | Formulaire RSVP | Lien externe vers un formulaire existant, réponses non visibles depuis le site |
| Google Photos | Album photo du mariage | Lien externe, ajouté après le mariage dans la variable `ALBUM_URL` du code — [EN ATTENTE, cf. PRD] |
| Google Search Console | Suivi du référencement (indexation, sitemap, données structurées) | Outil de supervision externe, aucune intégration dans le code du site hormis le fichier de vérification `googleb3fba4beb249fbe8.html` et `sitemap.xml` |
