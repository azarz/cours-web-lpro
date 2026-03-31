# Projet

Le cours s'organise autour d'un projet de site web, sur lequel vous serez évalués.

Le site web sera constitué de 2 pages.

[Lien du dossier où déposer votre rendu](https://drive.google.com/drive/folders/1I-zFpVJdTS-ww8PN6pN8qjqwZaetOAt8?usp=sharing) : créer un sous-dossier au format VOTRE_NOM_Votre_Prénom.

### Page 1 : CV
Cette page utilisant HTML et CSS contiendra votre CV facilement convertible en PDF, utile pour vos demandes de stage

Cette page devra inculre :

+ Une entête avec votre nom et ville de résidence
+ Un corps avec vos expériences professionnelles et formations
+ Une section listant vos compétences
+ Un bouton qui fait appel à du Javascript (et à la fonction `print()`) pour lancer l'impression du CV (qui ne doit pas apparaître sur le PDF !)

Le positionnement des différents éléments doit être géré via `grid` et / ou `flex`

### Page 2 : Carto web
Cette page contiendra une carte affichant les Points d'intérêt (POI) "Remonter le temps" de l'application Cartes IGN sur le fond WMTS "Plan IGN".

Consignes :

+ Vous pouvez utiliser la librairie cartographique de votre choix ([Leaflet](https://web.iamvdo.me/webmapping/leaflet/), [Maplibre](https://web.iamvdo.me/webmapping/maplibre/) ou [Openlayers](https://web.iamvdo.me/webmapping/ol-carte/))
+ Accès à la documentation pour afficher le Plan IGN : [documentation sur cartes.gouv.fr](https://cartes.gouv.fr/aide/fr/guides-utilisateur/utiliser-les-services-de-la-geoplateforme/diffusion/wmts/)
    * LAYER : `GEOGRAPHICALGRIDSYSTEMS.PLANIGNV2`
    * STYLE : `normal`
    * FORMAT : `image/png`
    * TILEMATRIXSET : `PM`
    * TILEMATRIX : `{z}`
    * TILECOL : `{x}`
    * TILEROW : `{y}`
+ Les POI doivent être cliquables, affichant une pop-up avec les infos des propriétés `commune`, `departement`, `accroche`, `theme` et `texte` mises en forme via CSS.
+ La popup doit contenir un lien vers le site [https://remonterletemps.ign.fr/comparer/](https://remonterletemps.ign.fr/comparer/) ouvrant directement la bonne vue à l'aide des autres propriétés du POI (`layer1`, `layer2`, `zoom`, `mode`) et de ses coordonnées.
  * Exemple : `https://remonterletemps.ign.fr/comparer/?lon=1.703952&lat=47.996355&z=14&layer1=ORTHOIMAGERY.ORTHOPHOTOS.1950-1965&layer2=ORTHOIMAGERY.ORTHOPHOTOS&mode=vSlider`
+ Données des Points d'intérêt disponibles [[https://azarz.github.io/cours-web-lpro/poi_rlt.json](poi_rlt.json) au format [GeoJSON](https://web.iamvdo.me/webmapping/notions/#formats-vecteurs), à charger via `fetch()` [(API Fetch)](https://web.iamvdo.me/js/fetch/).
+ Icône pouvant être utilisée par les POI : [https://azarz.github.io/cours-web-lpro/comparePoi.png](comparePoi.png)

### Sur les 2 pages : Menu de navigation
Les 2 pages seront reliées entre elles via un menu commun (latéral, en-tête ou pied-de-page) comprenant les liens du site, et éventuellement des liens externes et des informations complémentaires.

## Barème :

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




### Page 3 (Bonus) UNIQUEMENT SI LES 2 PAGES PRÉCÉDENTES SONT 100% FONCTIONNELLES

Faire l'exercice sur les métros : [https://web.iamvdo.me/webmapping/exercices/2-metro/](https://web.iamvdo.me/webmapping/exercices/2-metro/)

Ne pas oublier d'ajouter le menu de navigation, et le lien vers cette page dans le menu de navigation des autres pages

Si (et seulement si) les autres pages sont complètes, ce bonus sera pris en compte dans la notation (uniquement pour ajouter des points).

