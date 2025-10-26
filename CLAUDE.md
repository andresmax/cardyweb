# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static website for cardy.so - a simple, single-page landing page with no build process or dependencies.

## Architecture

**Technology Stack:**
- Pure HTML/CSS/JavaScript (no framework)
- Tailwind CSS via CDN (configured inline in index.html:56-67)
- Plus Jakarta Sans font via Google Fonts
- Progressive Web App (PWA) with service worker capabilities

**Key Files:**
- `index.html` - Single page containing all markup, styles, and Tailwind configuration
- `site.webmanifest` - PWA manifest file defining app metadata and icons
- `robots.txt` - Blocks all search engines and crawlers
- `assets/` - Logo files, favicons, and icons for various platforms

**Design Patterns:**
- Dark mode support via `prefers-color-scheme` media query
- Mobile-first responsive design with iOS Safari-specific fixes
- Comprehensive bot blocking via meta tags (index.html:9-19)
- Fallback logo display if SVG fails to load (index.html:101-103)

## Development Commands

**Local Development Server:**
```bash
# Python 3
python -m http.server 8000

# Node.js
npx http-server

# PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

**Deployment:**
This is a static site - simply upload all files to any web host. No build step required.

## Important Notes

- **No package.json or build process** - all dependencies loaded via CDN
- **Theme color is #01C3FF** - used consistently across PWA manifest and meta tags
- **Bot blocking is intentional** - site blocks all search engines and AI crawlers
- **iOS optimizations** - viewport-fit=cover and -webkit-fill-available used for proper iOS display
- **Tailwind config is inline** - modify the `tailwind.config` object in index.html:57-66, not an external file
