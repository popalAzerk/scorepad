# Score Pad — reconstruction web

Compteur de points pour jeux de société et de cartes, reconstruit à partir du comportement
décrit publiquement par l'app « Score Pad – compteur de points » (Nicolas Lehovetzki) :
nom de partie, joueurs personnalisés, mode standard ou somme nulle, victoire au score le plus
haut ou le plus bas, grille tour par tour, totaux automatiques, historique, export.

## Ce que fait l'application

- **Parties multiples** conservées côte à côte, avec reprise en un geste.
- **Joueurs** nommés, chacun avec un emoji et une couleur, réutilisés d'une partie à l'autre.
- **Deux modes de calcul** : *standard* (chacun marque librement) et *somme nulle* (chaque tour
  doit totaliser zéro — Tarot, contrats — avec avertissement avant enregistrement).
- **Victoire au plus haut ou au plus bas** — le total gagnant est mis en évidence.
- **Grille** : un tour par ligne, un joueur par colonne, appui sur une case pour saisir ou corriger.
- **Pavé numérique** intégré, montants négatifs, décimales ; le premier chiffre tapé remplace
  l'ancienne valeur au lieu de s'y accoler.
- **Annulation** du dernier tour, suppression d'une partie.
- **Export** : partage natif du résumé, sinon copie dans le presse-papiers.
- **Hors ligne**, sans compte, sans publicité : tout reste dans le `localStorage` de l'appareil.

## Fichiers

- `index.html` — l'application entière (HTML, CSS, JavaScript, aucune dépendance).
- `manifest.webmanifest` — installation sur l'écran d'accueil (PWA), mode autonome.

## Installation sur téléphone

Ouvrir l'adresse, puis « Ajouter à l'écran d'accueil ». L'application fonctionne ensuite sans réseau.

## Différences assumées avec l'original

- Pas de photos de joueurs : emoji et couleur, plus légers et suffisants.
- Pas de compte ni de synchronisation entre appareils : les données ne quittent pas l'appareil.
