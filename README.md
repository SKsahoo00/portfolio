# Sumit Kumar Sahoo — Portfolio

A single-page portfolio built with React, TypeScript, Tailwind CSS and TanStack Start.

## Highlights

- **Gaze-tracking portrait** — nine head-pose crops stacked in the hero. The image that matches the
  angle from the character's centre to your cursor is shown instantly; touch devices drift through
  the poses slowly, and `prefers-reduced-motion` turns the motion off.
- **Textured deep-red theme** with cream "paper" sections, Caveat Brush for display type and
  Poppins for body copy.
- **Sections**: hero, work (concept project cards), about, skills, contact — all on one scrolling
  route with smooth-scroll anchored navigation.
- **Contact**: sumitkumarsahooofficial@gmail.com and WhatsApp +91 72051 05942.

## Development

You need Node.js 20+ (or Bun) — [install Node with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd portfolio
npm install     # or: bun install
npm run dev     # or: bun run dev
```

The site is then available at http://localhost:8080.

Other scripts:

```sh
npm run build      # production build
npm run preview    # serve the production build locally
npm run lint       # ESLint
npm run format     # Prettier
npm run test       # Vitest
```

## Project layout

```
src/
  routes/
    __root.tsx    # html shell, fonts, head metadata
    index.tsx     # the whole portfolio: hero, work, about, skills, contact
  assets/         # portrait crops and project thumbnails (WebP)
  components/ui/  # shadcn-style primitives
  lib/            # helpers
  styles.css      # design tokens (oklch colours) and custom utilities
public/
  images/         # hero background texture
  favicon.ico
  robots.txt
```

## Built with

- TanStack Start (React 19)
- TypeScript
- Tailwind CSS v4
- lucide-react icons
- shadcn/ui primitives
