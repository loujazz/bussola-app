# Bussola Topografica

App HTML per carta topografica con bussola da orientamento interattiva.

## Logica bussola (IMPORTANTE)
- Corpo ruota → corpo + ghiera si muovono insieme
- Ghiera ruota → solo ghiera si muove, corpo fermo
- Ago sempre fisso (punta a Nord reale)
- Azimut = bodyAngle − bezelAngle
- La ghiera usa rotazione assoluta = bezelAngle + bodyAngle nel DOM SVG

## Struttura attuale
- `index.html` — app monolitica (HTML + CSS + JS in un file)

## TODO
- Separare HTML / CSS / JS in file distinti
- Aggiungere mappa reale (tile OpenStreetMap via Leaflet.js)
- Touch events per mobile
- Persistenza POI in localStorage
- Export mappa + POI come PDF
