# Creative Green Landscaping

Single-page site for Creative Green Landscaping (Adelaide). Self-contained
`index.html`, built to mirror the Artisan Exterior design language with original
branding and copy. No build step, no dependencies.

## Deploy to GitHub Pages

From your Mac, in the cloned repo folder with these files in the root:

```
git add .
git commit -m "Creative Green site"
git push origin main
```

Then enable Pages: repo Settings > Pages > Build and deployment >
Deploy from a branch > Branch: main > Folder: / (root) > Save.

The site will serve at `https://the-service-edit.github.io/creative-green/`
until a custom domain is connected.

## Before it goes live

- Swap every placeholder image (all marked `REPLACE` in `index.html`) with
  client photography. Slots: hero, six service tiles, one statement image,
  one full-width feature, five gallery images.
- Replace the email `hello@creativegreen.com.au` (appears in the CTA,
  social rail, footer and structured data).
- The three testimonials are placeholder copy. Swap for real reviews.
- Wire the footer newsletter input to a handler (Web3Forms or similar).

## Domain and SEO

If using `www.creativegreen.com.au`, add a `CNAME` file containing that domain
and point DNS at GitHub Pages. If staying on the Pages subpath, update these to
the real URL: the `canonical` and `og:url` tags in `index.html`, the `<loc>` in
`sitemap.xml`, and the `Sitemap:` line in `robots.txt`.

## Deliberate divergences from Artisan

- No phone number or search glyph in the nav (house style: email-led, no phone
  as primary CTA, and no non-functional controls).
- Newsletter signup is styled but not yet wired.

## Files

- `index.html` - the site
- `404.html` - branded not-found page
- `robots.txt`, `sitemap.xml` - SEO
- `.nojekyll` - serve files as-is on Pages
