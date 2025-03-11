# Cours de cartographie Web pour les Licence Pro Parcours 1 & 2 de l'ENSG

## Référence cours magistral
Le cours magistral s'appuie sur le super cours de Vincent De Olivera [@iamvdo](https://github.com/iamvdo), le web de A à Z : [https://web.iamvdo.me/](https://web.iamvdo.me/).

- Principes du web
- HTML
- CSS
- Serveur - PHP
- Javascript
  + Principe
  + Langage
  + Langage avancé
    * DOM
    * API Fetch
- Webmapping


## Projet

Le cours s'organise et est noté via un projet, qui consistera a créer un site web.

Le site web sera constitué de 3 pages :
- Une page utilisant HTML et CSS, qui contiendra votre CV (en bonus, facilement convertible en PDF, utile pour vos demandes de stage)
   + Une entête avec votre nom et ville de résidence 
   + Un corps avec vos expériences professionnelles et formations 
   + Une section listant vos compétences

- Une page contenant un formulaire permettant de générer l'emploi du temps d'un étudiant fictif (données issues du dossier [data](data)), à partir de son nom + prénom et de sa promotion.
   + Un champ "select" pour sélectionner l'élève 
   + Un champ "number" pour le numéro de mois
   + Un champ "number" pour le numéro de jour.
      * Seules les données pour les 15 premiers jours de mars sont disponibles (mois 3, jour de 1 à 15)
(en bonus, codé à l'aide de PHP + SQL)

- Une page contenant une carte affichant les POI "Remonter le temps" de l'application Cartes IGN sur le fond "Plan IGN". Les POI sont cliquables, affichant une pop-up avec toutes les infos de propriété et un lien avec vers le site https://remonterletemps.ign.fr/comparer/ ouvrant directement la bonne vue. Données disponibles dans le dossier data [data/poi_rlt.json](data/poi_rlt.json). En bonus, la popup contient également un bouton qui change la vie directement sur la page à l'aide du plugin https://github.com/digidem/leaflet-side-by-side

- Les 3 pages seront reliées entre elles via un menu commun (latéral ou en en-tête) comprenant tous les liens du site.

Barème :

CV /8
 - informations présentes /2
 - structure HTML cohérente /2
 - cohérence des sélecteurs CSS /2
 - positionnement CSS grid ou flex /2
bonus : impression format A4 (1pt) rendu "pro" (1pt)

Emploi du temps /4
- formulaire correct /1
- à la validation, le bon emploi du temps s'affiche /3
bonus : utilisation du PHP (2pts)

Carto web /8
- affichage de la carte /1
- utilisation de flux géoplateforme /1
- affichage des POI sur la carte (utilisation de fetch) /2
- remplissage des pop-ups des POI /2
- lien dans les pop-ups vers le site remonter le temps sur la vue correcte /2
bonus : bouton dans la popup pour modifier la vue carto à l'aide du plugin leaflet-side-by-side (2pts)

Menu navigation :
Si pas présent, -2 points 

