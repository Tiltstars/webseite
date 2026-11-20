# david-grasbeinter.de

Website von David Grasbeinter (KI-Training). Reines HTML und CSS, ohne Skripte und ohne Build-Schritt.

## Aufbau

Alles, was online geht, liegt im Ordner `public/`:

| Seite | Deutsch | Englisch |
|---|---|---|
| Startseite | `public/index.html` | `public/en/index.html` |
| Impressum | `public/impressum/index.html` | `public/en/legal-notice/index.html` |
| Datenschutz | `public/datenschutz/index.html` | `public/en/privacy/index.html` |

Gemeinsames Aussehen: `public/assets/style.css`. Symbol im Browser-Tab: `public/favicon.svg`.

## Hosting

Render, Typ **Static Site**, verbunden mit diesem Repository:

- Build Command: leer lassen
- Publish Directory: `public`

Jede Änderung auf dem Branch `main` geht automatisch online.

## Später nachtragen

- **Foto:** Bild als `public/assets/david.jpg` ablegen (quadratisch, mindestens 600 × 600 Pixel) und in beiden Startseiten den `DG`-Platzhalter durch die `<img>`-Zeile aus dem Kommentar darüber ersetzen.
- **Umsatzsteuer-ID / Wirtschafts-ID:** In beiden Impressum-Seiten den auskommentierten Block freischalten und die Nummer eintragen.

## Lokal ansehen

```bash
python -m http.server 8080 --directory public
```

Dann http://localhost:8080 im Browser öffnen.
