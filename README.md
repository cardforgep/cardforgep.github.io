# CardForge Frontend v8.12.3 — SEO / crawler policy

Frontend-only update on top of v8.12.2. Backend v8.12.2 and Dashboard v1.5.4 remain compatible and unchanged.

## Added
- `robots.txt`: allows Google/Bing indexing and OAI Search, blocks selected training-oriented AI crawlers.
- `sitemap.xml` for Google Search Console.
- canonical URL, robots directives, Open Graph/Twitter metadata.
- Schema.org `WebSite`, `SoftwareApplication`, and `FAQPage` JSON-LD.
- visible SEO section for marketplace/product-card queries.
- marketplace FAQ item.
- SEO-focused title/description for RU/EN/DE UI states.

## Deploy
Upload all files from this archive to the root of the `cardforgep.github.io` GitHub Pages repository. Keep `.nojekyll`. No VPS/backend/dashboard update is required.

After deployment check:
- https://cardforgep.github.io/robots.txt
- https://cardforgep.github.io/sitemap.xml
- https://cardforgep.github.io/

Then add the site to Google Search Console and submit `https://cardforgep.github.io/sitemap.xml`.

Note: robots.txt is a voluntary crawler protocol, not an access-control/security boundary. Scrapers that ignore it cannot be reliably blocked on GitHub Pages alone.
