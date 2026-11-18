# IG WaKaReBa website

This is a small, static HTML website for the IG WaKaReBa, a working group of the Basler Paddelsport IG. It is intentionally built without a framework, generator, JavaScript, npm, or a CMS. The HTML files are the source and the finished website.

## Edit and publish

1. Edit the relevant `.html` file in a text editor. Project entries are separate `<article class="project">` sections in `projekte/index.html`.
2. Put new images in `assets/` and refer to them with a relative path. The current homepage photo is `assets/birs-hero.jpg`.
3. Open `index.html` in a browser and follow the page links to review the change. No build step is needed.
4. Commit and push the files to the GitHub repository's publishing branch.
5. In GitHub, set **Settings → Pages → Build and deployment → Deploy from a branch**, select the publishing branch and `/ (root)`.

The site uses relative internal links so it works both at a custom domain and in a repository-based GitHub Pages preview. Keep page folders and their `index.html` names so existing paths such as `/projekte/` and `/ueber-uns/` remain stable.

## Page map

- `index.html` — purpose, approach, and contact email.
- `projekte/index.html` — project updates and their original source links.
- `berichte/index.html` — annual reports and presentations. The previous Jimdo page embedded Google Docs, but its direct document URLs were not available during this first migration pass. Replace the short notes with local PDF links or confirmed public document links.
- `ueber-uns/index.html` — founding story and relationship to the Basler Paddelsport IG.
- `impressum/index.html` — contact details. Add the correct legal entity and postal address before the site replaces the current site.
- `datenschutz/index.html` — intended behavior for this static site. Review it before publication against the actual hosting and external links; it deliberately does not repeat the old Jimdo/Google Analytics policy.
- `assets/styles.css` — shared layout, colors, and responsive styling.
- `assets/birs-hero.jpg` — local copy of the homepage image.

## Editing conventions

- The site language is German (`lang="de"`); preserve Swiss spelling such as “ss” rather than “ß”.
- Use one clear `<h1>` per page and descriptive headings for sections.
- Keep each project as a self-contained article. Put its newest update near the top, and retain its status date so readers can tell when information was current.
- Keep supporting links next to the claim or update they support. Use descriptive link text rather than “click here”.
- Use relative links for pages and local assets. External links should use their full `https://` URL.
- Add meaningful alternative text to informative images. Use `alt=""` only for decorative images.
- Keep navigation and footer links consistent across all page files. The menu is intentionally repeated in the HTML so every page works without scripts or server-side includes.
- Do not add analytics, cookies, external embeds, scripts, frameworks, package managers, or generated files without discussing the change first.

The copied project text reflects the public site as inspected on 18 November 2026. Verify dates and current project status before publishing; the old page contains several dated updates.
