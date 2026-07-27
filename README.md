# Dolerite documentation

The merchant-facing documentation for the Dolerite Shopify theme, published with
GitHub Pages. Excluded from the built site — this file is for whoever maintains it.

## Publishing

1. Push this repository to GitHub.
2. **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch `main`, folder `/ (root)`.
3. Wait for the first build, then open
   `https://<user>.github.io/dolerite-docs/`.

`_config.yml` holds `url` and `baseurl`. They are set for a project site at
`/dolerite-docs`. If a custom domain is added later, change those two lines and add a
`CNAME` file — every link on the site runs through `relative_url`, so nothing else
needs touching.

## The two URLs in the theme

The theme's `config/settings_schema.json` carries two attributes that Shopify surfaces
in the editor's Theme actions menu, and that Theme Store reviewers open:

| Attribute | Points at |
| --- | --- |
| `theme_documentation_url` | The root of this site |
| `theme_support_url` | The support contact form |

They must be **two distinct URLs**, and neither may point at a marketing page.

## Editing

Pages are plain Markdown with two lines of front matter (`title`, `description`).
The sidebar is `_data/nav.yml` — adding a page means adding a file and a line there.

Links between pages are written as `[text](other-page.md)`. GitHub Pages runs
`jekyll-relative-links` by default, which rewrites them to the built URLs, so the same
link works both in GitHub's file view and on the published site.

Headings get their ids from kramdown: lowercased, punctuation dropped, spaces to
hyphens. `## Mega menu promos` becomes `#mega-menu-promos`.

## Source of truth

These pages are maintained in the theme repository at `docs/merchant/` and copied here.
Edit them there, so the documentation ships and versions with the code it describes.

## Local build (optional)

Not required — GitHub builds the site on push. To preview locally you need Ruby:

```bash
bundle install
bundle exec jekyll serve
```
