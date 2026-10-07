# Landing Page (Astro + TypeScript)

Production-ready Astro foundation prepared for MCP / Figma design handoff.

## Project Structure

```text
/
├── public/                     # Static files (favicon, robots.txt, etc.)
├── src/
│   ├── assets/                 # Optimized design assets (images, icons)
│   ├── components/             # Modular section components
│   │   ├── Header.astro        # Header / Navigation
│   │   ├── Hero.astro          # Hero section
│   │   ├── SupportingContent.astro # Social proof / overview / logos
│   │   ├── Features.astro      # Feature & content grid
│   │   ├── CTA.astro           # Call to action section
│   │   └── Footer.astro        # Footer & legal links
│   ├── layouts/
│   │   └── BaseLayout.astro    # Master layout with SEO meta & OG tags
│   ├── pages/
│   │   └── index.astro         # Main landing page at /
│   └── styles/
│       └── global.css          # Modern CSS reset & design token variables
├── astro.config.mjs            # Astro configuration
└── tsconfig.json               # TypeScript configuration with path aliases
```

## TypeScript Path Aliases

- `@components/*` → `src/components/*`
- `@layouts/*` → `src/layouts/*`
- `@assets/*` → `src/assets/*`
- `@styles/*` → `src/styles/*`

## Commands

| Command | Action |
| :--- | :--- |
| `npm run dev` | Starts local dev server at `localhost:4321` |
| `npm run build` | Builds static production bundle to `./dist/` |
| `npm run check` | Runs Astro & TypeScript diagnostics |
| `npm run preview` | Previews production build locally |

## Design Handoff Ready

When design specifications arrive from Figma / MCP:
1. Populate design tokens in [`src/styles/global.css`](file:///Users/nael/Desktop/Amir/stampdlanding/src/styles/global.css) (colors, typography, spacing).
2. Drop visual assets (SVGs, imagery) into [`src/assets/`](file:///Users/nael/Desktop/Amir/stampdlanding/src/assets/).
3. Implement exact layout, copy, and components inside the modular section templates in [`src/components/`](file:///Users/nael/Desktop/Amir/stampdlanding/src/components/).
