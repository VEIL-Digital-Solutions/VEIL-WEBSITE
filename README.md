# VEIL Digital Solutions website

The site is a static HTML, CSS and JavaScript website hosted on GitHub Pages. It does not need a paid hosting plan or a custom domain to run.

## Updating the website

1. Open the [VEIL-WEBSITE repository](https://github.com/VEIL-Digital-Solutions/VEIL-WEBSITE) and sign in to an account with permission to edit it.
2. Open `index.html` and choose the pencil icon to edit text, links, services or contact details. Keep the HTML tags around the text in place.
3. Use **Commit changes** to save. GitHub Pages will publish the update after its deployment finishes.

The supplied VEIL brand artwork is used in the header, footer and homepage hero as `assets/veil-brand.png`. The browser tab icon uses `assets/veil-logo.svg`. Keep both files in place when updating the brand.

To change the share-preview artwork, replace `assets/veil-social-card.svg` and keep its filename. Check the email address and contact information in `index.html` before publishing changes to them.

## Public website scope

The experimental concept gallery and demo pages are excluded from the public release. The live site presents VEIL's services rather than fictional client concepts.

The demo "Add sample item" interaction is local to the browser. It does not submit an order or process payment. The request/customisation links open a pre-filled email to VEIL.

## Project enquiries and administration

The public website is static. Do not add a form that appears to submit customer enquiries unless it is connected to a real backend. A secure Cloudflare Functions + D1 endpoint needs Cloudflare Pages deployment, database bindings and account-side configuration. Never put API keys, passwords or private credentials in HTML, JavaScript or this repository.

There is no administration dashboard yet. Website content is currently updated by editing repository files; a real dashboard requires authenticated storage and server-side access controls.

## Google Search setup

Google Search Console helps verify the site, submit its sitemap and monitor search indexing. It does not edit the website.

1. Open [Google Search Console](https://search.google.com/search-console/) and add a **URL prefix** property for `https://veil-digital-solutions.github.io/VEIL-WEBSITE/`.
2. Choose HTML file verification. Upload the verification file Google provides to the repository root (beside `index.html`) and commit it.
3. After GitHub Pages publishes the file, return to Search Console and select **Verify**.
4. In Search Console, submit `https://veil-digital-solutions.github.io/VEIL-WEBSITE/sitemap.xml`.

The sitemap and `robots.txt` are already included. Google decides when and whether to index pages; verification and a sitemap do not guarantee a particular search position or immediate appearance. Keep the canonical URL in `index.html`, `robots.txt` and `sitemap.xml` in sync if the site address changes.
