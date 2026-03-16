# nberk.github.io

Personal site for Nick Berk, deployed at [nick-berk.com](https://nick-berk.com).

## Stack

- **Static site generator**: Hugo 0.158.0 extended
- **Hosting**: GitHub Pages via GitHub Actions
- **Custom domain**: `nick-berk.com` (CNAME in `static/CNAME`)

## Project Structure

```
hugo.toml              # Hugo configuration
content/               # Markdown content (homepage, blog posts)
layouts/               # HTML templates (baseof, partials, index)
assets/css/style.css   # Site-wide styles
static/                # Static files (favicon, headshot, CNAME)
.github/workflows/     # GitHub Actions deploy workflow
```

## Commands

```bash
# Local dev server
hugo server -D

# Build site
hugo --minify
```

## Deployment

Push to `main` triggers `.github/workflows/hugo.yml`, which builds with Hugo and deploys to GitHub Pages. No manual deploy step needed.

GitHub Pages source is set to **GitHub Actions** (not branch-based).
