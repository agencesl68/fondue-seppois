# Accueil Fondue — Amicale des Sapeurs-Pompiers de Seppois-le-Bas

App d'accueil pour le repas dansant « Fondue Suisse » du 24 octobre 2026 (salle polyvalente de Seppois-le-Bas).
À l'entrée, on tape le nom de la personne : l'app affiche sa table et anime le chemin depuis l'entrée sur le plan de la salle.

**En ligne :** https://agencesl68.github.io/fondue-seppois/

## Utilisation
1. Ouvrir le **lien d'accès de l'équipe** sur l'ordinateur de l'accueil (Chrome conseillé) :
   `https://agencesl68.github.io/fondue-seppois/#sheet=<identifiant du Google Sheet>`
   ou le lien créé par *Réglages → Soirée & sauvegarde → Créer et copier le lien* (plan + placements + sheet).
2. C'est tout : l'app enregistre le lien sur cet ordinateur, retire le lien de la barre d'adresse et charge les réservations.

Ce qui suit le « # » n'est jamais envoyé à GitHub : le lien du sheet (et donc les données des réservations)
n'est ni dans ce code public, ni sur le serveur. Sans lien d'accès, l'app n'affiche aucune réservation.

## Ce que fait l'app
- Lit le Google Sheet **en lecture seule** (export CSV) — elle n'écrit jamais dedans.
- Recherche par nom, table en grand, chemin animé jusqu'à la table, pointage des arrivées (même partielles).
- Plan de salle modifiable (déplacer, pivoter, redimensionner, copier-coller les tables).
- Fondues / jambons par table, enfants de moins de 6 ans, chaises en plus lues dans les remarques.
- Récap imprimable pour la cuisine.

Les données (plan, placements, arrivées) sont stockées dans le navigateur de l'ordinateur, pas sur GitHub.
