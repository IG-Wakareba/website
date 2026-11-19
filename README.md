# IG Wakareba website

This is a small, static HTML website for the IG Wakareba, a working group of the Basler Paddelsport IG. It is intentionally built without a framework, generator, JavaScript, npm, or a CMS. The HTML files are the source and the finished website.

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
- `berichte/index.html` — annual reports and presentations. The annual reports for 2025 and 2024, the Swiss Canoe Forum 2024 presentation, and the BPIG 2022 presentation are embedded from their confirmed Google Drive/Slides URLs.
- `ueber-uns/index.html` — founding story, BPIG affiliation, supporting organizations, and their logos.
- `impressum/index.html` — contact details. Add the correct legal entity and postal address before the site replaces the current site.
- `datenschutz/index.html` — short privacy notice covering GitHub Pages, the absence of Google Analytics and first-party trackers, and the Google document embeds.
- `assets/styles.css` — shared layout, colors, and responsive styling.
- `assets/birs-hero.jpg` — homepage hero photo.
- `assets/bpig-artwork.jpg` and `assets/logo-*.png`/`assets/logo-*.jpg` — affiliation and partner logos on `ueber-uns/index.html`.
- `assets/birs-st-jakob.jpg`, `assets/birs-forellenweg.jpg`, `assets/simmental.jpg`, and `assets/birs-redingbruecke.jpg` — photos and captions from the original homepage.
- `assets/kraftwerk-birsfelden-kursverbot.jpg`, `assets/wiese-unterlauf.jpg`, `assets/fischereigesetz-bl.jpg`, `assets/surfwellen-reding-joggeli.jpg`, `assets/fischpass-birsfelden.jpg`, `assets/schaenzli.jpg`, `assets/betretungsverbot-birsfelden.jpg`, `assets/moossee-grellingen.jpg`, `assets/wiese-vital.jpg`, `assets/solitude-promenade.jpg`, and `assets/reinacher-heide.jpg` — photos used in matching project entries.

## Editing conventions

- The site language is German (`lang="de"`); preserve Swiss spelling such as “ss” rather than “ß”.
- Use one clear `<h1>` per page and descriptive headings for sections.
- Keep each project as a self-contained article. Put its newest update near the top, and retain its status date so readers can tell when information was current.
- Keep supporting links next to the claim or update they support. Use descriptive link text rather than “click here”.
- Use relative links for pages and local assets. External links should use their full `https://` URL.
- Add meaningful alternative text to informative images. Use `alt=""` only for decorative images.
- Homepage photos are local files in `assets/` and are shown in captioned `<figure>` elements. Keep informative alt text, image dimensions, lazy loading for below-the-fold photos, and the original photo captions when changing them. The hero uses `object-fit: cover` with responsive `object-position` values in `assets/styles.css`; adjust those values to keep its subject visible. If one image cannot compose well at both wide and tall aspect ratios, use a separate mobile crop and a `<picture>` element with a media-specific `<source>` rather than forcing one crop everywhere.
- Project photos use `<figure class="project-image">` elements in `projekte/index.html`; use `project-image--portrait` for portrait-oriented files. Each project article lets text flow beside and below the image on desktop, then stacks in source order on mobile. Images keep their aspect ratio rather than being cropped. Clicking a photo opens a native HTML popover with a close button; keep its trigger and popover IDs matched and do not add JavaScript.
- Keep navigation and footer links consistent across all page files. The menu is intentionally repeated in the HTML so every page works without scripts or server-side includes.
- Do not add analytics, cookies, external embeds, scripts, frameworks, package managers, or generated files without discussing the change first.

The copied project text reflects the public site as inspected on 18 November 2026. Verify dates and current project status before publishing; the old page contains several dated updates.
