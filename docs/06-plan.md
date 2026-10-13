# Plan de construction — Site du mariage de Laly & Vincent

Chaque étape tient dans une session et se termine par quelque chose de vérifiable dans le navigateur.

## Fait

1. **Créer la page de base** (hero, prénoms, date, lieu) → vérifiable : la section Accueil s'affiche.
2. **Ajouter le compte à rebours en direct** → vérifiable : les chiffres défilent en temps réel sur la page.
3. **Ajouter le programme** (cartes Samedi / Dimanche) → vérifiable : les deux cartes et leurs horaires s'affichent.
4. **Ajouter la section "Le lieu"** avec la vraie photo du domaine et les boutons d'itinéraire → vérifiable : la photo et les deux boutons Google Maps s'affichent.
5. **Ajouter la liste des gîtes à proximité** → vérifiable : les 4 cartes de gîtes (adresse, téléphone, distance) s'affichent.
6. **Ajouter le dress code** (texte + 4 pastilles de couleur) → vérifiable : les 4 pastilles s'affichent dans la bonne couleur.
7. **Ajouter le bouton RSVP** vers le Google Form → vérifiable : le clic ouvre le formulaire dans un nouvel onglet.
8. **Ajouter la section Cadeaux** → vérifiable : le texte s'affiche.
9. **Ajouter la FAQ** (6 questions) → vérifiable : les 6 questions/réponses s'affichent.
10. **Construire la galerie photo protégée par code** (formulaire, vérification côté client, message de déverrouillage) → vérifiable : saisir le bon code affiche le message "Merci !".
11. **Ajouter la section Contact** (téléphones cliquables) → vérifiable : le clic ouvre l'application téléphone sur mobile.
12. **Ajouter mentions légales et politique de confidentialité** → vérifiable : les deux sections s'affichent en bas de page.
13. **Remplacer l'illustration par la vraie photo du couple** en haut de page → vérifiable : la photo s'affiche avant les prénoms.
14. **Ajouter le bouton "Ajouter à mon agenda"** → vérifiable : le clic ouvre Google Calendar pré-rempli.
15. **Publier le code sur GitHub et activer GitHub Pages** → vérifiable : le site est accessible à `vincentmatray-69600.github.io/site-mariage/`.
16. **Optimiser le référencement** (titres, meta description, Open Graph, JSON-LD Event + FAQPage, sitemap.xml, robots.txt, vérification Google Search Console) → vérifiable : le test de données structurées et le rapport Search Console ne signalent plus d'erreur bloquante.
17. **Optimiser la performance** (compression des images, chargement asynchrone des polices) → vérifiable : un test de vitesse (ex. PageSpeed) donne un score Performance ≥ 90.
18. **Corriger les contrastes de couleur** pour l'accessibilité → vérifiable : un test de vitesse donne un score Accessibilité à 100.

## À faire

19. **Créer l'album Google Photos**, y déposer les photos du mariage, régler le partage sur "accès restreint aux personnes ayant le lien" → vérifiable : ouvrir le lien de l'album dans un navigateur et voir les photos.
20. **Renseigner `ALBUM_URL` dans le code du site** avec le lien de l'album → vérifiable : sur le site, saisir le code d'accès affiche le bouton "Voir l'album photos", et le clic ouvre bien l'album.
21. **Supprimer les données après le mariage** : réponses du Google Form RSVP et album Google Photos → vérifiable : le formulaire et l'album ne sont plus accessibles.
