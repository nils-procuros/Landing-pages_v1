# Landingpages_v1 — Claude Instructions

## Stack
- Pure HTML + CSS, no framework, no build tool
- Inter via Google Fonts (loaded in index.html)
- TWK Everett: currently using system-ui fallback. To activate, drop font files into `/fonts/` and uncomment the @font-face rules in `design-system.css`

## File Structure
```
index.html          — main page
styles.css          — all component + layout styles
design-system.css   — CSS custom properties (tokens)
fonts/              — (empty) place TWK Everett .woff2 files here when available
```

## Conventions
- Layout padding: 64px left/right (via `--layout-padding-x`)
- All design tokens live in `design-system.css` — never hardcode colors/sizes in `styles.css`
- Placeholders (logo, video) are `<div>` elements — replace with `<img>` or `<video>` when assets are ready
- BEM-style class naming: `.block__element--modifier`

## Deployment
- Will be pushed to GitHub and hosted on Vercel (static site, no config needed)
