# Daphne & Sacha — Travel Content Portfolio

Static site, no build step, no dependencies. `index.html` + a `media/`
folder with the real photos and videos, ready to push to GitHub.

## Push to GitHub

```bash
cd daphne-sacha-portfolio      # this unzipped folder
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/<you>/<repo>.git
git push -u origin main
```

## Get a live link

**Option A — GitHub Pages (free, built into GitHub)**
Repo → Settings → Pages → Source: `Deploy from a branch` → Branch: `main` / `root`.
GitHub gives you a `https://<you>.github.io/<repo>/` link within a
minute or two.

**Option B — Netlify, connected to this repo**
On [app.netlify.com](https://app.netlify.com), "Add new site" →
"Import an existing project" → pick this GitHub repo. Every push to
`main` redeploys automatically, and you get a `https://...netlify.app`
link plus the option to attach a real domain later.

Either way, because it's a real hosted site (not a local file), video
plays correctly everywhere, including mobile Safari — which is not
guaranteed with local double-clicked HTML files.

## Current state

- **Email**: `daphnedenier@gmail.com` (contact link + form). The form
  has no backend by design — it opens the visitor's email app with
  their message pre-filled, so it works on any host, no server needed.
- **Instagram**: not linked on the site.
- **Testimonials** ("Kind Words"): three short quotes, one per hotel.
  Wording can be adjusted any time — they live directly in `index.html`.
- **Footer city**: Geneva.
- **`og:image`**: still points to a relative path. Once the site has a
  real domain, update it to the full `https://yourdomain.com/media/...`
  URL so link previews on Instagram/WhatsApp/iMessage show a photo.

## Updating content later

All copy lives directly in `index.html`. All media lives in
`media/<name>/` — swap a file for a new one of the same file name and
similar aspect ratio and the layout won't need to change.
