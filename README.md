# Blur website

Static site for https://blur.hazcod.com. Plain HTML and CSS, no build step, no JavaScript, no external requests, no analytics or cookies.

Files: `index.html`, `style.css`, `favicon.svg`, `robots.txt`, `sitemap.xml`, `CNAME`.

Product source and setup instructions live in [hazcod/blur](https://github.com/hazcod/blur). Keep platform status, build names and privacy claims consistent with that repository.

## Hosting

Upload this repository's root to any static host. There is no `website/` subdirectory or build step.

### GitHub Pages

1. Publish from the `main` branch and `/` (root) in the repository's Pages settings.
2. In the repository settings, set the custom domain to `blur.hazcod.com`. The `CNAME` file already contains it.
3. Add a DNS `CNAME` record for `blur` pointing to `hazcod.github.io`.

### Preview locally

    python3 -m http.server 8080

Open `http://localhost:8080`. Check the page at desktop and narrow mobile widths, tab through the navigation and setup links, and confirm each platform links to the correct guide section. This site must remain usable without JavaScript and must not load third-party fonts, tracking or other external subresources.
