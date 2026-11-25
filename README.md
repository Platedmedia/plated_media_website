# Plated Media Co website

One-page site for **Plated Media Co: ads made by a chef.** Plain HTML, CSS and a little vanilla JavaScript. No frameworks, no build step.

```
index.html     the whole site (styles and script are inside it)
privacy.html   plain-English privacy page (a template, so read it through)
images/        all photos and the logo
```

## Put it online with GitHub Pages (free)

1. Merge this work into the `main` branch.
2. On GitHub, open the repo and go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Pick **Branch: `main`** and folder **`/ (root)`**, then click **Save**.
5. After a minute or two the site is live at
   `https://tawhz1.github.io/plated_media_website/`

Using your own domain (like platedmediaco.com.au)? Add it under **Settings → Pages → Custom domain**, then update the two `og:` URLs near the top of `index.html`.

## Images still to add

Upload these into `images/` with **exactly** these file names. Until they're there, the site shows a tidy "Photo coming soon" panel in their place.

| File | Where it shows |
| --- | --- |
| `process-filming.jpg` | "How it works" |
| `work-rotisserie-logo.jpg` | The work grid |
| `work-picnic-westgate.jpg` | The work grid |
| `work-pasta-curry.jpg` | The work grid |

Already in place: `hero-chef-plating.jpg`, `q-portrait.jpg` (cropped from the "Who's behind it" mock-up), `made-in-the-west.jpg`, `work-banh-mi-footscray.jpg`, `work-ethiopian-footscray.jpg`, `work-bakery-sunshine.jpg`, the nine `cuisine-*.jpg` photos, and `logo-wordmark.jpg`. The logo was cropped from the corner of the banh mi image. If you have a cleaner original, upload it with the same name.

Tip: keep photos around 1600px wide or smaller so the site loads fast on phones.

## Placeholders to change

Search `index.html` for these:

| What | Search for | What to do |
| --- | --- | --- |
| **Form ID** | `YOUR_FORM_ID` | Sign up at formspree.io, create a form and paste your ID in. Full steps are in the comment above the form. File uploads need a paid Formspree plan. On the free plan the text still comes through. |
| **Phone number** | `04XX XXX XXX` | Replace the number in both the `href="tel:..."` and the visible text, then delete the "(placeholder)" note. |
| **Instagram** | `instagram.com/platedmediaco` | Check the handle is right. |
| **Reviews** | `PLACEHOLDER REVIEWS` | Swap in real reviews from real clients, with their permission. |
| **Package details** | `Edit the bullet points` | Make the bullets match what each package actually includes. |
| **Captions & suburbs** | `data-caption` / `<figcaption>` | Update the work and cuisine labels. |

Also read through `privacy.html` and make sure it matches how you actually work.

## Swapping a work photo for a video

Every tile in "The work" can play an `.mp4`. The comment above the grid in `index.html` explains how:

1. Point the tile's `data-src` at the `.mp4`, and the lightbox will play it as a video.
2. Optionally replace the thumbnail `<img>` with a muted, looping `<video>` so it moves in the grid too.
