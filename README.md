# Bukmark landing page

Marketing site for **Bukmark**, an Android app that saves posts from TikTok, Instagram, YouTube Shorts, Threads, X and LinkedIn under nicknames you choose.

It is a static site: one `index.html` (HTML, CSS and a little vanilla JS), no build step and no dependencies.

## What is inside

- `index.html`: the whole page (styles and scripts are inline).
- `assets/`: mascot, platform icons, the Inter font and real app screenshots (`assets/screens/`).
- `Bukmark.apk`: the current release APK that the Download buttons point to.

## Features

- Indonesian / English toggle. It starts from the visitor's browser language and remembers the choice.
- Scroll reveals, a typing search demo, tilting phone mockups and other micro-interactions. All motion turns off for visitors who prefer reduced motion.
- Hamburger menu on phones.
- Responsive from small phones to wide desktops.

## Run locally

Any static file server works. For example:

```bash
python -m http.server 8000
# open http://localhost:8000
```

## Deploy

It can be hosted anywhere that serves static files. For GitHub Pages: Settings, Pages, deploy from the `main` branch, root folder. The empty `.nojekyll` file tells Pages to serve the files as they are.

## Updating the APK

Build the app in the Android repo, then replace `Bukmark.apk` here with the new `Bukmark-release.apk`.
