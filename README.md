# PSU-EXT Site

Landing page for PSU-EXT, built with [Astro](https://astro.build) + Tailwind CSS. Published at [psu-ext-org.github.io](https://psu-ext-org.github.io), linked from the Crowd Supply campaign.

## Development

```sh
npm install
npm run dev       # localhost:4321
```

```sh
npm run build      # production build to ./dist/
npm run preview    # preview the production build locally
```

## Deployment

Pushes to `main` trigger `.github/workflows/deploy.yml`, which builds the site and publishes `dist/` to GitHub Pages via GitHub Actions. In the repo's **Settings → Pages**, the source must be set to **GitHub Actions** for this to take effect.

## Structure

- `src/components/` — page sections (Hero, Hardware, Measurement, Scripting, etc.)
- `src/data/links.ts` — external links (Crowd Supply, GitHub repos, socials). Several are placeholders pending the live campaign URL and public repos — see the `TODO` comment at the top of the file.
- `src/assets/images/` — sourced from the private `psu-ext-private` repo's `.doc/_media/`.
