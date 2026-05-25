# ⚔ Calorie Quest PWA

En spillaktig kaloriteller med RPG-temaer, animerte bakgrunner og AI-analyse.

## Innhold
```
calorie-quest/
├── index.html        ← Hele appen (én fil)
├── manifest.json     ← PWA-konfigurasjon
├── sw.js             ← Service worker (offline + auto-update)
├── icons/
│   ├── icon-192.png
│   └── icon-512.png
└── .github/
    └── workflows/
        └── deploy.yml ← Auto-deploy til GitHub Pages
```

## Deploy til GitHub Pages

### 1. Opprett repo og push
```bash
git init
git add .
git commit -m "initial commit"
git branch -M main
git remote add origin https://github.com/DITTBRUKERNAVN/REPONAVN.git
git push -u origin main
```

### 2. Aktiver GitHub Pages
Repo → **Settings** → **Pages** → Source: **GitHub Actions**

Appen er live på: `https://DITTBRUKERNAVN.github.io/REPONAVN/`

### 3. Oppdateringer
Push ny kode til `main` → GitHub bygger og deployer automatisk → appen oppdaterer seg selv hos alle brukere.

## Installer som app

**iPhone (Safari):**
Del-knapp → "Legg til på hjemskjerm"

**Android (Chrome):**
Meny (⋮) → "Installer app" eller "Legg til på startskjerm"

## AI-analyse
Legg inn API-nøkkel under ⚙ i appen:
- **Claude:** `sk-ant-...` fra [console.anthropic.com](https://console.anthropic.com)
- **Gemini:** `AIza...` fra [aistudio.google.com](https://aistudio.google.com) (gratis)

Nøkler lagres kun lokalt på enheten.
