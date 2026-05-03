# theJourney — Reisefotos & Trips

Meine persönliche Reise-Homepage mit interaktiver Weltkarte und chronologischer Timeline.

👉 **https://efcracken.github.io/theJourney**

---

## Wie füge ich eine neue Reise hinzu?

1. Ordner für die Reise anlegen: `bilder/reisename-jahr/` (z.B. `bilder/griechenland-2025/`)
2. Fotos in diesen Ordner hochladen (Cover-Bild als `cover.jpg` benennen)
3. In `index.html` im `TRIPS`-Array einen neuen Eintrag hinzufügen:

```js
{
  id: "griechenland-2025",          // eindeutig, keine Leerzeichen
  title: "Griechenland",
  subtitle: "Athen · Santorini",
  country: "Griechenland",          // für die Länder-Statistik
  date: "Juni 2025",
  year: 2025,
  coords: [39.0742, 21.8243],       // Breitengrad, Längengrad
  cover: "bilder/griechenland-2025/cover.jpg",
  photos: [
    { src: "bilder/griechenland-2025/01.jpg", title: "Akropolis",   date: "Jun 2025" },
    { src: "bilder/griechenland-2025/02.jpg", title: "Caldera",     date: "Jun 2025" },
    // weitere Fotos...
  ]
}
```

Die Reisen werden automatisch nach Jahr sortiert (neueste zuerst).

---

## Ordnerstruktur

```
theJourney/
├── index.html               ← Hauptseite (hier alles konfigurieren)
├── bilder/
│   ├── japan-2024/
│   │   ├── cover.jpg        ← Titelbild der Reise
│   │   ├── 01.jpg
│   │   └── ...
│   ├── island-2023/
│   │   └── ...
│   └── ...
└── README.md
```

---

## Features

- **Weltkarte** mit klickbaren Pins pro Destination (Leaflet.js)
- **Chronologische Timeline** nach Jahren gruppiert
- **Album-Ansicht** pro Reise mit Masonry-Galerie
- **Lightbox** mit Tastatur-Navigation (← → Esc)
- **Statistiken**: Reisen, Länder, Fotos, Jahre
- Responsives Design für Mobile & Desktop
