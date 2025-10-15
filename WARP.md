# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

This is a Jekyll-based GitHub Pages blog using the **Chirpy** theme (v7.3+). The site serves as Felix Schramm's personal blog and is deployed to https://felixschramm.eu.

## Essential Commands

### Development
```bash
# Install dependencies
bundle install

# Start development server (local)
bundle exec jekyll serve -l

# Start development server with custom host
bash tools/run.sh -H 0.0.0.0

# Start in production mode
bash tools/run.sh -p
```

### Build & Test
```bash
# Build site for production
JEKYLL_ENV=production bundle exec jekyll build

# Build and test (includes HTML validation)
bash tools/test.sh

# Test with custom config
bash tools/test.sh -c "_config.yml,_config_custom.yml"
```

### Content Creation
```bash
# Create new post (with jekyll-compose gem)
bundle exec jekyll post "Title of Post"

# Create new draft
bundle exec jekyll draft "Draft Title"

# Publish draft
bundle exec jekyll publish _drafts/draft-name.md
```

## Architecture & Content Structure

### Core Directories
- `_posts/` - Blog posts with naming convention `YYYY-MM-DD-title.md`
- `_tabs/` - Static pages (About, Archives, Categories, Tags) displayed in sidebar navigation
- `_data/` - YAML data files for authors, contact info, and social sharing
- `_plugins/` - Custom Jekyll plugins (includes Git-based last-modified tracking)
- `assets/` - Static assets (images, CSS, JS)

### Content Guidelines

**Blog Posts** (`_posts/`)
- Use front matter with required fields: `title`, `date`, `categories`, `tags`, `author`
- Support special Chirpy syntax:
  - Prompts: `{: .prompt-info}`, `{: .prompt-tip}`, `{: .prompt-warning}`, `{: .prompt-danger}`
  - File paths: `` `path/to/file`{: .filepath} ``
  - Code blocks with file attribution: `{: file="filename"}`
  - Line number disabling: `{: .nolineno}`
  - LaTeX math support enabled via `math: true`

**Navigation Tabs** (`_tabs/`)
- Order controlled by `order` field in front matter
- Use FontAwesome icons via `icon` field
- Default layout is `page`

### Theme Configuration
Key settings in `_config.yml`:
- Site metadata (title, tagline, description, URL)
- Social links and author info
- Theme mode, avatar, CDN settings
- Comment system integration (Disqus, Utterances, Giscus)
- Analytics providers
- PWA settings

### Git Integration
The site uses a custom plugin (`_plugins/posts-lastmod-hook.rb`) that automatically tracks post modification dates based on Git history. This sets `last_modified_at` for posts with multiple commits.

## Deployment

The site deploys automatically via GitHub Actions on pushes to `main`/`master`. The workflow:
1. Builds site with `bundle exec jekyll build` in production mode
2. Validates HTML using `htmlproofer`
3. Deploys to GitHub Pages

Manual deployment testing can be done using `tools/test.sh`.

## Development Notes

- The site inherits most layouts and includes from the Chirpy theme gem
- Custom modifications should be placed in the appropriate directories to override theme defaults
- Use `bundle info --path jekyll-theme-chirpy` to locate theme files for reference
- The site supports both light and dark themes with automatic switching
- Math rendering is available via LaTeX syntax when `math: true` is set in post front matter