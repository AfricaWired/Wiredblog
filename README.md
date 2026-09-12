# AfricaWired — Jekyll site

A static-site port of the AfricaWired company/blog site (originally a Django app at
`~/Desktop/africawired`), rebuilt in Jekyll on the same HTML5-UP "Massively" theme,
same orange/navy branding, and the same blog content.

## Run locally

```bash
bundle install
bundle exec jekyll serve
```

Visit http://localhost:4000

## Structure

- `index.html`, `about.md`, `services.md` — marketing pages
- `blog/index.html` — paginated blog listing (`paginate_path: /blog/page:num/` in `_config.yml`)
- `categories/*.html` — one static page per category, filtering `site.posts`
- `_posts/` — blog posts (Markdown, front matter: `title`, `category`, `author`, `date`)
- `_layouts/`, `_includes/` — page templates
- `_data/services.yml`, `_data/team.yml`, `_data/categories.yml` — editable content that
  doesn't need a new post/page (services list, founding team, category names/descriptions)
- `assets/` — the Massively theme's CSS/JS/webfonts/images (light + dark compiled
  stylesheets), plus `assets/css/custom.css` for AfricaWired-specific additions

## Known differences from the Django version

This is a static site, so a few dynamic features from the Django app aren't present:

- **No comments** — commenting required a logged-in account server-side; there's no
  backend here to authenticate against or store comments.
- **No login/register** — no backend, so no accounts.
- **No live search** — the Django blog's search box hit a database; this would need a
  client-side JS index (e.g. Lunr.js) to replicate, not added here.
- **View counts** — not tracked (would need a server or a third-party analytics embed).

Everything else — pages, categories, pagination, the post content, dark/light toggle,
RSS feed, sitemap — is ported over.
