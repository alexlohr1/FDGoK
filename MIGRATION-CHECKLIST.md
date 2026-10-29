# Florida Dental Group of Kendall — SEO Migration Checklist

## Completed in this package
- Unique English and Spanish page titles/descriptions; canonical URLs for production domain.
- English/Spanish hreflang on matching core pages.
- Dentist structured data on homepage, sitemap.xml and robots.txt.
- Selected relevant old service URL redirects in vercel.json.
- Prominent mobile click-to-call link and homepage phone action.
- Improved homepage heading and corrected awkward copy.

## CRITICAL: must complete before going live
1. Appointment/contact forms are FRONT-END DEMOS and do not send inquiries. Connect a HIPAA-appropriate scheduling/communication workflow and verify end-to-end delivery. Do not send protected health information to ad pixels or analytics.
2. Verify hours, dentist names and licenses, insurance plans, financing terms, phone, address, treatment claims, photos, and consent for testimonials.
3. Replace placeholder photographs with owned/licensed real clinic photos.
4. Confirm the domain will be **www.floridadentalgroup.com**; if using the non-www hostname instead, update all canonical/hreflang/schema/sitemap URLs. Redirect alternate hostname to canonical.
5. Check all legacy indexed pages and backlink targets against a full URL inventory; the redirects included here cover only URLs shown in screenshots, not a full migration map. Avoid redirecting unrelated pages to the homepage.
6. Ensure preview domain is not indexed after production deployment; do not accidentally block the production domain.
7. Add GA4 and Google Ads conversions with compliant tracking; test click-to-call and completed appointment requests separately.
8. Confirm redirects, status codes, sitemap, canonicals, hreflang, structured data and internal links on production after deployment.
9. Submit sitemap in Google Search Console and monitor indexed pages and non-branded clicks weekly.
10. Review page content for medical accuracy, originality, clinician attribution and substantive patient FAQs. Technical SEO alone cannot guarantee rankings.

## Important notes
- `/robots.txt` appearing as crawled-not-indexed is not a concern; robots.txt is not a search landing page.
- The three old hostname/HTTP redirects are expected when they point to the preferred canonical hostname.
- Obsolete template tag and event pages may correctly remain 404/410.
- Vercel configuration assumes a static deployment with files at project root. Test Vercel routing before launch.
