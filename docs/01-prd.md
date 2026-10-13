# PRD — Site du mariage de Laly & Vincent

## Résumé

Site web statique, en une seule page, qui centralise toutes les informations du mariage de Laly et Vincent (1er mai 2027, Domaine du Prieuré Saint Pierre, Montjoyer) pour éviter aux invités de poser des questions répétées.

## Utilisateurs

- **Invités** : consultent le site via le lien partagé par les mariés. Aucune connexion, aucun compte.
- **Laly & Vincent** : seuls éditeurs du site. Ils modifient directement le code source (pas d'interface d'administration).

## Fonctions

| Fonction | Ce qu'elle fait | État |
|---|---|---|
| Compte à rebours | Affiche en direct le temps restant avant le 1er mai 2027 15h00 | Terminé |
| Ajout à l'agenda | Bouton qui ouvre Google Calendar pré-rempli avec l'événement | Terminé |
| Programme | Détaille les horaires du samedi (cérémonie, cocktail, dîner, soirée) et du dimanche (brunch) | Terminé |
| Infos pratiques du lieu | Parking, hébergement sur place, transport, liste de gîtes à proximité (coordonnées, distance), liens d'itinéraire Google Maps | Terminé |
| Dress code | Présente la palette de couleurs du mariage ; précise d'éviter le blanc et le noir | Terminé |
| RSVP | Bouton qui renvoie vers un formulaire Google Forms externe | Terminé |
| Cadeaux | Indique l'absence de liste de mariage et la présence d'une cagnotte sur place | Terminé |
| FAQ | Répond à 6 questions fréquentes (enfants, horaire d'arrivée, pluie, allergies, parking, musique) | Terminé |
| Galerie photo | Protège l'accès aux photos par un code ; une fois le bon code saisi, affiche un lien vers un album externe | **En attente** — le mécanisme (code + déverrouillage) est fonctionnel, mais le lien de l'album (`ALBUM_URL`) est un placeholder tant que les photos du mariage ne sont pas disponibles. La fonction sera considérée terminée une fois ce lien renseigné. |
| Contact | Numéros de téléphone de Laly et Vincent, cliquables (`tel:`) | Terminé |
| Mentions légales & confidentialité | Informe sur la nature privée du site et l'absence de collecte de données propre au site | Terminé |
| Référencement (SEO) | Rend le site trouvable sur une recherche du type "mariage Laly et Vincent" : balises meta, données structurées (Event, FAQPage), sitemap, vérification Google Search Console | Terminé |

## Hors périmètre

- Le site ne stocke et n'affiche aucune réponse RSVP : les réponses existent uniquement dans le Google Form externe, consultable via le compte Google des mariés.
- Pas de compte invité, pas de connexion, pas d'espace personnalisé par invité.
- Pas d'interface d'administration : toute modification passe par l'édition du code source.
