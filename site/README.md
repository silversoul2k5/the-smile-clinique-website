# The Smile Clinique — Website

A modern one-page website for **The Smile Clinique**, a dental clinic on the Vallikkavu–Oachira Road, Karunagappalli, Kerala (5.0★, 95 Google reviews).

- Plain HTML / CSS / JS — no build step, no dependencies.
- Sections: Hero, trust strip, About, Services, Doctor, Gallery, Reviews, Visit/Map, WhatsApp CTA, Footer.
- Floating + header WhatsApp button → `https://wa.me/918714797199`
- Embedded Google Map of the clinic's real location.
- Clinic photos are pulled live from Google Maps (hot-linked Google-hosted URLs). For a permanent, faster site, replace the `<img>` `src` values in `index.html` with your own photos saved into a local `/images` folder.

## Run locally

Just open `index.html` in a browser, or serve it:

```bash
npx serve .
```

## Deploy to GitHub + Vercel

1. Create a new GitHub repository and push this folder:
   ```bash
   git init
   git add .
   git commit -m "Initial site: The Smile Clinique"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```
2. Go to [vercel.com](https://vercel.com), click **Add New → Project**, and import the GitHub repo.
3. Framework preset: **Other** (static site) — no build command, no output directory needed (or set Output Directory to `.`).
4. Click **Deploy**. Vercel will give you a live `*.vercel.app` URL immediately; you can attach a custom domain afterwards in Project → Settings → Domains.

## Editing content

- Address, phone, hours, doctor name, review text and services all live directly in `index.html` — search for the relevant section comment (`<!-- HERO -->`, `<!-- SERVICES -->`, etc.).
- Colors, fonts and spacing are controlled by CSS variables at the top of `css/style.css`.
