# MausBot pages

Visitor site: https://techfundoffice.github.io/mausbot-pages/

That is the GitHub Pages staging site. It serves the cloned pages in `mirror/`. Do not open https://mausbot.com when you are checking this repo.

`.github/workflows/pages.yml` publishes `mirror/` as the site root. The Markdown files in `content/pages` stay in the repo so [Pages CMS](https://pagescms.org) can edit them through `.pages.yml`. Those Markdown files are not the visitor site.

## Edit in Pages CMS

1. Sign in at https://app.pagescms.org with the techfundoffice GitHub account.
2. Install the Pages CMS GitHub App on that account if it is not installed yet.
3. Open `techfundoffice/mausbot-pages`.
4. Edit a page under Pages. A save commits the Markdown file back to `main`.

Each page has a title, a description, a URL, and a body. Saving in Pages CMS updates the Markdown file. It does not replace the cloned HTML that visitors see.
