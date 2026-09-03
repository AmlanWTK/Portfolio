# Amlan Sarkar — Portfolio

**Live site: https://amlanwtk.github.io/Portfolio/**

A single-page personal portfolio built as one self-contained `index.html` — no build step, no framework, no dependencies. Hand-written HTML, CSS and JavaScript, deployed straight to GitHub Pages.

## Highlights

- **Zero dependencies.** ~23 KB of hand-written CSS and ~6 KB of vanilla JS inlined into a single file. Nothing to install, nothing to build.
- **Scroll-reveal animations** driven by `IntersectionObserver` rather than an animation library.
- **Glassmorphic UI** using `backdrop-filter`, CSS grid layouts and a custom cursor.
- **Fully responsive** from mobile to desktop via CSS `@media` breakpoints.
- **Working contact form** wired to Formspree — no backend required.
- **Downloadable CV** served directly from the repo.

## Sections

| Section | Contents |
|---|---|
| Hero | Intro, primary CTAs, CV download |
| About | Background, education, stats |
| Skills | Languages, frameworks, mobile, databases, tools |
| Projects | MedDA Old2Modern, Mental Health AI, Civic Infrastructure Monitoring, Personal Finance Tracker, Kid-Safe Search |
| Contact | Formspree form, GitHub, LinkedIn, email |

## Structure

```
index.html                              # entire site: markup, styles, scripts
photo.jpg                               # profile image
Amlan_Sarkar_Full_Stack_Developer.pdf   # downloadable CV
```

## Running locally

```bash
git clone https://github.com/AmlanWTK/Portfolio.git
cd Portfolio
python3 -m http.server 8000
```

Then open http://localhost:8000. Opening `index.html` directly in a browser also works.

## Deployment

GitHub Pages serves the `main` branch from the repository root. Any push to `main` redeploys the live site.

## Updating

- **Content and styling** — edit `index.html`; styles live in the `<style>` block, behaviour in the `<script>` block at the bottom.
- **CV** — replace the PDF, keeping the filename so the download link stays valid.
- **Contact form** — the Formspree endpoint is set on the form's `action` attribute.
