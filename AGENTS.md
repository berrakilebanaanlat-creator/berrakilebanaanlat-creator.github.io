# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **static GitHub Pages site** for the Ancient Ghost Vision Detector Android app. It has **no** `package.json`, Docker, databases, or build step.

### Services

| Service | Purpose | How to run |
|---------|---------|------------|
| Static HTTP server | Local dev / E2E | From repo root: `python3 -m http.server 8080` |

### URLs (local, port 8080)

- Privacy policy: http://localhost:8080/ancient-ghost-vision/
- AdMob `app-ads.txt`: http://localhost:8080/app-ads.txt
- Google Search Console verification: http://localhost:8080/googlefeb5bd10cf5132b0.html

Production is served from GitHub Pages at `https://berrakilebanaanlat-creator.github.io/`.

### Lint / test / build

There are no project-defined lint, test, or build scripts. Validation is manual or via HTTP checks (status 200, expected content in HTML/`app-ads.txt`).

### Notes

- The privacy page language switcher uses hash routes (`#tr`, `#en`) and client-side JS; test both locales by loading the page and switching Türkçe / English.
- The React Native app, Play Billing backend, and CDN described in the privacy policy live **outside** this repo.
