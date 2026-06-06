# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project: BIBAS Website

Static HTML/CSS/JS website for BIBAS (Bankon International Business And Supply), a Belgian company based in Brussels specializing in product sourcing between Europe and Africa.

## File Structure

```
bibas/
├── index.html          — Homepage (hero, services overview, products, stats, process, CTA)
├── services.html       — Services detail page (sourcing, quality, logistics, documentation)
├── produits.html       — Product catalog with sidebar filter + search
├── a-propos.html       — About page (story, mission, timeline, team, certifications)
├── contact.html        — Contact page (form, FAQ, map)
├── css/style.css       — All styles (CSS variables, responsive breakpoints)
├── js/main.js          — Header scroll, mobile menu, fade-in, counter, contact form, tabs
└── photo/              — Company assets (logos, product images)
```

## Design System

- **Colors:** Navy `#0D1B3E`, Yellow/Gold `#F0BE00`, White `#FFFFFF`, Black `#0A0A14`
- **Font:** Poppins (Google Fonts CDN)
- **Icons:** Font Awesome 6.5 (CDN)
- **Logo:** `photo/logo_bibas_blue.jpeg` for light backgrounds, CSS text logo for dark backgrounds

## Real Company Data

- **Phone:** +32 465 52 32 32
- **Email:** contact@bibas.eu
- **Website:** www.bibas.eu
- **Address:** Brussels, Belgium
- **Managing Partner:** Jacques Lea Ebongue
- **Key differentiator:** "Nous opérons sans stockage" (on-demand sourcing only)

## Development

No build process — open any HTML file directly in a browser. All external dependencies load from CDN (Google Fonts, Font Awesome). Product images use Unsplash CDN URLs.

## Product Categories (produits.html)

Data attributes `data-category` on `.prod-card` elements control the JS filter:
- `pharma` — Pharmaceuticals
- `cosmetique` — Cosmetics  
- `alimentaire` — Food products
- `autre` — Equipment & other
