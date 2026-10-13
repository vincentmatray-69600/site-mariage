# Design — Site du mariage de Laly & Vincent

## Couleurs

### Palette de marque (couleurs exactes du mariage)

| Couleur | Hex | Usage |
|---|---|---|
| Terracotta | `#C05C3A` | Pastille "dress code" uniquement |
| Lavande | `#A9B2DE` | Pastille "dress code", fond du bouton itinéraire église |
| Ivoire | `#F0E3C4` | Pastille "dress code", fond de la section Accueil |
| Sauge | `#8B9A6C` | Pastille "dress code" uniquement |

### Variantes accessibles (texte et fonds avec texte)

Versions assombries/éclaircies des couleurs de marque, introduites pour respecter un contraste minimum de 4.5:1 (WCAG AA) partout où du texte apparaît.

| Couleur | Hex | Usage |
|---|---|---|
| Terracotta accessible | `#B35636` | Titres, boutons, liens, fond de la section Photos |
| Sauge accessible | `#6A7552` | Légendes, fond de la section Dress code |
| Sauge claire | `#8E9D70` | Texte sur fond très foncé (crédit du pied de page) |

### Neutres

| Couleur | Hex | Usage |
|---|---|---|
| Brun foncé | `#3A2E22` | Texte principal, fond de la section Contact |
| Gris-brun | `#6b6255` | Texte secondaire / descriptions |
| Taupe clair | `#cabf9d` | Texte discret sur fond foncé (footer, mentions légales) |
| Ivoire clair | `#FBF6E8` | Fond de cartes et sections alternées |
| Blanc | `#FFFFFF` | Fond de cartes |
| Lavande très clair | `#EEF0FA` | Fond de la section RSVP |
| Brun très foncé (1) | `#2f251b` | Fond de la section Mentions légales |
| Brun très foncé (2) | `#241c14` | Fond de la section Confidentialité |

## Polices

- **Fraunces** (serif) — titres, tous niveaux (h1, h2, h3), style display.
- **Work Sans** (sans-serif) — texte courant, boutons, étiquettes.
- Chargées depuis Google Fonts, en asynchrone (`preload` + bascule `media`) pour ne pas bloquer l'affichage.

## Logique responsive

- Pas de media queries : les tailles de police et les espacements utilisent `clamp()` pour s'adapter en continu à la largeur d'écran.
- Les grilles de cartes (programme, infos pratiques, gîtes) passent automatiquement à une colonne sur petit écran (`grid-template-columns: repeat(auto-fit, minmax(...))`).
- La barre de navigation défile horizontalement si elle ne tient pas sur une ligne.

## Allure de chaque section

| Section | Fond | Ambiance |
|---|---|---|
| Accueil | Ivoire `#F0E3C4` | Centré, photo du couple en grand, gros titres Fraunces, compte à rebours dans des pastilles blanches |
| Programme | Ivoire clair `#FBF6E8` | Deux cartes blanches côte à côte, titres terracotta |
| Le lieu | Blanc `#FFFFFF` | Photo pleine largeur, cartes infos sur fond ivoire clair, cartes gîtes à bordure sauge fine |
| Dress code | Sauge `#6A7552` | Fond coloré plein, texte et pastilles en ivoire clair |
| RSVP | Lavande très clair `#EEF0FA` | Centré, un seul bouton d'action terracotta |
| Cadeaux | Ivoire clair `#FBF6E8` | Centré, texte seul, section courte |
| FAQ | Blanc `#FFFFFF` | Liste de cartes ivoire clair, une question par carte |
| Photos | Terracotta `#B35636` | Fond coloré plein, formulaire blanc contrastant, texte ivoire clair |
| Contact | Brun foncé `#3A2E22` | Fond sombre, boutons téléphone semi-transparents, texte ivoire |
| Mentions légales | Brun très foncé `#2f251b` | Texte discret taupe clair, section courte |
| Confidentialité | Brun très foncé `#241c14` | Texte discret taupe clair, section courte |
