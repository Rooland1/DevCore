# DevCore - Weboldal készítő oldal

Modern, reszponzív weboldal, ahol a felhasználók csomagokat választhatnak, kitölthetnek egy részletes igényfelmérő kérdőívet, és a megrendelés e-mailben érkezik meg.

## 🚀 Élesítés (GitHub Pages / Netlify / bármilyen statikus hosting)

1. **EmailJS regisztráció** (ingyenes - 200 email/hó)
   - Menj a https://www.emailjs.com/ oldalra
   - Regisztrálj (Google vagy GitHub fiókkal gyors)
   - Hozz létre egy **Service** (pl. Gmail)
   - Hozz létre egy **Email Template**-et (lásd lent)
   - Másold ki a **Public Key**, **Service ID** és **Template ID** értékeket

2. **Email Template beállítása**
   - A sablonban használd ezeket a változókat (`{{variable}}` formában):
     - `{{to_email}}` - a te e-mail címed
     - `{{from_name}}` - ügyfél neve
     - `{{from_email}}` - ügyfél email címe
     - `{{phone}}` - telefonszám
     - `{{website_type}}` - weboldal típusa
     - `{{pages}}` - oldalszám
     - `{{style}}` - design stílus
     - `{{colors}}` - színvilág
     - `{{features}}` - kért funkciók
     - `{{notes}}` - egyéb megjegyzések
     - `{{payment}}` - fizetési mód
     - `{{cart_summary}}` - kosár tartalma
     - `{{total_price}}` - végösszeg

3. **Kód módosítása**
   - Nyisd meg az `index.html` fájlt
   - Keresd meg ezt a részt (a script tetején):
     ```js
     const EMAILJS_PUBLIC_KEY = 'YOUR_PUBLIC_KEY';
     const EMAILJS_SERVICE_ID = 'YOUR_SERVICE_ID';
     const EMAILJS_TEMPLATE_ID = 'YOUR_TEMPLATE_ID';
     ```
   - Cseréld ki az értékeket a sajátjaidra

4. **Feltöltés GitHub-ra**
   ```bash
   git init
   git add .
   git commit -m "DevCore weboldal"
   git remote add origin https://github.com/felhasznalonev/devcore.git
   git push -u origin main
   ```

5. **GitHub Pages beállítás**
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
| `logo2.jpg` | Logó és favicon |
| `README.md` | Ez a fájl |

## ✨ Funkciók

- **3 árazási csomag** (Alap 29.999 Ft, Profi 69.999 Ft, Prémium 119.999 Ft)
- **Kosár rendszer** - több csomag is hozzáadható
- **Részletes kérdőív** - igényfelmérés a pontos specifikációhoz
- **EmailJS** - a megrendelés automatikusan e-mailben érkezik
- **Animated background** - lebegő gradient orbs + grid
- **Reszponzív** - mobil, tablet, desktop
- **Scroll animációk** - Intersection Observer
- **Clean, minimalista design** - dark theme

## ⚠️ Fontos

Az EmailJS ingyenes verziója havonta **200 email** küldését teszi lehetővé, ami bőven elég egy induló vállalkozásnak. Ha többre van szükség, frissítheted a csomagot.

