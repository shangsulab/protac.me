# PROTAC.me

Simple static source for the `protac.me` portal.

## Files

- `index.html` — all page text and structure
- `style.css` — all visual styling
- `robots.txt` — currently asks crawlers not to index the site
- `CNAME` — custom domain for GitHub Pages
- `404.html` — fallback page

## Publish with GitHub Pages

1. Upload all files in this folder to the root of the `protac.me` repository.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select the `main` branch and `/ (root)`.
5. Set the custom domain to `protac.me`.
6. Do not change the existing DNS record for `docking.protac.me`.

## Search visibility

The site currently contains both:

- `robots.txt` with `Disallow: /`
- `noindex, nofollow` meta tags in `index.html`

This discourages normal search engines from indexing the site, but it is not password protection.

When ready for public indexing:

1. Change `robots.txt` to:

   ```
   User-agent: *
   Allow: /
   ```

2. Remove the robots meta tags from the `<head>` of `index.html`.

## Editing

All homepage wording is directly visible in `index.html`.  
No build process, framework, package installation, or JavaScript is required.


## Collaboration section

The homepage now includes:

- A direct link to `https://sushanglab.com`
- An academic-team description
- An open-for-collaboration section
- A direct email link to `ssu5@lsu.edu`
