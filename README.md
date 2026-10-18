# Accueil Fondue — Amicale des Sapeurs-Pompiers de Seppois-le-Bas

App d'accueil pour le repas dansant « Fondue Suisse » du 24 octobre 2026 (salle polyvalente de Seppois-le-Bas).
À l'entrée, on tape le nom de la personne : l'app affiche sa table et anime le chemin depuis l'entrée sur le plan de la salle.

**En ligne :** https://agencesl68.github.io/fondue-seppois/

## Utilisation
1. Ouvrir le lien sur l'ordinateur de l'accueil (Chrome conseillé).
2. Réglages → **Source** : coller le lien du Google Sheet des réservations (partagé en « Lecteur »).
   Le lien n'est pas dans ce code public : il reste enregistré sur l'ordinateur uniquement.
3. Réglages → **Soirée & sauvegarde** → *Importer* le fichier `.json` exporté depuis l'ordinateur où le plan a été préparé.

## Ce que fait l'app
- Lit le Google Sheet **en lecture seule** (export CSV) — elle n'écrit jamais dedans.
- Recherche par nom, table en grand, chemin animé jusqu'à la table, pointage des arrivées (même partielles).
- Plan de salle modifiable (déplacer, pivoter, redimensionner, copier-coller les tables).
- Fondues / jambons par table, enfants de moins de 6 ans, chaises en plus lues dans les remarques.
- Récap imprimable pour la cuisine.

Les données (plan, placements, arrivées) sont stockées dans le navigateur de l'ordinateur, pas sur GitHub.
