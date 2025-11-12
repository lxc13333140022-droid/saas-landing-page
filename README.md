# 🚀 {{ProductName}} — SaaS Landing Page (Static)

A conversion‑focused single‑file landing page (`index.html`) that follows the “High‑Converting SaaS Landing Page” flow (hero → partners → benefits → how‑it‑works → pricing → testimonials → FAQ → CTA → footer).
Deploy on GitHub Pages, Netlify, Vercel, or any static host.

**Author of `index.html`:** [David Carrero](https://carrero.es)  
**Design inspiration:** https://x.com/him_uiux/status/1971911092206293283

---

## ✨ Features

- HTML5 + Tailwind via CDN (no build step).
- Accessible by default (semantics, ARIA, focus, contrast).
- Outcome‑driven copy blocks (benefits over features).
- Sticky navbar, dual CTAs, partner logos, bento‑style benefits.
- How it works (3 steps), pricing with monthly/annual toggle (vanilla JS).
- Testimonials, FAQ, final CTA, basic SEO meta.
- Easy to localize (base copy in Spanish).

---

## 📁 Structure

```text
.
├─ index.html
├─ assets/
│  ├─ logo.svg
│  ├─ screenshot-hero.png
│  └─ og-cover.png
└─ README.md
```

> The HTML contains `{{…}}` placeholders. Search & replace with your product name, URLs, and copy.

---

## 🖊️ Keep author & inspiration inside `index.html`

Add this `<meta>` tag inside `<head>`:

```html
<meta name="author" content="David Carrero — https://carrero.es (Inspired by https://x.com/him_uiux/status/1971911092206293283)">
```

Optionally, add a header comment:

```html
<!--
  Built by David Carrero — https://carrero.es
  Inspired by: https://x.com/him_uiux/status/1971911092206293283
-->
```

---

## ⚙️ Quick customization

1) **Meta & brand:** update `<title>`, description, and swap `assets/logo.svg` & `assets/screenshot-hero.png`.  
2) **Hero:** replace `{{ProductName}}`, value proposition, and CTA URLs.  
3) **Partners / Benefits / How it works:** use outcome‑oriented copy.  
4) **Pricing:** edit `.price` (`data-m` monthly / `data-y` annual) and plan details.  
5) **Testimonials & FAQ:** add real quotes and 4–6 key questions.  
6) **Footer:** link to Privacy, Terms, DPA, Status, Blog, etc.

---

## 🧪 Run locally

Open `index.html` directly, or serve statically:

```bash
# Python
python3 -m http.server 5173

# or
npx serve -p 5173
```

Visit: http://localhost:5173

---

## ☁️ Deploy

### GitHub Pages
1. Push to `main`.  
2. Settings → Pages → **Source:** “Deploy from a branch”, **Branch:** `main` (root).

### Netlify / Vercel
- Connect the repo → Deploy as static site.  
- Build command: none, Output dir: `/`.

---

## 🔒 Accessibility & Performance

- AA/AAA contrast, keyboard navigation, `:focus-visible`.  
- Descriptive `alt` text and `sr-only` labels.  
- Tailwind via CDN (swap to built CSS if you need critical CSS).

---

## 🔍 SEO checklist (optional)

- [ ] `<title>` ≤ 60 chars & `<meta name="description">` ≤ 155 chars  
- [ ] Open Graph & Twitter Card  
- [ ] Favicon + `site.webmanifest`  
- [ ] `sitemap.xml` & `robots.txt`  
- [ ] Analytics with `defer`  
- [ ] Lighthouse pass (Performance / A11y / SEO)

---

## 🤝 Contributing

PRs welcome. Ideas: light/dark theme, blog/changelog, i18n, newsletter modal.

Steps: fork → branch `feat/my-change` → commit & push → PR.

---

## 📜 License

MIT License — see `LICENSE`.  
Please keep the author & inspiration credit in public forks.
