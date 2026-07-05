# Genesis — Landingpage

Kleine statische Vorstellungsseite für den Genesis-Bot. Kein Server, keine
Datenbank nötig — reines HTML/CSS.

## Setup

### 1. GitHub-Repo
Diesen Ordner in ein neues GitHub-Repo hochladen (z.B. `genesis-website`).

### 2. Bei Netlify importieren
- app.netlify.com -> "Add new site" -> "Import an existing project"
- GitHub verbinden, das Repo auswählen
- Build-Einstellungen übernimmt Netlify automatisch aus `netlify.toml`
- "Deploy site" klicken

### 3. Einladungslink eintragen

In `public/index.html` nach `INVITE_LINK_HIER_EINTRAGEN` suchen und durch
deinen echten Discord-Einladungslink ersetzen. Den bekommst du so:

1. discord.com/developers/applications -> deine Genesis-Anwendung öffnen
2. Links auf "OAuth2" -> "URL Generator"
3. Scopes: `bot`, `applications.commands`
4. Bot Permissions: mindestens "Manage Roles" + "Manage Channels" (oder
   einfach "Administrator")
5. Den generierten Link unten kopieren
6. In `index.html` einfügen, committen — Netlify deployt automatisch neu

## Anpassungen

- Texte/Farben: `public/index.html` und `public/style.css`
- Icon: `public/assets/genesis-icon.png` (durch ein neues Bild ersetzen, gleicher Dateiname reicht)
- Die Seite nutzt die gleiche Farbpalette wie das Bewerbungs-Dashboard
  (Cyan `#2dd4ee`, Violett `#9b6bff`, dunkler Hintergrund) für einen
  einheitlichen Look über alle Phil7442-Projekte hinweg
