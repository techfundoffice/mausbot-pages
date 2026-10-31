# MausBot pages

Static copy of every page in [the MausBot sitemap](https://mausbot.com/sitemap.xml), saved with goclone. `.pages.yml` tells [Pages CMS](https://pagescms.org) how to open those HTML files.

## Edit in Pages CMS

1. Sign in at [app.pagescms.org](https://app.pagescms.org) with the techfundoffice GitHub account.
2. Install the Pages CMS GitHub App on that account if it is not installed yet.
3. Open `techfundoffice/mausbot-pages`.
4. Edit a page. A save commits back to `main`.

The media library is the `imgs` folder. Uploads go there.

## GitHub Pages

This repo is private. `.nojekyll` is in the root so GitHub Pages can serve the HTML and the `css`, `js`, and `imgs` folders from `main` without running Jekyll. Page links are relative, so they keep working when the site is published under a project path.
