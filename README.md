# Samuel Chibueze | Engineering Portfolio

A single-page portfolio for a Senior AI and Full-Stack Software Engineer with a focus on system design and architecture. It tells the story of the work: three stints as a founding engineer, payments and booking platforms, production RAG systems and event-driven microservices.

**Live site:** _add your Netlify or Vercel URL here after deploying_

## What's on the page

- **Hero:** positioning, headline metrics and contact links
- **The hats I've worn:** system designer and architect, founding engineer, payments architect, AI engineer, full-stack builder, team lead, researcher
- **Engineering philosophy:** seven principles that guide every system I design
- **The work:** ten projects, each with the problem it solves, the technology used and the value created, plus repo links
- **Toolbox:** languages, architecture, AI, data, infrastructure and observability

## Project structure

```
.
├── index.html   # the entire site: HTML, CSS and content in one file
└── README.md
```

There is no build step, framework or dependency. The only external resource is the Poppins font from Google Fonts, which falls back to the system font if it fails to load.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
# or
python3 -m http.server 8000
```

## Deploy

### Netlify

**Drag and drop:** go to [app.netlify.com/drop](https://app.netlify.com/drop) and drop the folder.

**From GitHub:**
1. Push this repo to GitHub.
2. In Netlify choose **Add new site**, then **Import an existing project**, and pick the repo.
3. Leave **Build command** empty and set **Publish directory** to `.`
4. Click **Deploy**.

### Vercel

1. Push this repo to GitHub.
2. In Vercel choose **Add New**, then **Project**, and import the repo.
3. Set **Framework Preset** to **Other**. Leave the build command and output directory empty.
4. Click **Deploy**.

### GitHub Pages

1. In the repo go to **Settings**, then **Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`.
3. Save. The site goes live at `https://<your-username>.github.io/<repo-name>/`.

## Customise

Everything lives in `index.html`:

| To change | Look for |
| --- | --- |
| Colours and theme | the `:root` block at the top of the `<style>` tag |
| Headline and intro | the `<header class="hero">` section |
| Projects | `<article class="card">` blocks; the `order:N` style controls display order |
| Philosophy | the `<div class="phil">` block |
| Contact details | the `<footer>` and hero buttons |
| Link previews and SEO | the `<meta>` tags in `<head>` |

The page follows the visitor's light or dark mode automatically, and the background animation stops for visitors who prefer reduced motion.

## Before you go live

- Add the SignBridge repo link and the EF4A frontend repo link.
- Confirm the repo links open for visitors. Repos under private organisations will show a 404.
- Replace the placeholder live-site URL at the top of this file.

## Contact

Samuel Chibueze, Lagos, Nigeria
[sechibueze@gmail.com](mailto:sechibueze@gmail.com) · [GitHub](https://github.com/sechibueze) · [LinkedIn](https://linkedin.com/in/sechibueze)
