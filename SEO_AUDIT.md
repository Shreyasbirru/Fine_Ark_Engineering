# Fine Ark Engineering SEO Audit

Audit date: 2026-11-09  
Scope: Static HTML site in the repository; source-level audit (no live production URL supplied).

## Project and Scope

The website is a static, root-level HTML5 site using Bootstrap, site CSS, jQuery, and JavaScript plugins (including Swiper). There is no framework router or build configuration in the repository. The 11 business pages below are indexable candidates. The unrelated GSAP `demo.html` has been removed; six HTML documents under `assets/css/images/` are 404 vendor artifacts already marked `noindex`.

The Git remote identifies a source repository, not a confirmed public website origin. No production domain is present in project configuration. Canonical URLs, `og:url`, absolute social image URLs, and an absolute-URL XML sitemap therefore cannot be emitted safely until the owner confirms the live HTTPS hostname and preferred www/non-www form.

## Page-by-Page Audit

| Page URL                       | Existing title                               | Proposed title                                         | Proposed meta description                                                                                                                                        | Existing H1                                                             | Primary keyword                            | SEO issues found before implementation                                                                                                                                                          |
| ------------------------------ | -------------------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- | ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `/index.html`                  | (empty)                                      | Industrial Engineering & Plant Installation - Fine Ark | Fine Ark Engineering provides industrial fabrication, AAC plant equipment, machinery installation, structural work and piping in Ahmednagar, Maharashtra.        | 8 rotating-slide H1s; first: Precision Fabrication For Heavy Industries | industrial engineering services            | Empty title and description; eight H1s in slider; no canonical, social metadata, or schema.                                                                                                     |
| `/about.html`                  | About Us                                     | Fine Ark Engineering - Industrial Engineering Company  | Learn about Fine Ark Engineering, an industrial engineering company based in Ahmednagar, Maharashtra. Explore our company profile, leadership and capabilities.  | About Us                                                                | Fine Ark Engineering                       | Empty description; generic image ALT text; no canonical, social metadata, or schema.                                                                                                            |
| `/products.html`               | Products                                     | AAC, Chemical & Sugar Plant Equipment - Fine Ark       | Explore Fine Ark Engineering products for AAC, pharmaceutical and chemical, and sugar plants, including autoclaves, reactors, heat exchangers and tanks.         | Products                                                                | AAC plant equipment                        | Empty description; product links target missing `portfolio-details.html`; no canonical, social metadata, or schema.                                                                             |
| `/services.html`               | Services                                     | Industrial Plant Installation Services - Fine Ark      | Explore Fine Ark Engineering services: AAC machinery installation, machinery removal, structural fabrication, piping and industrial insulation.                  | Services                                                                | industrial plant installation services     | Empty description; service-card images use generic ALT text; no canonical, social metadata, or schema.                                                                                          |
| `/gallery.html`                | Gallery                                      | Industrial Engineering Project Gallery - Fine Ark      | View Fine Ark Engineering's gallery of industrial engineering work and product demonstration videos. Contact our team to discuss your project.                   | Gallery                                                                 | industrial engineering projects            | Empty description; script-generated images use generic numbered ALT text; no canonical, social metadata, or schema. The generated gallery range (2 to 28) has matching image files.             |
| `/contact.html`                | Contact Us                                   | Contact Fine Ark Engineering - Ahmednagar, India       | Contact Fine Ark Engineering in Ahmednagar, Maharashtra for enquiries about AAC plant equipment, machinery installation, fabrication and piping services.        | Contact Us                                                              | industrial engineering services Ahmednagar | Empty description; address links use `#`; no canonical, social metadata, or schema. Contact details should be reconciled before using phone data in schema (different numbers appear on pages). |
| `/aac-installation.html`       | AAC Machine Installation                     | AAC Plant Installation Services in India - Fine Ark    | Fine Ark Engineering provides AAC machinery and plant installation, including autoclaves, moulds, structural fabrication and piping. Enquire today.              | AAC Machine Installation                                                | AAC plant installation                     | Empty description; generic service-image ALT; H1 followed by H3-level section headings; no canonical, social metadata, or schema.                                                               |
| `/machinery-installation.html` | Machinery / Equipment Installation & Removal | Industrial Machinery Installation & Removal - Fine Ark | Fine Ark Engineering offers industrial machinery installation and removal. Contact us to discuss your equipment requirements.                                    | Machinery / Equipment Installation & Removal                            | industrial machinery installation          | Empty description; generic service-image and gallery ALT text; H1 followed by H3-level section headings; no canonical, social metadata, or schema.                                              |
| `/structural-work.html`        | Structural Work                              | Industrial Structural Fabrication Work - Fine Ark      | Fine Ark Engineering offers industrial structural work, including structural fabrication and erection services. Contact us to discuss your project requirements. | Structural Work                                                         | structural fabrication work                | Empty description; generic service-image and gallery ALT text; H1 followed by H3-level section headings; no canonical, social metadata, or schema.                                              |
| `/piping-work.html`            | Piping Work                                  | Industrial Piping Installation Work - Fine Ark         | Explore industrial piping work from Fine Ark Engineering, including piping installation and maintenance. Contact us to discuss your plant requirements.          | Piping Work                                                             | industrial piping work                     | Empty description; generic service-image and gallery ALT text; H1 followed by H3-level section headings; no canonical, social metadata, or schema.                                              |
| `/insulation-work.html`        | Insulation Work                              | Industrial Insulation Work - Fine Ark                  | Explore industrial insulation work from Fine Ark Engineering for plant and equipment applications. Contact us to discuss your project requirements.              | Insulation Work                                                         | industrial insulation work                 | Empty description; generic service-image ALT; H1 followed by H3-level section headings; no canonical, social metadata, or schema.                                                               |

## Implementation Results

- Audited and optimized all 11 indexable business pages. The separate GSAP `demo.html` was removed as requested; six bundled vendor 404 documents remain marked `noindex` and are not listed as business pages.
- Added unique titles and descriptions to all 11 pages, plus Open Graph title/description/type/site name/locale and Twitter summary-card metadata. Descriptions are 125-160 characters. Search-volume and ranking claims were not made.
- Corrected the homepage slider to one H1 and seven H2 elements. Service detail pages now use one H1 followed by four H2 section headings, retaining the existing heading CSS class and visible copy.
- Added Organization JSON-LD to each page with the company name, email and address available in the website. Added WebSite and WebPage schema to the homepage, AboutPage, CollectionPage, ContactPage, and Service entities where appropriate. No LocalBusiness, product-specific Product schema, phone number, social profiles, or unverified claims were added.
- Added accurate image alternatives for service, gallery, founder, facility and partner-logo images. Added verified dimensions, lazy loading and async decoding for below-fold content images, and high-priority preload for the first hero image. Source image paths and formats were retained.
- Added a permissive `robots.txt`. Removed 442 active `href="#"` placeholders and all source occurrences of those dead placeholder links; removed the 77 `portfolio-details.html` references that targeted a missing page. A post-change local-reference scan found no active missing local targets.
- Canonical URLs, `og:url`, absolute social image URLs, and `sitemap.xml` remain unimplemented because no production HTTPS hostname or preferred host was found in the repository. Do not publish placeholder or guessed URLs.
- There is no package manifest or production build command. Live redirects, HTTP status, rendered routes, Google Rich Results results, and Core Web Vitals require a deployed site and were not measurable from this repository.

Proposed text is based on the content and service names already present in the site, not external keyword-volume or ranking claims. Descriptions may be adjusted for actual search snippets after the production domain and owner-approved wording are confirmed.

## Pre-Implementation Findings

The following items describe the audit baseline before the changes summarized above.

- All 11 business pages have an empty meta description. The homepage title is empty; the other business page titles are distinct.
- The homepage slider contains eight H1 elements. Other business pages have one H1 each. Service-detail sections jump from H1 to H3 in the main content.
- No canonical links, Open Graph/Twitter metadata, or JSON-LD structured data are present on business pages.
- No `robots.txt` or `sitemap.xml` exists. The site has no declared preferred host, HTTPS enforcement, or slash policy in the checked source.
- Confirmed dead internal destination: product cards link to `portfolio-details.html`, which is not present. Product-detail content is also not available to author without verified product facts. `contact-two.html` references are in commented-out markup and are not active links.
- Contact page shows an Ahmednagar, Maharashtra address and email; phone numbers differ between the contact and other pages. Do not select one for Organization schema until confirmed.
- Several content images use placeholder ALT values such as `image` or generic numbered gallery descriptions. CSS background images (including hero and product-card backgrounds) do not have ALT text by design; adjacent HTML text should carry their meaning.
- Gallery JavaScript creates 27 visible thumbnails and links to corresponding originals; source image paths exist. HTML source-only checks cannot establish HTTP status, rendered behavior, or Core Web Vitals.
- The site has no package manifest or production build command. Local link checks must account for JavaScript-generated paths and commented-out markup.

## Keyword-to-Page Mapping

| Page                   | Target theme                                            |
| ---------------------- | ------------------------------------------------------- |
| Home                   | Industrial engineering and fabrication services         |
| About                  | Fine Ark Engineering company profile                    |
| Products               | AAC, pharmaceutical/chemical, and sugar plant equipment |
| Services               | Industrial plant and equipment installation services    |
| AAC installation       | AAC plant and machinery installation                    |
| Machinery installation | Industrial machinery installation and removal           |
| Structural work        | Industrial structural fabrication and erection          |
| Piping work            | Industrial piping work and installation                 |
| Insulation work        | Industrial insulation work                              |
| Gallery                | Industrial engineering project gallery                  |
| Contact                | Fine Ark Engineering contact in Ahmednagar, Maharashtra |

Search volume, competition, and current rankings were not available in the repository and have not been asserted. Pharma/chemical equipment and sugar plant equipment remain product-category themes, not separate landing pages, because no dedicated pages exist.

## Owner Inputs Needed for Final Technical SEO

1. Confirm the production HTTPS hostname and canonical host preference (www or non-www). This is required for correct canonical links, sitemap URLs, `og:url`, and absolute social image URLs.
2. Reconcile the phone number shown on the contact page with the number in shared page chrome before adding it to structured data.
3. Supply verified product-specific details if individual product pages are expected; do not generate specifications from the current product names alone.
4. Provide approved social profile URLs if they should appear in schema or social metadata.

## Validation Boundary

This audit is a source review. No live crawl, server response/redirect testing, Search Console data, Analytics data, Lighthouse/Web Vitals run, or production build can be claimed from the repository alone. After changes, validate the static HTML metadata, local assets and links; live host behavior remains a deployment-side check.
