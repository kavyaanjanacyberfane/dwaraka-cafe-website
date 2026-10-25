# Dwaraka Cafe Website

Responsive Nuxt 3 + Vue 3 website for Dwaraka Cafe, a pure vegetarian restaurant in Patancheru Industrial Area, Hyderabad.

## Run locally
Use Node.js 20 or newer.

```bash
npm install
npm run dev
```

Open the local URL shown in the terminal (usually http://localhost:3000).

## Production
```bash
npm run build
npm run preview
```

## Pages
- `/` Home
- `/about` About
- `/contact` Contact and location

## Before publishing
- Replace `https://dwarakacafe.com` in `nuxt.config.ts` and page SEO with the real live domain.
- Confirm address, telephone, business name, opening hours, and Google Business Profile URL.
- Add official social profiles when available.
- Check `/sitemap.xml` after deployment. `@nuxtjs/seo` supplies sitemap and Schema.org integration.
- The contact-page map is a designed visual that links to Google Maps, not an embedded map.

## Assets
- `public/images/dwaraka-cafe-logo.png`: supplied logo
- `public/images/google-review-poster.png`: supplied review poster
