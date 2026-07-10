# seo-birmingham.uk — repo brain

Astro 5 + Tailwind static site for seo-birmingham.uk. Deploys via Cloudflare Pages on git push (build `npm run build`, output `dist`).

## Brain

- 2026-07-10: Integrity fix. Deleted the fabricated case studies section entirely — `src/pages/case-studies/` (index + "Colmore Law Firm" + "Jewellery Quarter Retailer" pages), which carried invented stats (340% traffic, 210% leads, fake Review schema/reviewBody quotes from anonymised "clients") despite an "illustrative, composite" disclaimer. Removed all nav/footer links to `/case-studies/` in `src/layouts/Base.astro`, the CTA button on the homepage, the related-links entry on the AI search optimisation page, the case-studies mention in the pricing FAQ footer text, the fabricated-results FAQ item on `/about/` that referenced the deleted page as containing "real ranking improvements... revenue impact", and the 3 case-study lines in `public/llms.txt`. No title/meta/heading/body-copy rewrites — pure removal + link wiring fix. Build passes, sitemap regenerates clean (no case-studies URLs). Pushed to origin/master.
