# Backend & données — Site du mariage de Laly & Vincent

Le site n'a pas de backend ni de base de données (cf. TRD). Les données personnelles listées ci-dessous vivent soit dans le code source du site, soit dans des services externes liés (Google Forms, Google Photos), soit sont générées passivement par l'hébergeur.

## Risque identifié

Le site est hébergé sur GitHub Pages, **public par défaut et maintenant indexé par Google**. Il est donc consultable par n'importe qui sur Internet, pas seulement par les invités ayant reçu le lien. Toute donnée affichée sur le site (notamment les numéros de téléphone) est donc publique de fait. Ce compromis a été accepté sciemment pour permettre le référencement du site.

## Inventaire des données personnelles

| Donnée | Où elle est stockée | Qui peut la lire | Qui peut l'écrire / la modifier | Durée de conservation |
|---|---|---|---|---|
| Téléphones de Laly et Vincent | Code source du site, servi par GitHub Pages (infrastructure GitHub / Fastly). Région : **[À CONFIRMER]** | Public — toute personne visitant le site (indexé par Google) | Vincent uniquement (seul accès en écriture au dépôt GitHub) | Indéfinie, tant que le site reste en ligne. **[À CONFIRMER]** si retrait prévu après le mariage |
| Réponses RSVP (nom, présence, allergies/régime, chanson) | Google Forms / feuille de réponses associée (infrastructure Google). Région : **[À CONFIRMER]** | Laly et Vincent (propriétaires du formulaire) ; Google selon sa propre politique | Toute personne ayant le lien du formulaire (accès restreint au lien, non public) | Supprimées après le mariage (engagement pris par Laly et Vincent) |
| Photos des invités (une fois l'album en ligne) | Google Photos (infrastructure Google). Région : **[À CONFIRMER]** | Toute personne ayant le lien de l'album, révélé après saisie du code sur le site (accès restreint au lien) | Laly et Vincent. **[À CONFIRMER]** si la photographe a un accès direct à l'album ou transmet les photos séparément | Supprimées après le mariage (engagement pris par Laly et Vincent) |
| Logs d'accès au site (adresses IP, user-agent des visiteurs) | Infrastructure GitHub Pages / Fastly, hors du contrôle de Laly et Vincent. Région : **[À CONFIRMER]** | GitHub et ses sous-traitants, selon leur propre politique de confidentialité — ni Laly ni Vincent n'y ont accès via ce projet | Généré automatiquement à chaque visite, aucune action des propriétaires du site | **[À CONFIRMER]** — régie par la politique de GitHub, non documentée dans ce projet |

## Secret technique (hors données personnelles)

| Élément | Où il est stocké | Qui peut le lire | Qui peut l'écrire | Durée |
|---|---|---|---|---|
| Code d'accès à la galerie photo (actuellement `PRIEURE1MAI`) | En clair dans le JavaScript du site, visible par quiconque consulte le code source de la page | Toute personne qui inspecte le code source, pas seulement les invités | Vincent uniquement | Jusqu'au prochain changement dans le code |
