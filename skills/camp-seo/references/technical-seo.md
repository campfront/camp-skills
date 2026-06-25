# Technical SEO checklist (camp sites)

Load this for the full-build tier, or when a camp's pages are indexed slowly, dropping, or not appearing at all. This is the general technical foundation, trimmed to what a small camp site actually needs. Work top down: a page cannot rank if it cannot be crawled and indexed, so fix those first.

## 1. Crawlability

The site must let search engines find and read its pages.

- **robots.txt**: check it does not block important pages by accident, and that it references the XML sitemap.
- **XML sitemap**: exists, is submitted to Search Console, lists only canonical and indexable URLs, and updates when pages change.
- **Site architecture**: important pages within three clicks of the homepage, a logical hierarchy, no orphan pages (pages with no internal links pointing to them).

For a small camp site this is usually simple. Most site builders generate a sitemap automatically; confirm it exists at `/sitemap.xml` and is submitted.

## 2. Indexation

Being crawlable is not the same as being indexed.

- Check coverage in Search Console, and compare indexed pages against the pages you expect.
- Watch for accidental `noindex` tags on pages you want found.
- Canonical tags should point the right way (a page should usually canonical to itself).
- Avoid redirect chains and loops, soft 404s, and duplicate pages without a canonical.

## 3. Canonicalization

Duplicates split ranking strength and confuse search engines.

- Every page has a canonical tag, and unique pages self-reference (`/programs/soccer` canonicals to `/programs/soccer`).
- Be consistent on HTTP versus HTTPS, www versus non-www, and trailing slashes. Pick one form and redirect the others.
- Never point a program page's canonical at the homepage; that hides the program page from search.

## 4. Site speed and Core Web Vitals

Most parents search on a phone, and slow pages lose both rankings and visitors. Targets:

- **LCP** (largest contentful paint, how fast the main content appears): under 2.5s.
- **INP** (interaction to next paint, how responsive the page feels): under 200ms.
- **CLS** (cumulative layout shift, how much the page jumps as it loads): under 0.1.

Most common fixes for a camp site: compress and resize photos (the usual culprit), serve modern image formats (WebP), enable caching, and lazy-load images below the fold. Measure with PageSpeed Insights and the Search Console Core Web Vitals report.

## 5. Mobile

- Responsive design, not a separate mobile site.
- Tap targets large enough, readable font sizes, viewport configured.
- No horizontal scroll.
- The same content on mobile as desktop (Google indexes the mobile version).

## 6. Security

- HTTPS across the whole site, with a valid certificate.
- No mixed content (HTTP assets on an HTTPS page).
- HTTP redirects to HTTPS.

## 7. URL hygiene

- Readable and descriptive: `/programs/soccer-day-camp-denver`, not `/p?id=123`.
- Hyphens, not underscores; lowercase always.
- Reflect the hierarchy, and keep it shallow (avoid `/a/b/c/d/e`).
- If you change a URL, add a 301 redirect from the old one, or you lose its ranking and break existing links.

## Schema detection caveat

A raw page fetch or `curl` cannot see structured data injected by JavaScript, and many site builders inject it that way. So "no schema found" from a fetch alone is a false finding. Verify structured data with Google's Rich Results Test (https://search.google.com/test/rich-results), which renders the page, or by inspecting the rendered DOM in a browser.

## Common traps on small camp sites

- A brand-new domain with no content live until spring, so nothing has had time to rank for the January peak.
- The whole site (or the program section) accidentally set to `noindex` after a rebuild.
- Several near-identical town or program pages that get filtered as thin or duplicate content.
- Photos uploaded at full camera resolution, tanking page speed.
- The site moved or rebuilt without redirects, dropping every previously ranking page.
