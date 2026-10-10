# MAGCOOLEST — project website

Public website of the MAGCOOLEST coordinated project (MICIU/AEI, PID2025-174502NB-C31, C32 and C33).
Plain HTML and CSS, no build step, served by GitHub Pages.

## How to edit

Every page is a self-contained `.html` file. Open it, change the text between the tags, commit.
There is no compilation: what you commit is what gets served, usually within a minute.

- `index.html` — home page (English). `ES/index.html` — home page (Spanish).
- `research.html`, `team.html`, `news.html`, `publications.html`, `open-science.html`, `contact.html`
- `css/style.css` — the only stylesheet. Colours are defined once at the top, under `:root`.
- `img/` — logos and figures. `assets/` — reports, press releases and outreach material.

### Adding a news entry

Copy an existing `<article class="entry">` block in `news.html`, put it at the top of the
section, and change the date, title and text. Keep the `datetime` attribute in ISO format
(`2027-03-14`). Mirror the two most recent entries on the home page.

### Adding a publication

Copy a list item in `publications.html`. Include the DOI, a link to the open-access version
and, when there is one, a link to the dataset in Zenodo.

## Before going live

- [ ] Add the official MICIU/AEI and European Union logos to `img/` as
      `logo-micinn-aei.svg` and `logo-ue.svg`. Download them from the funder's own site so
      the versions are the current ones.
- [ ] Set the custom domain in Settings → Pages. GitHub writes the `CNAME` file itself.
- [ ] Replace the placeholder link to the Zenodo community in `open-science.html`.
- [ ] Check the team page with each group: names, roles and affiliations must be confirmed
      by the people listed.

## Licence

Content (text, figures, outreach material): CC BY 4.0.
Code (templates, stylesheet): MIT.
