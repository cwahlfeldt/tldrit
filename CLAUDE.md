# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**TLDR.it** - A collection of rapid reference guides for programming languages and tools. Static HTML pages with embedded CSS, no build process required.

## Architecture

- **Multi-page static site**: Each guide is a standalone HTML file
- **No build process**: Static HTML served directly
- **No JavaScript**: Pure HTML/CSS with CSS animations
- **No external dependencies**: Only Google Fonts loaded externally

## File Structure

- `index.html` - Landing page with links to all guides
- `zig.html` - Zig language reference (accent: `#f7a41d` orange)
- `rust.html` - Rust language reference (accent: `#f74c00` rust-orange)

## Development

To preview the site, open `index.html` in a browser or use any static file server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (if npx available)
npx serve .
```

## Adding a New Guide

1. Copy an existing guide (e.g., `rust.html`) as a template
2. Update the `--accent` and `--accent-glow` CSS variables in `:root`
3. Update content, version badge, and footer links
4. Add a card to `index.html` with appropriate `.guide-card.{name}` class and styles

## Styling Conventions

- CSS uses custom properties (variables) defined in `:root` for theming
- Base color scheme: Dark theme (`--bg: #0a0a0a`), each guide has its own accent color
- Fonts: JetBrains Mono (code), Space Grotesk (body), Instrument Serif (headings)
- Syntax highlighting classes: `.kw` (keywords), `.fn` (functions), `.str` (strings), `.num` (numbers), `.cmt` (comments), `.type` (types), `.builtin` (builtins), `.op` (operators)
- Each guide page includes a "Back to all guides" link in the header
