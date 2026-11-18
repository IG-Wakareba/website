# Editing guidance for coding agents

This repository is the plain HTML source for the IG WaKaReBa website. The intended workflow is: edit source files, inspect the pages in a browser, then commit to GitHub Pages.

## Constraints

- Keep the site static: no JavaScript, npm, CMS, framework, site generator, build pipeline, or third-party runtime.
- Edit the existing HTML and shared `assets/styles.css` directly. Do not generate or minify source.
- Preserve the German copy, Swiss spelling, page URLs, keyboard access, mobile layout, and accessible heading order.
- Use only relative links for local pages and assets so the site also works under a GitHub Pages repository path.
- Do not invent project facts, dates, document URLs, legal identities, postal addresses, or image descriptions. Keep questions for the site owner explicit.
- Project updates belong in separate `<article class="project">` blocks in `projekte/index.html`, with their source links and a visible status date.
- Keep all repeated navigation and footer links in sync across pages.

## Repository map

- `index.html`: organization overview and homepage.
- `projekte/index.html`: project history and updates.
- `berichte/index.html`: annual reports and presentations; document URLs still need confirmation.
- `ueber-uns/index.html`: founding story and organizational role.
- `impressum/index.html` and `datenschutz/index.html`: legal information that must be checked before launch.
- `assets/styles.css`: site-wide visual styles.
- `assets/birs-hero.jpg`: homepage photograph.

When asked to make a change, update only the relevant page and shared styles if needed. Check internal links, image paths, and HTML validity for every edited page. Do not mark the site launch-ready while the report links and legal details noted in `README.md` remain unresolved.
