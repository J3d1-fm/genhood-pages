# genhood.com

Static site for Genhood / Gengames Interactive. No build step, no dependencies —
just HTML/CSS/JS. Edit the files directly and re-upload.

```
index.html      — home (Hero · About/Mission · Vibe · Game · Careers · Contact)
careers.html    — Careers + open role (Influence Manager / SMM, AI-integrated)
privacy.html    — Privacy Policy
pitch.html      — CONFIDENTIAL investor materials cover (unlisted, noindex)
pitch/          — interactive.html (pitch) + deck PDF (unlisted, noindex)
assets/         — images (game art, logos, screenshots)
robots.txt      — blocks /pitch from search engines
sitemap.xml     — lists public pages only
CNAME           — custom domain for GitHub Pages (genhood.com)
```

### Two things to set before/at deploy
- **LinkedIn link**: already set in the footer of `index.html` and `careers.html`
  → https://www.linkedin.com/in/filipp-mishchenko-893182234/
- **Confidential pitch**: it lives at `https://genhood.com/pitch.html`. It is NOT
  linked from the site and is excluded from search (robots.txt + noindex), so it's
  reachable only by people you send the link to — confidential, not secret. Share
  that URL directly with investors. (It is still publicly reachable by anyone who
  has the link; if you ever want a real password, tell me and I'll add a gate.)

## Deploy to GitHub Pages

1. Create a repo on github.com (e.g. `genhood-site`). Public is fine.
2. Upload everything in this folder to the repo root (drag the files into the
   GitHub web uploader, or `git push`). Keep `assets/` as a folder and keep
   `CNAME` at the root.
3. Repo → **Settings → Pages** → "Build and deployment" → Source: **Deploy from a
   branch** → Branch: `main`, folder: `/ (root)` → Save.
4. Wait ~1 min. The site goes live at `https://<username>.github.io/genhood-site/`
   first, then at your domain once DNS is set.

## Point genhood.com at it

In your domain registrar's DNS, add:

- Four `A` records for the apex `genhood.com` →
  `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- One `CNAME` record for `www` → `<username>.github.io`

The included `CNAME` file already tells GitHub the domain is `genhood.com`. In
Settings → Pages, tick **Enforce HTTPS** once the certificate is issued (a few
minutes to a few hours after DNS propagates).

## Updating content

- Text/links: edit `index.html` (everything is plain, labeled HTML).
- Privacy Policy: edit `privacy.html`.
- Images: drop a new file in `assets/` and point the matching `<img src="">` at it.

The Bloghouse Rivals "Play" buttons link to the live Google Play listing.
