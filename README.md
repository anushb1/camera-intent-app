# camera-intent-app (repo)

This repository includes a static **Camera Intent** web app under [`camera-intent-app/`](camera-intent-app/).

## Live site (GitHub Pages)

After you enable Pages (see below), the app is served at:

**https://anushb1.github.io/camera-intent-app/**

Use **HTTPS** so the phone browser allows the camera and motion APIs.

## One-time GitHub setup

1. Push this repo to GitHub (you already have `origin` set).
2. On GitHub: **Settings → Pages → Build and deployment**
3. Under **Source**, choose **GitHub Actions** (not “Deploy from a branch”).
4. Push to `main` or run the workflow manually (**Actions → Deploy to GitHub Pages → Run workflow**).

The workflow file is [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml).

## Local testing

```bash
cd camera-intent-app
python3 -m http.server 8765
```

Open http://127.0.0.1:8765/

## Phone testing

Open the **Live site** URL in Safari or Chrome. Allow camera (and motion if asked). Add the page to the home screen if you want a full-screen feel.
