# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Landing page for **Topper Stopper™** by Waste Wise Innovation - a smart recycling bin technology that prevents contamination and provides real-time data insights.

## Tech Stack

- **Astro 4** - Static site generator with zero-JS by default
- **Tailwind CSS** - Utility-first CSS framework
- **TypeScript** - Type safety throughout
- **Lucide Icons** - Icon library (via lucide-astro)

## Commands

```bash
npm install      # Install dependencies
npm run dev      # Start dev server at localhost:4321
npm run build    # Build for production (outputs to dist/)
npm run preview  # Preview production build locally
npm run format   # Format code with Prettier
```

## Project Structure

```
src/
├── components/     # Reusable Astro components
│   ├── Navbar.astro
│   ├── Hero.astro
│   ├── TrustedBy.astro
│   ├── HowItWorks.astro
│   ├── Features.astro
│   ├── Results.astro
│   ├── About.astro
│   ├── Contact.astro
│   ├── Footer.astro
│   └── Observer.astro  # Intersection observer for animations
├── layouts/
│   └── Layout.astro    # Base HTML layout with global styles
└── pages/
    └── index.astro     # Main landing page (composes components)
```

## Architecture Notes

- **Component-based**: Each page section is a separate `.astro` component
- **Path aliases**: Use `@components/*` and `@layouts/*` for imports
- **Animations**: Fade-in animations use `fade-in-section` class with IntersectionObserver
- **Custom colors**: Extended Tailwind with `eco-*` color palette (green theme)
- **Glass effects**: `.glass-panel` and `.glass-panel-dark` utility classes defined in Layout

## Styling Conventions

- Use Tailwind utility classes directly in components
- Custom CSS goes in `<style>` blocks within components or `is:global` in Layout
- Color palette: `eco-50` through `eco-950` for brand greens
- Rounded corners: Use `rounded-[2rem]` or `rounded-[3rem]` for cards/panels
