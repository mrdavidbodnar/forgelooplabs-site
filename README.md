# SEO fix package for forgelooplabs.com

## What's in here

- **index.html** — your real homepage, with only the `<head>` section changed:
  improved title/description, canonical tag, Open Graph tags, Twitter Card tags,
  and JSON-LD structured data (Organization + all 3 products). Nothing in `<body>`
  was touched — your markup, nav, sections, and content are untouched.
- **robots.txt** — new file, tells search engines the site is crawlable and points to the sitemap.
- **sitemap.xml** — new file, lists your homepage for indexing.

## How to drop in

1. Replace your repo's `index.html` with the one here (or diff it against your
   current version first if you've made other changes since you sent it to me).
2. Add `robots.txt` and `sitemap.xml` to the repo root (same folder as `index.html`).
3. Commit and push.

## Verify after it's live

- `https://forgelooplabs.com/robots.txt` and `/sitemap.xml` load correctly
- View page source on the homepage — confirm title/meta/OG tags are in `<head>`
- https://www.opengraph.xyz/ — paste your URL to preview social link previews
- https://search.google.com/test/rich-results — paste your URL to validate the JSON-LD

## Still outstanding (not a file fix)

Single-page site with anchor links (#models, #how-it-works, etc.) means Google
only indexes one URL. To rank "Weekend Recycler," "Recycler Pro," and "Lab Recycler"
separately, you'd eventually want real separate pages/routes per model. Say the
word and I'll sketch out that structure.
