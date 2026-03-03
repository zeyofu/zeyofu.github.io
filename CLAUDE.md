# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal academic website for Xingyu Fu, hosted on GitHub Pages at zeyofu.github.io. This is a **pure static site** — no build system, no static site generator, no package.json or Gemfile.

## Development

No build or install step. Edit HTML/CSS/JS files directly. To preview locally, open `index.html` in a browser or use any static file server (e.g., `python3 -m http.server`).

## Architecture

- **`index.html`** — Main homepage with bio, highlights, and research publications
- **`pages/`** — Additional pages (golf.html, 404.html)
- **`asset/css/style.css`** — Custom styles (Bootstrap CSS is also in asset/css/)
- **`asset/image/`** — Profile picture and paper thumbnail images
- **`asset/pdfs/`** — PDFs tracked with Git LFS (see .gitattributes)
- **`js/`** — Vendored libraries (Bootstrap, jQuery, Chart.js, etc.)
- **`charts.js`** — Chart.js configurations for data visualizations

## Key Conventions

- Uses Bootstrap 4/5 grid for responsive layout
- Font Awesome for icons (loaded from asset/css/all.css and asset/webfonts/)
- New research papers are added as rows in the publications section of index.html, typically with a thumbnail image in asset/image/ and links to paper/website/code/dataset
- PDFs must be added via Git LFS (`asset/pdfs/*.pdf` is configured in .gitattributes)
