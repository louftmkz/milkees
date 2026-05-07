# Milkees

Stillzeit, Pumpen und Flasche tracken — offline & lokal gespeichert. Eine kleine PWA, die ohne Account und ohne Server funktioniert.

## Tech

Single-File Vanilla JS PWA. Kein Build-Schritt, kein Framework.

- `index.html` — komplette App (HTML, CSS, JS in einer Datei)
- `manifest.json` — PWA Manifest
- `service-worker.js` — Offline Cache
- `icons/` — App Icons in mehreren Größen
- `vercel.json` — Vercel Cache Headers

## Lokale Entwicklung

Da Service Worker eine Origin brauchen, einfach einen lokalen Server starten:

```bash
python3 -m http.server 8000
# oder
npx serve
```

Dann `http://localhost:8000` öffnen.

## Deploy

Auf Vercel verbunden mit diesem Repo — bei jedem `git push` zu `main` baut Vercel automatisch neu.

## Auf iPhone installieren

1. Safari öffnen, Website aufrufen
2. Teilen → "Zum Home-Bildschirm"
3. Bestätigen

Das Icon erscheint und die App läuft im Standalone-Modus (ohne Browser-Chrome).
