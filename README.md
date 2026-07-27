# Shibuya Punk Portfolio

> A premium personal portfolio that feels like walking through Shibuya at midnight.  
> Editorial. Raw. Tactile. Asymmetric. Unforgettable.

![Astro](https://img.shields.io/badge/Astro-5.x-FF5D01?style=flat-square&logo=astro&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.x-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat-square&logo=typescript&logoColor=white)

---

## Design Philosophy

Inspired by Japanese underground fashion, editorial magazines, street posters, brutalist design, offset print, and Shibuya wayfinding signage. Not cyberpunk — **Shibuya Punk**.

## Features

- **11 sections**: Hero, Profile, Skills, Featured Project, Projects (with filters), Gallery (with lightbox), Statistics, Marquee, Contact, Footer
- **Signature scroll navigation** inspired by subway wayfinding
- **Micro-interactions**: Magnetic buttons, tilt cards, cursor spotlight, scroll reveal
- **Editorial design**: Hard shadows, paper textures, grain overlays, torn edges, masking tape effects
- **Dark mode only** with a curated crimson/brown/orange palette
- **Mobile-first** responsive design
- **Accessible**: ARIA labels, keyboard navigation, semantic HTML, focus states
- **SEO optimized**: Meta tags, Open Graph, structured headings
- **GitHub Pages** deployment via GitHub Actions

## Tech Stack

| Technology | Purpose |
|---|---|
| Astro 5 | Static Site Generation |
| Tailwind CSS 4 | Utility-first styling |
| TypeScript | Type safety |
| GitHub Actions | CI/CD deployment |

## Getting Started

### Prerequisites

- Node.js 20+
- npm 9+

### Installation

```bash
npm install
```

### Development

```bash
npm run dev
```

Open [http://localhost:4321](http://localhost:4321) in your browser.

### Build

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## Project Structure

```
src/
├── components/
│   ├── Navigation.astro
│   ├── ScrollSignature.astro
│   ├── hero/HeroSection.astro
│   ├── profile/ProfileSection.astro
│   ├── skills/SkillsSection.astro
│   ├── projects/FeaturedProject.astro
│   ├── projects/ProjectsSection.astro
│   ├── gallery/GallerySection.astro
│   ├── stats/StatsSection.astro
│   ├── marquee/MarqueeSection.astro
│   ├── contact/ContactSection.astro
│   └── footer/FooterSection.astro
├── layouts/BaseLayout.astro
├── pages/index.astro
├── styles/global.css
└── utils/scripts.astro
public/
└── favicon.svg
.github/workflows/
└── deploy.yml
```

## Customization

1. **Personal info**: Update name, tagline, bio, and contact details in the component files
2. **Projects**: Edit the `projects` array in `ProjectsSection.astro`
3. **Skills**: Modify skill cards and proficiency percentages in `SkillsSection.astro`
4. **Images**: Replace placeholder elements with your actual images
5. **Colors**: Adjust the color palette in `global.css` under `@theme`
6. **GitHub Pages base path**: Update `base` in `astro.config.mjs` to match your repository name

## Deployment

This project includes a GitHub Actions workflow for automatic deployment to GitHub Pages.

1. Push to the `main` branch
2. Go to **Settings → Pages** in your GitHub repository
3. Under **Source**, select **GitHub Actions**
4. The site will deploy automatically on each push to `main`

## License

MIT
