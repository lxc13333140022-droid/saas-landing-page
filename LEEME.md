# 🚀 {{ProductName}} — Landing Page SaaS (Estática)

Landing orientada a conversión en un único `index.html`, siguiendo la anatomía “High‑Converting SaaS Landing Page” (hero → partners → beneficios → cómo funciona → precios → testimonios → FAQ → CTA → footer).
Publicación inmediata en GitHub Pages, Netlify, Vercel o cualquier hosting estático.

**Autor del HTML:** [David Carrero](https://carrero.es)  
**Inspirado en:** https://x.com/him_uiux/status/1971911092206293283

---

## ✨ Características

- HTML5 + Tailwind por CDN (sin *build*).
- Accesible por defecto (semántica, ARIA, focus, contraste).
- Bloques de copy orientados a **beneficios**.
- Navbar fija, CTAs dobles, logos de confianza, beneficios tipo *bento*.
- Cómo funciona (3 pasos), precios con toggle mensual/anual (JS nativo).
- Testimonios, FAQ, CTA final, meta SEO básica.
- Fácil de localizar (base en español).

---

## 📁 Estructura

```text
.
├─ index.html
├─ assets/
│  ├─ logo.svg
│  ├─ screenshot-hero.png
│  └─ og-cover.png
└─ LEEME.md
```

> El HTML incluye marcadores `{{…}}`. Sustitúyelos por tu marca, enlaces y textos.

---

## 🖊️ Autor e inspiración dentro de `index.html`

Añade esta metaetiqueta en el `<head>`:

```html
<meta name="author" content="David Carrero — https://carrero.es (Inspirado en https://x.com/him_uiux/status/1971911092206293283)">
```

Y, opcionalmente, este comentario al inicio del archivo:

```html
<!--
  Construido por David Carrero — https://carrero.es
  Inspirado en: https://x.com/him_uiux/status/1971911092206293283
-->
```

---

## ⚙️ Personalización rápida

1) **Meta & marca:** actualiza `<title>`, description y reemplaza `assets/logo.svg` y `assets/screenshot-hero.png`.  
2) **Hero:** cambia `{{ProductName}}`, propuesta de valor y URLs de CTA.  
3) **Partners / Beneficios / Cómo funciona:** redacta en clave de resultado.  
4) **Precios:** edita `.price` (`data-m` mensual / `data-y` anual) y detalles de planes.  
5) **Testimonios & FAQ:** añade citas reales y 4–6 preguntas clave.  
6) **Footer:** enlaza Privacidad, Términos, DPA, Estado, Blog, etc.

---

## 🧪 Probar en local

Abre `index.html` directamente o sirve estático:

```bash
# Python
python3 -m http.server 5173

# o
npx serve -p 5173
```

Visita: http://localhost:5173

---

## ☁️ Despliegue

### GitHub Pages
1. Sube a `main`.  
2. Settings → Pages → **Source:** “Deploy from a branch”, **Branch:** `main` (root).

### Netlify / Vercel
- Conecta el repo → Publica como sitio estático.  
- Comando de build: ninguno, Carpeta de salida: `/`.

---

## 🔒 Accesibilidad y rendimiento

- Contraste AA/AAA, navegación por teclado, `:focus-visible`.  
- Texto alternativo `alt` y etiquetas `sr-only`.  
- Tailwind por CDN (puedes migrar a CSS compilado si lo necesitas).

---

## 🔍 Checklist SEO (opcional)

- [ ] `<title>` ≤ 60 y `<meta name="description">` ≤ 155  
- [ ] Open Graph & Twitter Card  
- [ ] Favicon + `site.webmanifest`  
- [ ] `sitemap.xml` y `robots.txt`  
- [ ] Analítica con `defer`  
- [ ] Revisión Lighthouse (rendimiento / a11y / SEO)

---

## 🤝 Contribuciones

¡Se aceptan PRs! Ideas: tema claro/oscuro, blog/changelog, i18n, newsletter modal.

Pasos: fork → rama `feat/mi-cambio` → commit & push → PR.

---

## 📜 Licencia

Licencia MIT — ver `LICENSE`.
Por favor, mantén el crédito de autor e inspiración en *forks* públicos.
