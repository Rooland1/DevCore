# DevCore - TODO

## ✅ Completed

### Frontend
- [x] Kosár rendszer (navbar ikon + számláló, kosár panel)
- [x] Fizetési módok: Banki átutalás, 2 részletben (i info), Kártya (Stripe)
- [x] Kérdőív modal (név, email, telefon, weboldal típusa, oldalszám, design stílus, színvilág, funkciók, egyéb igények)
- [x] Stripe kártyaelem integráció (teszt mód, `4242 4242 4242 4242`)
- [x] EmailJS - megrendelés küldése e-mailben
- [x] Reszponzív design (mobil, tablet, desktop)
- [x] Animált háttér, scroll animációk
- [x] Toast értesítések

### Dokumentáció
- [x] README.md - teljes telepítési útmutató EmailJS + Stripe beállítással

## 🔧 Beállítás szükséges

Az alábbi szolgáltatásokat regisztrálni kell az élesítés előtt:

1. **EmailJS** (https://www.emailjs.com/) - ingyenes, 200 email/hó
   - Public Key, Service ID, Template ID beállítása

2. **Stripe** (https://stripe.com/) - teszt módban ingyenes
   - Stripe Publishable Key beállítása (jelenleg Stripe teszt key van beállítva)
   - Éles fizetéshez backend szükséges (lásd: server.js)

