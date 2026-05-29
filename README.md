# adrienbeton.vercel.app

Source of my personal site & product lab — a static one-pager presenting who I am
and a few of my convictions. Zero framework, self-hosted fonts, GSAP animations,
deployed on Vercel.

**Live:** [adrienbeton.vercel.app](https://adrienbeton.vercel.app)
**About me:** [github.com/adrienbeton](https://github.com/adrienbeton) · [LinkedIn](https://linkedin.com/in/abeton)

## Stack

Vanilla HTML / CSS / JS · [GSAP](https://gsap.com) for scroll animations · WebP assets ·
self-hosted variable fonts. No build step, no dependencies — a single `index.html`
served as-is.

## Structure

```
index.html        markup, styles and scripts in one file
assets/           portraits, project shots (WebP), fonts
vercel.json       output config
```

## Run locally

Any static server works:

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```
