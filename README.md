# MausBot pages

The published pages are Markdown files in `content/pages`. [Pages CMS](https://pagescms.org) edits them through `.pages.yml`. GitHub Pages renders them with the Cayman theme (`theme: jekyll-theme-cayman` in `_config.yml`), which is one of the themes GitHub Pages supports.

The original goclone snapshot of https://mausbot.com/sitemap.xml is in `mirror/`. Jekyll does not publish that folder.

## Edit in Pages CMS

1. Sign in at https://app.pagescms.org with the techfundoffice GitHub account.
2. Install the Pages CMS GitHub App on that account if it is not installed yet.
3. Open `techfundoffice/mausbot-pages`.
4. Edit a page under Pages. A save commits the Markdown file back to `main`.

Each page has a title, a description, a URL, and a body. The layout stays `default`, which is the Cayman theme layout.
