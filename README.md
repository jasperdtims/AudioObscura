# Audio Obscura Festival 2026 PWA

Deze map bevat de complete webapp:

- `index.html`
- `manifest.webmanifest`
- `sw.js`
- `favicon.ico`
- `icons/`

## Publiceren via GitHub Pages

1. Maak een nieuwe GitHub-repository.
2. Upload **de inhoud van deze map naar de root van de repository**.
3. Open in GitHub: **Settings → Pages**.
4. Kies onder **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/(root)**
5. Sla op en wacht tot GitHub Pages de site heeft gepubliceerd.

GitHub Pages gebruikt HTTPS. Dat is nodig voor de service worker en PWA-functionaliteit.

## Installeren op iPhone

1. Open de GitHub Pages-URL in Safari.
2. Tik op **Delen**.
3. Kies **Zet op beginscherm**.
4. Open de app daarna vanaf het beginscherm.

De app gebruikt het Audio Obscura-icoon en opent in standalone modus, dus zonder de normale Safari-interface.

## Cache bij updates

Als je later wijzigingen publiceert en iOS blijft een oude versie tonen, wijzig dan in `sw.js`:

`audio-obscura-festival-2026-v1`

naar bijvoorbeeld:

`audio-obscura-festival-2026-v2`

Daarmee wordt een nieuwe cache opgebouwd.
