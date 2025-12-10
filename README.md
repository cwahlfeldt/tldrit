# TLDR.it

Rapid reference guides for programming languages and tools. Everything you need to know, distilled to the essentials.

## What is TLDR.it?

A collection of fast, scannable reference guides for developers. No frameworks, no build process, just clean HTML and CSS.

## Current Guides

- **Zig** (v0.15.1) - Systems programming, "better C"
- **Rust** (v1.91.1) - Memory safety without garbage collection
- **C** (C23) - The foundational systems language
- **Python** (v3.13) - High-level, readable, versatile

## Features

- **Fast to scan** - No fluff, just the syntax and patterns you need
- **Copy-paste ready** - Complete, runnable code examples
- **Essentials only** - Covers 90% of daily use cases
- **Dark mode native** - Easy on the eyes
- **No dependencies** - Pure HTML/CSS, loads instantly

## Local Development

No build process required. Just open `index.html` in a browser or use any static server:

```bash
# Python
python -m http.server 8000

# Node.js
npx serve .

# PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

## Project Structure

```
tldrit/
├── index.html          # Landing page
├── styles.css          # Shared styles
├── zig.html           # Zig reference
├── rust.html          # Rust reference
├── c.html             # C reference
├── python.html        # Python reference
└── README.md          # This file
```

## Contributing a New Guide

1. Copy an existing guide (e.g., `rust.html`) as a template
2. Update the `--accent` and `--accent-glow` CSS variables in `:root`
3. Update content, version badge, and footer links
4. Add a card to `index.html` with the appropriate `.guide-card.{name}` class and styles
5. Choose a unique accent color and icon shape for visual distinction

## Design Conventions

- **Colors**: Each guide has its own accent color (defined in CSS variables)
- **Fonts**: JetBrains Mono (code), Space Grotesk (body), Instrument Serif (headings)
- **Syntax highlighting**: Semantic classes (`.kw`, `.fn`, `.str`, `.num`, `.cmt`, `.type`, etc.)
- **Structure**: Consistent sections with clear navigation

## License

MIT
