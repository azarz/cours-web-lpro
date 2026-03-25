## Projet

Le cours s'organise autour d'un projet de site web, sur lequel vous serez évalués.

Le site web sera constitué de 2 pages :

- Une page utilisant HTML et CSS, qui contiendra votre CV (facilement convertible en PDF, utile pour vos demandes de stage)
    + Une entête avec votre nom et ville de résidence
    + Un corps avec vos expériences professionnelles et formations
    + Une section listant vos compétences
    + Un bouton qui fait appel à du Javascript (et à la fonction `print()`) pour lancer l'impression du CV (qui ne doit pas apparaître sur le PDF !)

- Une page contenant une carte affichant les POI "Remonter le temps" de l'application Cartes IGN sur le fond WMTS "Plan IGN".
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
    + La popup doit contenir un lien vers le site [https://remonterletemps.ign.fr/comparer/](https://remonterletemps.ign.fr/comparer/) ouvrant directement la bonne vue à l'aide des propriétés du POI
        * Exemple : `https://remonterletemps.ign.fr/comparer/?lon=1.703952&lat=47.996355&z=14&layer1=ORTHOIMAGERY.ORTHOPHOTOS.1950-1965&layer2=ORTHOIMAGERY.ORTHOPHOTOS&mode=vSlider`
    + Données des POI disponibles [ici](poi_rlt.json) au format [GeoJSON](https://web.iamvdo.me/webmapping/notions/#formats-vecteurs), à charger via `fetch()` [(API Fetch)](https://web.iamvdo.me/js/fetch/).
    + Icone des POI : [ici](comparePoi.png)

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

