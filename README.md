# Beldium Consultancy - complete website source

Website: https://consultancy.beldium.com/
Source snapshot: 30 October 2026

## What is included
All 14 website pages, shared CSS and JavaScript, logo, original SVG artwork, institutional review PDF, sitemap, robots.txt and original Sites hosting manifest.

This is the actual editable HTML/CSS/JavaScript source used by the website. It is a static website, not a React/Vite Lovable project. No compilation or npm dependencies are required.

## Run locally
From this extracted directory, run:

    python3 -m http.server 8000 --directory dist

Then open http://localhost:8000/ in a browser. Use a web server rather than double-clicking index.html because asset and navigation paths start at the site root.

## Edit
- dist/index.html: homepage
- dist/style.css: shared styling
- dist/app.js: navigation, audience selector and enquiry handling
- dist/expertise/: five service pages
- dist/about/, dist/approach/, dist/contact/: institutional pages
- dist/perspectives/: editorial index and three articles
- dist/resources/: downloadable review pack page
- dist/assets/: logo and SVG artwork
- dist/documents/: public institutional review PDF

Pages contain their own header/footer markup. Apply shared navigation or footer edits across all HTML files.

## Deploy elsewhere
Upload the CONTENTS of dist/ to the web host document root. The host must serve directory index.html files for nested routes. The .openai/hosting.json file is the original Sites hosting configuration; it is not needed by other static hosts. Do not reuse its project ID to publish an unrelated Site.

If changing domain, update canonical and Open Graph metadata where applicable, sitemap.xml and robots.txt. DNS and TLS configuration belong to the hosting provider and are not included as credentials.

## Behaviour and external resources
The enquiry form opens the visitor's email application to partnerships@beldium.com. It does not submit to a backend or store records. Google Fonts are loaded externally; navigation and footer links also reference beldium.com.

## Security
No Git history, access tokens, passwords or environment secrets are included.
# consultancy
