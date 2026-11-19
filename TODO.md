# Pre-deployment checklist

The site is a static HTML/CSS prototype. Work through the required items below before replacing the current Jimdo site. Keep this checklist current as decisions are made.

## Content and assets

- [x] Add embeds and direct links for the 2025 and 2024 annual reports, Swiss Canoe Forum 2024 presentation, and BPIG presentation 2022 in `berichte/index.html`.
- [x] Confirm public viewing access for the BPIG presentation 2022; its current embed requires viewers to sign in to Google.
- [ ] Review all copied project descriptions and source links with the site owners. Confirm every status and date is still current, especially updates dated 2026.
- [x] Confirm permission to reuse `assets/birs-hero.jpg` and any other images that will be added. Add accurate attribution where required.
- [ ] Proofread all German content, names, email addresses, and links.

## Legal and privacy

- [x] Add the complete postal address and confirm the responsible legal person or organization in `impressum/index.html`.
- [x] Have the site owner review `datenschutz/index.html` against the actual hosting configuration, GitHub Pages processing, and all external links.
- [x] Confirm the contact email addresses are monitored and correct.

## GitHub Pages and domain

- [x] Create or select the GitHub repository and add this site to it.
- [ ] Decide whether the site will use a `github.io` address or a custom domain, and confirm who controls the domain and DNS.
- [x] Enable GitHub Pages for the chosen publishing branch and repository root. Do not add a build system; the committed HTML and CSS are the finished site.
- [ ] If using a custom domain, configure its DNS and GitHub Pages custom-domain setting, then verify HTTPS works.
- [ ] Decide how visitors will move from the Jimdo address to the new site. Configure a redirect if the current domain/provider supports it; otherwise update links and public references.

## Final review and launch

- [ ] Preview the published GitHub Pages site on desktop and mobile.
- [ ] Check every page, navigation link, email link, document link, image, and stylesheet on the published URL. Confirm repository-based paths work if using a project site.
- [ ] Check keyboard navigation, visible focus, image alternative text, page titles, and page descriptions.
- [ ] Confirm the report links and required legal details are present; do not launch with placeholders or unresolved notes.
- [ ] Get approval from the site owner, then announce the new address and retire or redirect the old Jimdo site when ready.
