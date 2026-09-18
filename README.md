# Digi Money Plug — Landing Page

A single sign-up landing page for **Digi Money Plug**, an app that consolidates verified ways for everyday people to earn and save money online.

**Live site (local dev server):** [http://127.0.0.1:5500/day_3_landing_page_project/](http://127.0.0.1:5500/day_3_landing_page_project/)

## Structure

```
day_3_landing_page_project/
├── index.html   # Page markup + scroll-reveal script
├── styles.css   # All styling
└── README.md
```

No build step or dependencies — just static HTML/CSS/JS. Open `index.html` directly in a browser, or serve the folder with any static file server.

## Sections

1. **Hero** — one-line title, one-sentence subheading, and a phone mockup preview.
2. **How It Works** — 3-step process.
3. **Why Digi Money Plug** — 6-item feature grid.
4. **Top Features** — the 3 opportunity types on a dark contrast panel: earn money online, get verified discounts, and find passive income.
5. **Call to Action** — email sign-up form.

## Design

- **Font:** [Nunito](https://fonts.google.com/specimen/Nunito) (Google Fonts)
- **Palette:** light background with hot-pink (`#FF2D78`) and neon-green (`#39FF14`) accents, defined as CSS custom properties in `:root` at the top of `styles.css`
- **Animations:** elements tagged with the `.reveal` class fade/slide in on scroll via `IntersectionObserver` (see the script at the bottom of `index.html`). Falls back to fully visible content if JavaScript is unavailable, and respects `prefers-reduced-motion`.

## Customizing

- Colors, spacing, and radius live as CSS variables in `styles.css` (`:root` block) — change once, applies everywhere.
- The sign-up form (`.signup-form` in the CTA section) currently just prevents default submission (`onsubmit="return false;"`) — wire it up to your email provider or backend endpoint.
