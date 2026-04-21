# V&A Collection Browser

A personal PWA for browsing the V&A's [Order an Object](https://www.vam.ac.uk/info/order-an-object) collection, with the ability to track items you've already viewed in person.

## Features

- Search and filter V&A collections (venue, object type, date range)
- Mark items as **viewed** — persisted in local storage
- Toggle to **hide viewed items** so you only see new things
- Manage your viewed list (view all, remove items)
- Each card links to the full V&A collection page
- Works offline (service worker caches previous searches)
- Installable as a home screen app on iOS/Android

## Deploy to GitHub Pages

1. Create a new repo on [github.com/new](https://github.com/new) (public, empty — no README)
2. Push:

```bash
git init
git add .
git commit -m "initial commit"
git branch -M main
git remote add origin git@github.com:YOUR_USERNAME/va-browser.git
git push -u origin main
```

3. Go to **Settings → Pages → Source: main branch, / (root)** → Save
4. Live in ~60 seconds at `https://YOUR_USERNAME.github.io/va-browser/`

## Add to Home Screen (iPhone/Android)

1. Open the site URL in **Safari** (iOS) or **Chrome** (Android)
2. Tap **Share → Add to Home Screen**
3. Tap **Add**

## Data

Uses the [V&A Collections API](https://developers.vam.ac.uk/) (no API key needed). Viewed items are stored in your browser's localStorage — no server, no account required.
