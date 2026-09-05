# florianhoffarth.com

Kommunalverwaltung · Führung · Digitalisierung · Kommunikation

This repository contains the personal professional website of Florian Hoffarth.
The site serves as a compact professional evidence layer — a digital appendix to
the CV covering projects, publications and professional background.

**Live site:** <https://florianhoffarth.com>

*TLS certificate provisioning for the custom domain is currently pending.*

## About

The site presents a professional profile in German, structured around:

- work in public administration
- leadership and project coordination
- digital transformation
- selected digital projects
- research and publications
- verifiable references and contact details

## Technical setup

- static HTML and CSS
- no JavaScript
- no build step, no package manager, no dependencies
- system fonts
- local assets only
- no analytics, no tracking, no cookies, no external embeds
- deployed via GitHub Pages

The pages can be opened directly in a browser; no tooling is required.

## Deployment

Deployment runs through GitHub Actions on pushes to `main`. The workflow copies
an explicit allowlist of public site files into the Pages artifact, so repository
documentation is not part of the published web root.

## Project structure

```text
index.html                  Professional profile
impressum.html              Legal notice
datenschutz.html            Privacy notice
styles.css                  Shared layout and responsive rules
assets/portrait.png         Local portrait image
.github/workflows/pages.yml GitHub Pages deployment
```

## Privacy

- no analytics
- no cookies
- no tracking
- no external embeds
- local assets only

Full details are published in the [privacy notice](https://florianhoffarth.com/datenschutz.html).
