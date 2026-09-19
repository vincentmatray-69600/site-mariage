# site-mariage

Le site du mariage de Laly &amp; Vincent — 1er mai 2027, Domaine du Prieuré Saint Pierre (Montjoyer).

Page statique unique (`index.html` + dossier `assets/`), sans dépendance externe autre que Google Fonts. Programme, infos pratiques, RSVP, FAQ, et une galerie photo protégée par un code.

## Aperçu en local

Ouvrez simplement `index.html` dans un navigateur, ou servez le dossier avec n'importe quel serveur statique.

## Hébergement (GitHub Pages)

Dans les réglages du dépôt : **Settings → Pages**, source **Deploy from a branch**, branche `main`, dossier `/ (root)`. Le site sera ensuite disponible à une adresse du type `https://vincentmatray-69600.github.io/site-mariage/`.

## À modifier vous-même après le mariage

Dans `index.html`, tout en bas du fichier, deux lignes sont prévues pour ça :

```js
var PHOTO_CODE = "PRIEURE1MAI";
var ALBUM_URL = "#"; // remplacez "#" par le lien de l'album (Google Photos, etc.)
```

- `PHOTO_CODE` : le code communiqué aux invités pour accéder à la galerie.
- `ALBUM_URL` : le lien vers l'album en ligne (Google Photos partagé, galerie de la photographe...) une fois les photos disponibles.

Le lien RSVP (`href` de la section RSVP) et le lien vers l'album pour les FAQ/mentions légales peuvent être modifiés directement dans le HTML si besoin.
