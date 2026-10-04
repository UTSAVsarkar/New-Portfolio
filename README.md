# Utsav Sarkar | Portfolio

Personal portfolio of Utsav Sarkar, Data Scientist working on AI governance platforms, LLM agents and explainable ML.

A single-file static website: plain HTML, CSS and vanilla JavaScript. No framework, no build step, no dependencies to install.

## Sections

- **Hero:** intro, role, live agent-monitor demo panel
- **About:** background, quick facts, education
- **Impact numbers:** 14+ Delta tables, 50+ endpoints, 1.8M users analysed, 10 Kaggle medals
- **Work experience:** Infocepts, Havells, MAQ Software, each point followed by its own looping animation
- **Toolbox:** skills grouped by category
- **Projects:** Vehicle Complaint Intelligence System and a second end-to-end build, each with an animated demo
- **Contact:** email, phone, LinkedIn

## Features

- **Per-point work demos:** every work-experience bullet has a small animation under it that loops while it is on screen and pauses when it is not
- **Source peek:** hovering a card reveals a faint patch of that card's own HTML around the cursor (mouse devices only)
- **Light and dark theme:** follows the device setting
- **Responsive:** single-column layout on phones
- **Accessible motion:** animations are skipped for visitors with "reduce motion" turned on
- **Email fallback:** if no mail app opens from a "Say hello" button, the email is copied and an "Open Gmail" link appears
- **Share metadata:** page description, social preview tags and a favicon

## Run locally

Open `myPortfolio.html` in any modern browser. That's it.

For a local server instead:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000/myPortfolio.html
```

## Deploy

Rename `myPortfolio.html` to `index.html` so hosts serve it at the root URL.

**GitHub Pages**
1. Push `index.html` and this README to a GitHub repository.
2. Go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then save.
4. Your site appears at `https://<username>.github.io/<repo>/` after a minute or two.

**Netlify**
1. Go to Netlify and choose **Add new site > Deploy manually**.
2. Drag the folder containing `index.html` onto the page.

## Customize

Everything lives in `myPortfolio.html`.

| To change | Look for |
| --- | --- |
| Colours and theme | the `:root` block at the top of the `<style>` section (`--a`, `--b`, `--c`, `--bg`, ...) |
| Name, role and intro | the `<header class="hero">` block |
| Work experience text | `<section id="work">` and the `.job` cards |
| Work experience animations | the `mk(J[0], [...])`, `mk(J[1], ...)` and `mk(J[2], ...)` calls near the end of the script |
| Tech tags under each job | the `<div class="jt">` rows |
| Skills | the skills data used by the `#tabs` and `#chips` script |
| Contact details | `<section class="contact" id="contact">` and the `mailto:` links in the hero |
| Share title and description | the `<meta>` tags in `<head>` |
| Animation speed | the `sl` helper (the `ms * .55` factor); lower is faster |

## Tech

- HTML5, CSS3 (custom properties, grid, flexbox, CSS masks)
- Vanilla JavaScript (IntersectionObserver, Web Animations API)
- Fonts: Bricolage Grotesque and DM Sans from Google Fonts (needs an internet connection to load; falls back to system fonts offline)

## Notes

- The numbers and names inside the animated demos are illustrative and are marked that way on the page.
- To add a share image for link previews, host an image and add `<meta property="og:image" content="https://...">` to `<head>`.

## Contact

Utsav Sarkar
Email: utsavsarkar2000@gmail.com
LinkedIn: https://www.linkedin.com/in/utsav-sarkar-49892325a/
