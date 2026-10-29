# Florida Dental Group of Kendall — production migration candidate

## Verified in this package (source-level)
- 36 HTML pages: 18 English and 18 Spanish.
- Local navigation/assets resolve in the package; each page has title, meta description, canonical, one H1 and English/Spanish hreflang.
- XML sitemap, robots.txt, Vercel redirect configuration included.
- Three Smile Design patient before/after pairs are stored locally at `public/images/result-01/02/03-before/after.jpg`; the owner confirms that they are real and authorized for publication. The Results pages now accurately describe them and do not show demo labels. The image loader never falls back to stock photography for these six clinical result files.
- Homepage testimonial, Smile Design emphasis, Book Now/Reserva Ya, and bilingual email-draft contact workflow are retained.

## Important: still requires LIVE verification before domain migration
1. **Contact form is a temporary mailto draft, not an automatic form submission.** Patients must press Send in their email client. Do not collect medical history or other sensitive health information via ordinary email. Test both languages on mobile and desktop.
2. **Preview indexing:** the canonical tags intentionally point to `https://www.floridadentalgroup.com/`. The Vercel preview remains publicly reachable. After the domain is connected, inspect Search Console for accidental preview indexing and apply an appropriate preview-only noindex rule if necessary (do not noindex the production domain).
3. **Domain/DNS:** connect `www.floridadentalgroup.com` to Vercel, configure apex-to-www and HTTP-to-HTTPS redirects at your DNS/hosting layer, verify certificate and that all redirects are 301/308.
4. **Old site:** redirect map contains 11 confirmed legacy service URLs, not a complete historical crawl. Export all high-value indexed/linked old URLs and map each to the closest new page. Leave obsolete templates 404/410; do not redirect all to the homepage.
5. **Verify real business facts** (hours, address, phone, financing availability, clinical treatments, doctor credentials) and real social profile URLs with the practice. Never claim unverified specialties.
6. **Google:** after launch inspect `robots.txt`, `sitemap.xml`, canonical/hreflang and JSON-LD with URL Inspection and Rich Results Test. Submit sitemap in Search Console; monitor pages, impressions, and call conversions.
7. **Performance/accessibility:** perform real mobile Lighthouse and keyboard testing in the deployed environment. Source-level validation does not prove Core Web Vitals or production HTTP behavior.
8. **Patient imagery:** although the owner confirms permission, retain consent records in the practice's own secure system. Do not include patient identities in site files.
9. **Formspree:** do not use it to transmit patient health information without confirming an appropriate HIPAA arrangement; use a suitable provider or restricted nonclinical inquiry fields.

## Critical test URLs
- `/`, `/index.html`, `/es/`, `/es/index.html`
- `/results.html`, `/es/results.html`
- `/services/smile-design.html`, `/es/services/smile-design.html`
- `/contact.html`, `/es/contact.html`
- `/robots.txt`, `/sitemap.xml`
- Legacy redirects: `/vk2/veneers/`, `/invisalign`, `/emergency`, `/whitening`

**Status:** Production *candidate*, pending domain-level and live interaction checks. Do not describe the migration as completed until these checks pass.
