# lbh-link-in-bio
# Link in Bio

A single-file, dependency-free "link in bio" page (Linktree-style). Edit one config block, push, done.

## Deploy on GitHub Pages

1. Create a new repo. For a personal page at `https://<username>.github.io`, name the repo exactly `<username>.github.io`. (Any repo name also works — you'll just get `https://<username>.github.io/<repo>/`.)
2. Add `index.html` to the repo root and commit.
3. Repo **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. Wait ~1 minute, then open the URL Pages shows you.

## Customize

Open `index.html` and edit only the `CONFIG` block near the bottom:

- `name`, `handle`, `bio` — your text.
- `avatar` — an image URL, or leave `""` to auto-show your initials.
- `theme` — change the hex values to rebrand the whole page (accent drives the buttons + the background glow).
- `links` — each gets a big tappable button. `icon` is optional; `highlight: true` makes one featured gradient button (use it on just one).
- `socials` — the small icon row up top.

### Icons
Use any key from the `ICONS` object: `website, link, mail, calendar, github, x, instagram, linkedin, youtube, tiktok, spotify`. To add your own, paste an SVG into `ICONS` with a new key and reference that key.

## Notes / limits
- Fully static, so there are **no click analytics** and no dashboard — editing means editing this file and pushing.
- No external requests (no Google Fonts / icon CDN), so it's fast and private.
