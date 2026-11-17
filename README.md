Domain-root crawl entry for the Brand Directory.

The canonical storefront pages remain in [a789b1/brand-directory](https://github.com/a789b1/brand-directory). The root homepage reuses the public directory assets and points to its canonical URL. This repository supplies the host-root robots.txt and canonical URL sitemap.

## Search Console sitemap delivery

The active sitemap is served from this repository through jsDelivr:

https://cdn.jsdelivr.net/gh/a789b1/a789b1.github.io@main/sitemap.xml

On 17 November 2026, Search Console reported **Success / 56 discovered pages** for this sitemap. All 56 entries retain their original `https://a789b1.github.io/brand-directory/` URLs. Only sitemap delivery uses the CDN; the storefronts and their canonical URLs have not moved.

The exact CDN URL-prefix property and the original GitHub Pages property are verified in the same Search Console account. Keep `google7bcc335101fc0fa1.html` in this repository to preserve verification. The root `robots.txt` declares the CDN sitemap, following Google's [cross-site sitemap instructions](https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap#cross-submit).

Check sitemap processing in the [CDN sitemap report](https://search.google.com/search-console/sitemaps?resource_id=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fa789b1%2Fa789b1.github.io%40main%2F). Continue checking search performance and page indexing in the original GitHub Pages property.

When the canonical page inventory changes, regenerate the directory sitemap and update this repository's `sitemap.xml` with the same URL list. Verify the served CDN contents before expecting Search Console to reflect an update; CDN caches can retain an older version temporarily.

The original GitHub-hosted sitemap records were still pending at the time the CDN submission succeeded. The same XML passed schema validation and Google's live fetch test on the original host. This establishes a working alternate delivery path, not a proven underlying cause for Google's original fetch/processing failure. Historical failed submissions are retained for diagnosis.
