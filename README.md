# taransingh.dev

Personal portfolio website for Taran Pal Singh — Computer Science student at the University of Southampton. The site presents experience, projects, awards, and skills, with a downloadable CV and links to contact channels.

## Key features

- Single-page layout with sections for Experience, Projects, Awards, Skills, and a "Playground" section
- Project index with hover/focus-to-expand cards linking out to live projects (e.g. Hive, Claros)
- Downloadable CV (`Taran_Singh_CV.pdf`) and mailto/LinkedIn/GitHub contact links
- Custom canvas-based mini game ("Colour Rush") built without a game engine, with local high-score persistence via `localStorage`
- Spotify iFrame API integration for an embedded playlist player with custom transport controls
- Scroll-triggered reveal animations via `IntersectionObserver`
- Live clock and cursor particle-trail effects, both respecting `prefers-reduced-motion`

## Tech stack

- Plain HTML, CSS, and vanilla JavaScript — no framework, no build step, no dependencies
- Google Fonts (Anton, Inter, Space Mono) loaded via CDN link tags
- Spotify iFrame API (`https://open.spotify.com/embed/iframe-api/v1`) loaded via script tag
- Native browser APIs: Canvas 2D, `IntersectionObserver`, `localStorage`

## Project structure

```
.
├── index.html          # entire site: markup, embedded <style>, and embedded <script>
└── Taran_Singh_CV.pdf   # downloadable CV, linked from the page
```

## Setup / installation

No installation or dependencies are required — there is no `package.json` or build tooling in this repo.

## Usage / running locally

Open `index.html` directly in a browser, or serve the directory with any static file server, for example:

```
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deployment

This repository is named `36taransingh5-dotcom.github.io`, so it is deployed automatically via GitHub Pages: any push to the default branch (`main`) publishes `index.html` at `https://36taransingh5-dotcom.github.io`. No build step runs before publishing — the checked-in `index.html` is served as-is.
