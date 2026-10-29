# Denzi — Wellness × Technology × Creativity

Responsive portfolio website for Denzi, built with HTML, CSS, and a small inline JavaScript enhancement layer.

## GitHub Pages deployment

This repository includes a GitHub Actions Pages workflow at `.github/workflows/pages.yml`.

1. Open **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **GitHub Actions**.
3. The workflow deploys automatically on pushes to `main`, or run it manually from **Actions → Deploy DENZI to GitHub Pages → Run workflow**.
4. Wait for the workflow's **Deploy to GitHub Pages** job to finish successfully.
5. The expected project site URL is **https://anmoloraon200-create.github.io/DENZI/**.

## Project files

- `index.html` — portfolio content and inline interactions
- `style.css` — complete stylesheet
- `.github/workflows/pages.yml` — automatic Pages deployment
- `robots.txt` and `sitemap.xml` — crawl metadata

The homepage stylesheet path is configured to match the root-level `style.css` file. This site is static; it does not include a database, authentication, admin dashboard, or persisted inquiry form. The inquiry form explains that contact delivery is not configured and does not claim to send or save submissions. Do not submit sensitive health information.

## Local preview

Open `index.html` in a browser or serve the repository with any static HTTP server.

## Next production steps

If you later need secure lead storage, login, booking, or admin management, add a server-side backend and authentication rather than placing secrets in browser JavaScript.
