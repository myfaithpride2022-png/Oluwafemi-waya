# Oluwafemi Waya — Portfolio

A playful, Meeko-inspired portfolio built with **Astro + Tailwind CSS v4**.
Same structure and energy as the Meeko Framer template — hero with rotating
photos, quick-nav cards, selected works, about, and contact — re-skinned in a
tangerine/cream palette and tailored for a website developer.

## Quick start

Requires Node.js 22 or newer.

```bash
npm ci
npm run dev      # local dev at http://localhost:4321
npm run build    # production build -> dist/
npm run preview  # preview the production build
```

GitHub Actions runs the production build for pushes to `main` and pull requests
targeting `main`.

## Deploy to Vercel

**Option A — GitHub (recommended):**
1. Push this folder to a GitHub repo.
2. Go to [vercel.com](https://vercel.com) → **Add New → Project** → import the repo.
3. Vercel auto-detects Astro. No build settings needed — just hit **Deploy**.

**Option B — CLI:**
```bash
npm i -g vercel
vercel
```

## Customising

| What | Where |
|---|---|
| Hero text, tags, photos | `src/components/Hero.astro` + `public/images/me-1..3.png` |
| Project cards & links | `src/components/SelectedWorks.astro` |
| Bio, stack, education | `src/components/About.astro` |
| Email & socials | `src/components/Contact.astro`, `src/components/Footer.astro`, `src/components/Nav.astro` |
| Colors & fonts | `src/styles/global.css` (`@theme` block) |
| Site URL (SEO) | `astro.config.mjs` → `site` |

### Swap the project mockups
The `work-*.png` files in `public/images/` are generated placeholders.
Replace them with real screenshots (keep the same filenames, ~1200×880 for
featured, ~900×660 for "More builds") — no code changes needed.
