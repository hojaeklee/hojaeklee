# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a personal website built with Hugo static site generator using the hugo-book theme. The site is titled "One Layer Deeper" and is deployed to GitHub Pages at https://hojaeklee.github.io/.

## Architecture

The project follows standard Hugo conventions:
- **content/**: Contains all markdown content files
  - `docs/`: Documentation section
  - `til/`: "Today I Learned" blog posts
  - `posts/`: Blog posts (currently empty)
- **themes/hugo-book/**: Git submodule containing the hugo-book theme
- **public/**: Generated static site files (gitignored in production)
- **static/**: Static assets (currently empty, theme provides defaults)
- **archetypes/**: Content templates for new pages

## Key Commands

### Development
```bash
# Start development server with live reload
hugo server -D

# Start server with specific theme (if not set in config)
hugo server --theme hugo-book

# Start server with minification
hugo server --minify
```

### Building
```bash
# Build the static site
hugo

# Build with minification
hugo --minify

# Build including draft content
hugo -D
```

### Content Management
```bash
# Create new content
hugo new docs/new-page.md
hugo new til/2025-05-26-new-learning.md
hugo new posts/new-post.md
```

## Configuration

Main configuration is in `hugo.toml`:
- `baseURL`: Set to GitHub Pages URL
- `bookSection`: Set to "*" to include all content in navigation
- Theme is implicitly set to hugo-book via git submodule

## Theme Customization

The hugo-book theme supports customization through:
- `assets/_custom.scss`: Custom styles
- `assets/_variables.scss`: Override SCSS variables
- `static/favicon.png`: Custom favicon
- `layouts/partials/`: Override theme partials

## Content Structure

Content files use Hugo front matter:
- `title`: Page title
- `date`: Publication date
- `draft`: Draft status
- `weight`: Menu ordering
- `bookToC`: Show/hide table of contents
- `bookCollapseSection`: Collapse section in menu

## Deployment

The site appears to be configured for GitHub Pages deployment. The `public/` directory contains the built site with multiple search index versions, suggesting iterative builds.