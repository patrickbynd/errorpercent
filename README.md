# errorpercent

A tiny static site to reproduce a Lighthouse split: ~70% URLs valid and ~30% fail immediately with "The URL you have provided appears to be invalid." when a runner consumes the `sitemap.xml`.

- 7 valid pages with absolute URLs in the sitemap
- 3 intentionally invalid entries (relative path, protocol-relative, and missing scheme)
- GitHub Pages deployment via Actions generates sitemap and robots with your repo URL

## Deploying on GitHub Pages
1. Create a new GitHub repository and push this folder to `main`.
2. The included workflow deploys to Pages and generates `sitemap.xml` and `robots.txt`.
3. Your site will be at `https://<your-user>.github.io/<repo>/` after the workflow runs.

You can ignore local dev; hosting is handled by GitHub Pages.
