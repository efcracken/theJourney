# theJourney — Mein Portfolio

Mein persönliches Foto- und Video-Portfolio, erreichbar unter:
👉 **https://efcracken.github.io/theJourney**

---

## Wie füge ich neue Fotos hinzu?

1. Bild in den Ordner `bilder/` hochladen (auf GitHub: "Add file" → "Upload files")
2. In `index.html` im `PORTFOLIO`-Array einen neuen Eintrag hinzufügen:

```js
{
  type: "image",
  src: "bilder/mein-foto.jpg",
  title: "Mein Titel",
  category: "natur",   // natur | reisen | portrait | video
  date: "Zürich, 2025"
}
```

## Wie bette ich ein YouTube-Video ein?

```js
{
  type: "youtube",
  src: "VIDEO_ID",     // die ID aus der YouTube-URL: ?v=VIDEO_ID
  title: "Mein Video",
  category: "video",
  date: "2025"
}
```

## Kategorien anpassen

Die Filterkategorien sind in `index.html` in der `<nav>` definiert.
Einfach umbenennen oder neue hinzufügen — `category` in den Einträgen muss jeweils übereinstimmen.

---

## Ordnerstruktur

```
theJourney/
├── index.html       ← Hauptseite (hier alles konfigurieren)
├── bilder/          ← Fotos hier hochladen
└── README.md        ← Diese Datei
```
