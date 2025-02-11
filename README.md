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

Le cours s'organise et et noté via un projet, qui consistera a créer un site web.

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

- Une page contenant une carte affichant les POI "Remonter le temps" de l'application Cartes IGN sur le fond "Plan IGN". (en bonus, les POI sont cliquable avec un raccourci vers le site remonter le temps). Données disponibles dans le dossier data [data/poi_rlt.json](data/poi_rlt.json)

- Les 3 pages seront reliées entre elles via un menu commun (latéral ou en en-tête) comprenant tous les liens du site.