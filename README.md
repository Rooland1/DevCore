# DevCore - Weboldal készítő oldal

Modern, reszponzív weboldal, ahol a felhasználók megtekinthetik a csomagokat és üzenetet küldhetnek Formspree-n keresztül.

## 🚀 Élesítés (GitHub Pages / Netlify / bármilyen statikus hosting)

1. **Formspree regisztráció** (ingyenes - 50 email/hó, fizetős verzióban korlátlan)
   - Menj a https://formspree.io/ oldalra
   - Regisztrálj (Google vagy GitHub fiókkal gyors)
   - Hozz létre egy új **Form**-ot
   - Másold ki a Form ID-t (pl. `xjkyjvgg`)
   - Az `index.html` fájlban keresd meg a form action-t:
     ```html
     <form id="messageForm" action="https://formspree.io/f/xjgnagkd" method="POST">
     ```
   - Cseréld ki a `xjgnagkd` részt a saját Form ID-dra (ha másikat szeretnél használni)

2. **Formspree értesítések beállítása**
   - A Formspree dashboardon beállíthatod, hogy melyik email címre érkezzenek az üzenetek
   - Automatikus válasz email-t is beállíthatsz a felhasználóknak

3. **Feltöltés GitHub-ra**
   ```bash
   git init
   git add .
   git commit -m "DevCore weboldal"
   git remote add origin https://github.com/felhasznalonev/devcore.git
   git push -u origin main
   ```

4. **GitHub Pages beállítás**
   - Repó → Settings → Pages
   - Source: Deploy from branch → main → / (root) → Save
   - Pár perc múlva elérhető a `https://felhasznalonev.github.io/devcore/` címen

## 🛠 Lokális fejlesztés

```bash
# 1. Nyisd meg az index.html-t böngészőben
start index.html       # Windows
open index.html        # Mac
```

## 📁 Fájlok

| Fájl | Leírás |
|------|--------|
| `index.html` | Fő weboldal (HTML + CSS + JS minden benne) |
| `style.css` | Stíluslap |
| `logo2.jpg` | Logó és favicon |
| `README.md` | Ez a fájl |

## ✨ Funkciók

- **3 árazási csomag** (Alap 29.999 Ft, Profi 69.999 Ft, Prémium 119.999 Ft)
- **Üzenetküldő űrlap** - csomag választással, automatikus email értesítés Formspree-n keresztül
- **Animated background** - lebegő gradient orbs + grid
- **Reszponzív** - mobil, tablet, desktop (3 csomag egymás mellett kicsinyítve mobilon)
- **Scroll animációk** - Intersection Observer
- **Clean, minimalista design** - dark theme
- **Toast értesítések** - küldés sikerességének visszajelzése

## ⚠️ Fontos

A Formspree ingyenes verziója havonta **50 email** küldését teszi lehetővé. Ha többre van szükség, frissítheted a csomagot.

