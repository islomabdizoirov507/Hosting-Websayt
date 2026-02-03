# HostUz — HTML/CSS Hosting Website (Demo)

Internet hosting kompaniyasi uchun **marketing websayt** (demo). Loyiha **faqat HTML5 + CSS3** asosida qurilgan (Bootstrap/JavaScript ishlatilmagan).

## Asosiy imkoniyatlar

- **Desktop-first** layout: container + grid tizimi
- **Responsive**: desktop / tablet / smartphone
- **Typography**: `Lato` (fallback fontlar bilan)
- **UI komponentlar**: CTA buttonlar, cardlar, pricing bloklar, formalar
- **CSS animatsiya**: `moveRightAndFade` (scroll ko‘rinishida, JSsiz)
- **Iconlar**: Font Awesome (CDN orqali)
- **GitHub Pages**: repo’dan deploy qilish mumkin

---

## Sahifalar (minimal to‘plam)

- `index.html` — Home / Landing (Hero + CTA + Xizmatlar + Narxlar preview)
- `pricing.html` — Plans / Pricing (paketlar, taqqoslash, “Order” CTA)
- `order.html` — Buyurtma (demo forma)
- `contact.html` — Aloqa / Support (demo forma + kontaktlar)
- `about.html` — Kompaniya haqida (missiya, infratuzilma, rekvizitlar)

> Agar repo’da eski demo sahifalar (`hosting.html`, `vps.html`, `domains.html`, `login.html`) qolgan bo‘lsa va endi ishlatilmasa — ularni o‘chirib tashlashingiz yoki keyingi versiya uchun alohida branch’da saqlashingiz mumkin.

---

## Stil fayllari (CSS arxitekturasi)

- `common_styles.css` — **GLOBAL** (hamma sahifalar uchun):
  - container / grid
  - navbar + footer
  - typography (Lato + rem/clamp)
  - button/link stillari
  - umumiy card va form stillari
  - `@keyframes moveRightAndFade`

- `home_style.css` — **faqat `index.html`** (Hero video, Home sectionlar)

- `pages_style.css` — **pricing/order/contact/about** sahifalariga xos stillar

---

## Papkalar (tavsiya)

```
assets/
  brand/      # logo/brand SVG/PNG
  bg/         # hero.mp4 va section backgroundlar
css/
  (ixtiyoriy) # agar CSS’larni papkaga ajratsangiz
```

> Muhim: GitHub Pages (Project Pages) uchun video yo‘li odatda **relativ** bo‘lishi kerak:  
> `assets/bg/hero.mp4` (boshlanishida `/` bo‘lmasin).

---

## Lokal ishga tushirish

1) Fayllarni yuklab oling yoki repo’ni clone qiling  
2) Brauzerda `index.html` ni oching

---

## GitHub Pages’da chiqarish (Deploy)

1) GitHub repo → **Settings** → **Pages**  
2) **Source**: “Deploy from a branch”  
3) **Branch**: `main` va papka: `/ (root)`  
4) Saqlang (Save)  
5) Bir necha daqiqadan keyin Pages link paydo bo‘ladi

---

## Ish jarayoni (GitHub)

- HTML/CSS’da o‘zgartirish qiling
- `Commit` → `Push`
- GitHub Pages avtomatik yangilanadi

---

## Foydalanilgan resurslar

- **Font Awesome** — ikonlar uchun (CDN)
- **Google Fonts — Lato** — tipografiya
