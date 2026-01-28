## Projet

Le cours s'organise autour d'un projet de site web, sur lequel vous serez évalués.

Le site web sera constitué de 2 pages :

- Une page utilisant HTML et CSS, qui contiendra votre CV (facilement convertible en PDF, utile pour vos demandes de stage)
   + Une entête avec votre nom et ville de résidence
   + Un corps avec vos expériences professionnelles et formations
   + Une section listant vos compétences

- Une page contenant une carte affichant les POI "Remonter le temps" de l'application Cartes IGN sur le fond WMTS "Plan IGN".
  + Les POI sont cliquables, affichant une pop-up avec les infos des propriétés `commune`, `département`, `accroche`, `titre` et `description` mises en forme.
  + La popup contient un lien vers le site [https://remonterletemps.ign.fr/comparer/](https://remonterletemps.ign.fr/comparer/) ouvrant directement la bonne vue (par exemple, https://remonterletemps.ign.fr/comparer/?lon=1.703952&lat=47.996355&z=14&layer1=ORTHOIMAGERY.ORTHOPHOTOS.1950-1965&layer2=ORTHOIMAGERY.ORTHOPHOTOS&mode=vSlider)
  + Données disponibles [ici](poi_rlt.json).

- Les 2 pages seront reliées entre elles via un menu commun (latéral ou en en-tête) comprenant tous les liens du site.

### Barème :

- CV /10
  + informations présentes /2
  + structure HTML cohérente /2
  + cohérence des sélecteurs CSS /2
  + positionnement CSS grid ou flex /2
  + bouton pour impression format A4 /2

- Carto web /10
  + affichage de la carte /2
  + utilisation du flux WMTS Géoplateforme /2
  + affichage des POI sur la carte (utilisation de l'API fetch) /2
  + remplissage des pop-ups des POI /2
  + lien dans les pop-ups vers le site remonter le temps sur la vue correcte /2

- Menu navigation : Si pas présent, **-2 points**

