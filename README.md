# newastuce-data

Données publiques consommées par l'appli NewAstuce (réseau Astuce, Métropole Rouen Normandie).

- **Release `data-latest`** : `astuce.db.gz` (base SQLite des horaires, générée chaque nuit depuis le GTFS ouvert publié sur transport.data.gouv.fr) et `manifest.json`.
- **GitHub Pages** : `config.json` (configuration distante de l'appli) et `privacy.html` (politique de confidentialité).

Ce dépôt est alimenté automatiquement ; ne pas modifier à la main.

Données source : Métropole Rouen Normandie, via transport.data.gouv.fr, sous Licence Ouverte v2.0 (Etalab).

Note : `cityway.apiKey` dans `config.json` n'est pas un secret. C'est la clé client publique que Cityway publie lui-même pour les widgets de myastuce.fr (`staticwc.mrn.cityway.fr/3.1/assets/MRN_appsettings.json`) et que chaque navigateur reçoit. Elle figure ici pour pouvoir être changée, ou la source coupée (`enabled: false`), sans republier l'appli.
