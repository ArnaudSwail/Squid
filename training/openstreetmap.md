# OpenStreetMap

Les objets de base de la base de données OSM sont les noeuds (*node*) et les chemins (*way*).
Les chemins permettent de définir des lignes et des polygones.

## L'API d'OpenStreetMap, Overpass API
Il est possible d'interroger OpenStreetMap via le bais de requêtes HTTP.

OpenStreetMap utilise un langage spécifique pour la création de requêtes.

[OpenSteetMap Overpass API](http://overpass-turbo.eu/)

Requête pour récupérer les zones résidentielles, commerciales et de bureaux
```
(
  way
  [landuse=residential]
  ({{bbox}});

  way
  [landuse=commercial]
  ({{bbox}});

  way
  [landuse=retail]
  ({{bbox}});

);
(._;>;);
out;
```

Quelques exemples de définition de zones
```
(
  way
  	[landuse=meadow]
  	({{bbox}});

  way
  	[landuse=farmland]
  	({{bbox}});

  way
  [landuse=orchard]
  ({{bbox}});

  way
  [landuse=greenhouse_horticulture]
  ({{bbox}});

  way
  [landuse=greenfield]
  ({{bbox}});

  way
  [landuse=grass]
  ({{bbox}});

  way
  [landuse=forest]
  ({{bbox}});

  way
  [landuse=  military]
  ({{bbox}});

  way
  [landuse	= commercial]
  ({{bbox}});

  way
  [landuse	= construction]
  ({{bbox}});

  way
  [landuse	= industrial]
  ({{bbox}});

  way
  [landuse	= residential]
  ({{bbox}});

  way
  [landuse	= retail]
  ({{bbox}});

);
(._;>;);
out;
```
