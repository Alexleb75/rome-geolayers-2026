# rome-geolayers-2026

Couches GeoJSON de Rome pour **GEOlayers 3** (After Effects).

**Utilisation** : dans GeoLayers → Feature Search → source **GitHub Repo** → URL nue de ce repo, branche `main`.
La recherche se fait **par nom de fichier** ; le chemin du dossier s'affiche comme contexte.

## Structure (1 fichier = 1 entité)
```
Fleuves/    Tibre (Fleuve)            tracé complet source → embouchure (~410 km)
            Aniene (Fleuve)           tracé complet source → confluence avec le Tibre (~120 km)
Quartiers/  Centre historique (Quartier)   contour des 20 rioni intra-muros (≈ murs d'Aurélien, 13,7 km²)
            Esquilino (Quartier)           contour du rione XV
Pays/       Vatican (État)
Monuments/  Colisée (Monument)
            Palazzo della Sapienza (Monument)
Lieux/      Roma Termini (Gare)            emprise des bâtiments de la gare
            Mercato Esquilino (Marché)     Nuovo Mercato Esquilino
Collines/   Aventin (Colline)              point du sommet
```

## Agrégat (racine)
`rome-tout.geojson` : toutes les entités dans un seul fichier.

## Propriétés
`name` (FR), `name_it`, `categorie`, `lat`/`lon` (point représentatif), `source`.

## Sources
OpenStreetMap (© contributeurs OpenStreetMap, licence ODbL). Régénération : `build_rome.py` dans le dossier parent.
