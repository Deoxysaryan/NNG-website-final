# Legal pages review release | 15 October 2026

New review routes: /legal/, /terms-and-conditions/, /privacy-policy/, /cancellation-refunds/, /disclaimer/.

Public staging: https://deoxysaryan.github.io/NNG_Codex_Build/preview-20261004-r1/legal/

Policies are proposals, with effective date and commercial rules pending NNG approval. Identity was transcribed from the client-supplied GST certificate; its raw PDF is not included. The certificate is not an independent live GST-status check. A grievance officer, commercial rules, data providers and retention schedule must still be confirmed. Arrange qualified Indian legal review before production activation.

The source routes live under public/ as static HTML and share public/legal/policies.css. The typography reuses the existing published landing assets. Build the landing assets alongside these pages, as the existing review build does. Native anchor links intentionally perform full navigation to these static routes.

src/components/layout/Footer.tsx adds accessible policy links after mount, matching the published shared-footer patch. No business content or catalogue media is rebuilt. Add these same links to the landing-page generator footer on the next intentional landing rebuild; the current five published landing footers have been updated in place.

The immutable October 9 published snapshot and its manifests remain untouched. This release is an additive source update, not a claim that the older snapshot equals the later live staging site. All existing media remains remote. No local server, installation or full build is needed for this release.

Regeneration: python3 legal-pages/build_pages.py writes legal-pages/public. Copy generated folders to the project public/ directory before the normal export. The generator is for these policy routes only.

Key sources checked 15 October 2026:
- https://astroarunpandit.org/privacy-policy
- https://astroarunpandit.org/terms/
- https://astroarunpandit.org/refund-policy
- https://adityakundali.com/privacy-policy/
- https://www.adityakundli.com/refund-policy/
- https://www.astrotips.in/download-kundali/terms_and_conditions
- https://www.wipo.int/wipolex/en/text/494931 (SPDI Rules, official text reproduction)
- https://thc.nic.in/Central%20Governmental%20Rules/Consumer%20Protection%20%28E-Commerce%29%20Rules%2C%202020.pdf
- https://www.meity.gov.in/static/uploads/2025/11/c56ceae6c383460ca69577428d36828b.pdf
- https://www.pib.gov.in/newsite/erelcontent.aspx?lang=2&reg=48&relid=294532

Assessment: privacy disclosure and a real complaint process matter; a page titled Legal is a navigation choice. Separate service boundaries and cancellation/order terms suit NNG's mixed consultation/product offer. Do not copy competitor blanket browsing consent, unlimited submission licences, all-sales-final clauses, foreign boilerplate, or unsupported claims of encryption/certification. Current staging has no observed analytics/pixel in inspected entry points; do not infer a site-wide security audit. India DPDP commencement is phased under G.S.R.843(E); do not represent all substantive duties as already commenced. The September 2026 e-commerce amendments are announced for 1 January 2027; reassess before that date.
