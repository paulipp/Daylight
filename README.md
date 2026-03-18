# Helsinki Aurinko ☀️

Auringonnousu- ja laskuaikojen seuranta Helsingissä. Toimii PWA:na — asennettavissa suoraan puhelimeen.

## Ominaisuudet

- Tänään: nousu, lasku, päivän pituus, muutos eiliseen
- 14 päivän ennuste taulukossa
- 3 kuukauden graafi
- Toimii offline (service worker)
- Asennettavissa Android & iOS -laitteille

## Tiedostorakenne

```
/
├── index.html          # Sovellus
├── manifest.json       # PWA-manifesti
├── sw.js               # Service worker
├── favicon.ico
└── icons/
    ├── icon-72x72.png
    ├── icon-96x96.png
    ├── icon-128x128.png
    ├── icon-144x144.png
    ├── icon-152x152.png
    ├── icon-192x192.png
    ├── icon-384x384.png
    ├── icon-512x512.png
    ├── apple-touch-icon.png
    ├── favicon-32x32.png
    └── favicon-16x16.png
```

## Julkaisu GitHub Pagesilla

1. Luo uusi repository GitHubissa
2. Pushaa kaikki tiedostot `main`-haaraan
3. Mene **Settings → Pages**
4. Source: `Deploy from a branch` → `main` → `/ (root)`
5. Tallenna — sivu on hetken kuluttua osoitteessa `https://<käyttäjä>.github.io/<repo>/`

## Asennus puhelimelle

**Android (Chrome):**
Avaa sivu selaimessa → kolme pistettä → *Lisää aloitusnäyttöön*

**iOS (Safari):**
Avaa sivu Safarissa → jaa-painike → *Lisää Koti-valikkoon*

## Tekniset tiedot

- Aurinkolaskelmat: Jean Meeus -algoritmi
- Koordinaatit: 60.1699°N, 24.9384°E (Helsinki)
- DST (kesä-/talviaika) lasketaan automaattisesti
- Ei ulkoisia riippuvuuksia (paitsi Google Fonts)
- Ei palvelinpuolen koodia — toimii staattisena sivuna
