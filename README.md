# The Syrup Lab

A minimal cocktail syrup calculator website. No tracking, no cookies, no JS frameworks.

## Stack

- Plain HTML, CSS, JavaScript — zero dependencies
- Google Fonts (Cormorant Garamond + DM Mono) loaded via CDN
- Cloudflare Pages for free hosting

## Project structure

```
syrup-site/
├── index.html       ← Landing page
├── gomme.html       ← Gomme syrup calculator
├── style.css        ← Shared stylesheet
├── _headers         ← Cloudflare security & cache headers
├── _redirects       ← Cloudflare URL redirects
└── README.md
```

## Deploy to Cloudflare Pages (free)

### Option A — Drag & drop (fastest)

1. Go to https://pages.cloudflare.com and sign in (free account)
2. Click **Create a project** → **Direct Upload**
3. Give the project a name (e.g. `the-syrup-lab`)
4. Drag the entire `syrup-site/` folder into the upload box
5. Click **Deploy** — your site will be live at `<name>.pages.dev` in seconds

### Option B — GitHub (recommended for updates)

1. Push this folder to a GitHub repository
2. In Cloudflare Pages → **Create a project** → **Connect to Git**
3. Select your repo; set **Build command** to *(empty)* and **Output directory** to `/` (or `.`)
4. Click **Save and Deploy**

Every future `git push` will auto-deploy.

## Adding more calculators

1. Copy `gomme.html` to a new file, e.g. `simple-syrup.html`
2. Update the calculator logic in the `<script>` block
3. Add a nav link in `<header>` in all HTML files
4. Uncomment / update the "coming soon" card on `index.html`

## Fonts & offline use

The site loads fonts from Google Fonts. If you want it to work fully offline,
download the two font files and host them locally, then update the `@import` in `style.css`.
