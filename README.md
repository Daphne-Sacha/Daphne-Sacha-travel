# Daphne & Sacha — Travel Content Portfolio

## Why this version, and not the single-file one

The all-in-one HTML file worked everywhere for photos, but video
packed that way (as "base64") is known to be unreliable specifically
on mobile Safari/iOS — it can fail to play even though the exact
same file plays fine on a computer. That's a limitation of the
technique, not of the design, and there's no local-file workaround
that fixes it for good. The real fix is hosting the site properly,
which is what this version is built for.

## Get a working link in under a minute (no account, free)

1. Unzip this file — you should end up with `index.html`, `README.md`
   and a `media` folder, all in one place.
2. Go to **app.netlify.com/drop** on your computer.
3. Drag the whole unzipped folder onto the page.
4. Netlify gives you a live `https://...netlify.app` link immediately.
   Open that link on your iPhone — video will play normally, because
   it's now a real hosted site instead of a local file.

That link works for testing today and can be shared with Nakama /
Akre / Anahata for feedback. When you're ready to put this on a real
domain, the same drag-and-drop panel lets you connect one — or I can
walk you through that when you get there.

## Before you publish — replace these

Search `index.html` for `yourdomain.com`, `yourhandle`, `[Your City]`,
and the three "Add a short, real quote..." lines:

1. **Email** — `hello@yourdomain.com` (contact link + form). The form
   has no backend by design: it opens the visitor's email app with
   their message pre-filled, so it works on any host, no server needed.
2. **Instagram handle** — `instagram.com/yourhandle`.
3. **Three testimonials** — in "Kind Words." Replace with real
   feedback from Nakama, Akre and Anahata once you have it.
4. **Footer city** — `[Your City]`.
5. **`og:image`** — once the site is live, change it to the full
   `https://yourdomain.com/media/...` URL so link previews on
   Instagram/WhatsApp/iMessage show a photo.

## Updating content later

All copy lives directly in `index.html`. All media lives in
`media/<name>/` — swap a file for a new one of the same file name
and similar aspect ratio and the layout won't need to change.
