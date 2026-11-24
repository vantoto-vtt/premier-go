# Météo RDC 🌤️

Application météo progressive en français pour connaître les conditions actuelles et la météo prévue à l'heure d'arrivée dans une destination (ville, commune, quartier ou adresse).

## Fonctionnalités
- Conditions actuelles (température, ressenti, vent, humidité et pluie).
- Prévisions des 7 prochains jours.
- Recherche des lieux avec Open-Meteo et repli sur OpenStreetMap/Nominatim.
- Prévision horaire à la destination pour un déplacement dans les 7 jours.
- Géolocalisation avec autorisation explicite de l'utilisateur.
- Design responsive et installation comme PWA.
- Sans clé API et sans collecte de données sur un serveur applicatif.

## Lancement
Ouvrir `index.html` via un serveur local HTTP (la géolocalisation et le service worker nécessitent HTTPS ou localhost) :

```bash
python -m http.server 8080
```

Puis visiter http://localhost:8080

## Publier avec GitHub Pages
Dans **Settings → Pages**, sélectionner **Deploy from a branch**, puis `main` et `/ (root)`. La publication peut prendre quelques minutes.

## Sources et limites
- Prévisions : [Open-Meteo](https://open-meteo.com/) — les valeurs sont des modèles et estimations, pas des capteurs en direct dans chaque rue.
- Recherche de lieux : Open-Meteo Geocoding et [Nominatim / OpenStreetMap](https://nominatim.org/).
- Les quartiers peuvent avoir des résultats approximatifs. Les prévisions horaires sont limitées aux 7 prochains jours. Open-Meteo peut arrondir les heures à la grille de disponibilité.
- La recherche et la météo nécessitent une connexion Internet, même si l'interface peut rester en cache.
- Respecter les conditions d'attribution et les limites d'usage des services externes avant une montée en charge ou une monétisation.

Licence : prototype d'application.
