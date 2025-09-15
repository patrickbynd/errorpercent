# errorpercent

A tiny static site to reproduce a Lighthouse split: 1 URL passes and 9 URLs fail during the audit (e.g., timeout/NO_FCP) while keeping the sitemap valid with absolute URLs.

- 10 absolute URLs in the sitemap
- 9 URLs include `?stall=1` to intentionally stall before first paint
- GitHub Pages deployment via Actions generates sitemap and robots with your repo URL

## Deploying on GitHub Pages
1. Create a new GitHub repository and push this folder to `main`.
2. The included workflow deploys to Pages and generates `sitemap.xml` and `robots.txt`.
3. Your site will be at `https://<your-user>.github.io/<repo>/` after the workflow runs.

You can ignore local dev; hosting is handled by GitHub Pages.

