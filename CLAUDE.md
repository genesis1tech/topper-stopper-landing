# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static landing page for "Helios Robotics | Robi" - a promotional page for a fictional home guardian robot. The project consists of a single self-contained HTML file with no build process.

## Technology Stack

- **Single-file HTML** with inline CSS and JavaScript
- **Tailwind CSS** via CDN (`cdn.tailwindcss.com`)
- **Lucide Icons** via CDN (`unpkg.com/lucide`)
- **Google Fonts** (Inter, plus multiple font families loaded for flexibility)

## Development

No build commands are required. To preview:
- Open `generated-page.html` directly in a browser
- Or use a local server: `python3 -m http.server 8000` then visit `http://localhost:8000/generated-page.html`

## Architecture Notes

The HTML file is fully self-contained with:
- Inline `<style>` blocks for custom CSS (glass-panel effects, animations)
- Inline `<script>` blocks for JavaScript (number counter animation, intersection observer for fade-ins)
- All assets are external (hosted on Supabase storage)

## Key UI Components

- **Navigation**: Fixed navbar with glass-panel styling
- **Hero Section**: Full-width with background image and CTA
- **Features Grid**: Three glass-panel cards with feature descriptions
- **Specs Section**: Product specifications table with stat cards
- **Footer**: Email signup form and social links
