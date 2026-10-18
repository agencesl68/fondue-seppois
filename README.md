# Accueil Fondue — Amicale des Sapeurs-Pompiers de Seppois-le-Bas

App d'accueil pour le repas dansant « Fondue Suisse » du 24 octobre 2026 (salle polyvalente de Seppois-le-Bas).
À l'entrée, on tape le nom de la personne : l'app affiche sa table et anime le chemin depuis l'entrée sur le plan de la salle.

**En ligne :** https://agencesl68.github.io/fondue-seppois/

## Utilisation
1. Ouvrir https://agencesl68.github.io/fondue-seppois/ sur l'ordinateur de l'accueil (Chrome ou Safari).
2. Taper le **code d'accès de l'équipe** (demandé une seule fois par ordinateur) : les réservations se chargent.
3. Pour retrouver le plan de salle et les placements préparés sur un autre ordinateur :
   sur celui-ci, *Réglages → Soirée & sauvegarde → Créer et copier le lien*, puis ouvrir ce lien sur l'ordinateur de l'accueil.

Le lien du Google Sheet est **chiffré** dans ce code public (AES-GCM, clé dérivée du code d'accès) :
sans le code, les réservations restent illisibles. L'app se met à jour toute seule quand une nouvelle version est publiée.

## Placeurs (téléphones)
Sur le téléphone de chaque placeur : ouvrir https://agencesl68.github.io/fondue-seppois/?placeur, taper le code d'accès puis son prénom.
Quand l'accueil pointe une arrivée, le placeur reçoit le nom, le nombre de personnes, la table et le chemin animé sur le plan
(vibration + son si activé). « Je m'en occupe » puis « Placés » : l'accueil voit en direct qui accompagne qui.
Les messages passent par le relais gratuit ntfy.sh, compressés et **chiffrés** (AES-GCM) : le relais ne peut pas les lire.

## Ce que fait l'app
- Lit le Google Sheet **en lecture seule** (export CSV) — elle n'écrit jamais dedans.
- Recherche par nom, table en grand, chemin animé jusqu'à la table, pointage des arrivées (même partielles).
- Plan de salle modifiable (déplacer, pivoter, redimensionner, copier-coller les tables).
- Fondues / jambons par table, enfants de moins de 6 ans, chaises en plus lues dans les remarques.
- Récap imprimable pour la cuisine.

Les données (plan, placements, arrivées) sont stockées dans le navigateur de l'ordinateur, pas sur GitHub.
