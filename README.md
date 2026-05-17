# 🎬 Z Môjho Objektívu

**Elegantná link stránka pre QR kód – Peter Obala**

> Motorky · Cesty · Atmosféra · Slovensko v pohybe

---

## 🌐 Live stránka

**[zmojhoobjektivu.github.io](https://zmojhoobjektivu.github.io)**

---

## 📁 Štruktúra projektu

```
z-mojho-objektivu/
├── index.html           ← celá stránka (HTML + CSS + JS v jednom)
├── assets/
│   ├── avatar.png       ← originálne logo (1254×1254px)
│   ├── avatar_400.png   ← optimalizované pre web (400×400px)
│   └── avatar.webp      ← WebP pre rýchle načítanie
└── README.md
```

---

## 🚀 Publikovanie na GitHub Pages

### Krok 1 – Vytvor repozitár

1. Choď na **github.com** → **New repository**
2. Názov: `zmojhoobjektivu` (alebo vlastný)
3. Nastav na **Public**
4. Klikni **Create repository**

### Krok 2 – Nahraj súbory

```bash
git init
git add .
git commit -m "🚀 Z Môjho Objektívu – link page"
git branch -M main
git remote add origin https://github.com/TVOJE_MENO/zmojhoobjektivu.git
git push -u origin main
```

### Krok 3 – Zapni GitHub Pages

1. V repozitári: **Settings → Pages**
2. **Source:** Branch `main`, folder `/ (root)`
3. Klikni **Save**
4. Za 1–2 minúty je stránka live na:
   ```
   https://TVOJE_MENO.github.io/zmojhoobjektivu/
   ```

### Krok 4 – Vlastná doména (voliteľné)

Ak máš doménu (napr. `zmojhoobjektivu.sk`):

```
# DNS záznamy u registrátora:
A     @    185.199.108.153
A     @    185.199.109.153
A     @    185.199.110.153
A     @    185.199.111.153
CNAME www  TVOJE_MENO.github.io
```

V Settings → Pages vlož doménu a zaškrtni **Enforce HTTPS**.

---

## 🔧 Personalizácia

Všetko je v jednom súbore `index.html`:

| Čo zmeniť | Kde hľadať |
|---|---|
| URL stránky pre OG tagy | `<meta property="og:url">` v `<head>` |
| Sociálne URL | `href` atribúty na `.link-btn` elementoch |
| Popis / text | sekcia `<section class="hero">` |
| Farby | `:root` CSS premenné na začiatku `<style>` |
| Logo / avatar | súbory v `assets/` |
| QR URL text | `<p class="qr-url">` |

---

## ✅ Funkcie

- ✅ Mobilná link stránka optimalizovaná pre QR kód
- ✅ Tvoje logo ako profilovka (WebP + PNG fallback)
- ✅ YouTube, Facebook, Instagram – veľké tlačidlá s hover efektom
- ✅ QR kód automaticky generovaný podľa URL (API + offline fallback)
- ✅ Tlačidlo Zdieľať (Web Share API na mobile)
- ✅ Dark cinematic štýl – červená, oranžová, čierna
- ✅ Jemné animácie pri načítaní
- ✅ SEO + Open Graph meta tagy
- ✅ Favicon (SVG objektív)
- ✅ Celé v jednom index.html – žiadny backend

---

*Created with ❤️ by Peter Obala*  
*© 2025 Z Môjho Objektívu*
