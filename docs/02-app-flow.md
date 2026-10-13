# App Flow — Site du mariage de Laly & Vincent

Site à page unique. Les "pages" ci-dessous sont des sections ancrées de cette même page, atteintes par clic sur la nav ou défilement.

## Navigation globale

- Barre de navigation fixe en haut, visible sur toutes les sections.
- Liens : Programme, Le lieu, Dress code, RSVP, Cadeaux, FAQ, Photos, Contact.
- Clic sur un lien → défilement fluide vers la section correspondante (`#id`).
- Clic sur "L & V" (logo) → retour à `#accueil`.

## `#accueil` — Accueil

- Photo du couple, prénoms, date, compte à rebours en direct (jours/heures/minutes/secondes).
- Clic sur **"Ajouter à mon agenda"** → ouvre Google Calendar pré-rempli, dans un nouvel onglet (sortie du site).

## `#programme` — Programme

- Deux cartes : Samedi 1er mai (cérémonie, cocktail, dîner, soirée) et Dimanche 2 mai (brunch).
- Pas d'élément cliquable dans cette section.

## `#lieu` — Le lieu & infos pratiques

- Photo du domaine, infos parking/hébergement/transport, liste des gîtes à proximité.
- Clic sur **"Itinéraire — Église de Valaurie"** → ouvre Google Maps, nouvel onglet (sortie du site).
- Clic sur **"Itinéraire — Domaine de Montjoyer"** → ouvre Google Maps, nouvel onglet (sortie du site).
- Clic sur un numéro de téléphone de gîte → ouvre l'application téléphone (`tel:`).
- Clic sur un email de gîte (La Valdaine, Gîte La Source) → ouvre l'application mail (`mailto:`).

## `#dresscode` — Dress code

- Texte + 4 pastilles de couleur représentant la palette du mariage.
- Pas d'élément cliquable.

## `#rsvp` — RSVP

- Clic sur **"Répondre au RSVP"** → ouvre le Google Form externe, nouvel onglet (sortie du site).

## `#cagnotte` — Cadeaux

- Texte uniquement (pas de liste de mariage, cagnotte sur place).
- Pas d'élément cliquable.

## `#faq` — Questions fréquentes

- 6 questions/réponses affichées en liste (pas d'accordéon, tout est visible).
- Pas d'élément cliquable.

## `#photos` — Galerie photo

- État par défaut : formulaire "Code d'accès" (champ texte + bouton "Voir les photos").
- Soumission du formulaire :
  - **Code incorrect** → affiche "Code incorrect, merci de réessayer." sous le champ, le formulaire reste affiché.
  - **Code correct, album renseigné** → masque le formulaire, affiche "Merci !" et un bouton **"Voir l'album photos"** → ouvre l'album externe, nouvel onglet (sortie du site). *(État non encore actif — album en attente, cf. PRD.)*
  - **Code correct, album non renseigné** → masque le formulaire, affiche "Merci ! L'album sera mis en ligne juste après le mariage." *(État actuel du site.)*

## `#contact` — Une question ?

- Clic sur "Laly — 06 26 21 20 26" ou "Vincent — 07 60 64 50 73" → ouvre l'application téléphone (`tel:`).
- Clic sur "Mentions légales" → défilement vers `#mentions-legales`.
- Clic sur "Politique de confidentialité" → défilement vers `#confidentialite`.

## `#mentions-legales` et `#confidentialite`

- Texte uniquement.
- Clic sur "↑ Retour en haut" → défilement vers `#accueil`.
