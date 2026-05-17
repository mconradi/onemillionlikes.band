# One Million Likes — static press site

Single-page band press kit: plain HTML + CSS (one small script for the copyright year and YouTube embeds). Add assets under `images/`; replace placeholders in `index.html` as you go.

## Preview locally

Open `index.html` in your browser, or from this folder:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Swap embeds and links

| What | Where |
|------|--------|
| **Spotify** | Music section: replace the gray placeholder with Spotify → Share → **Embed** → paste the `<iframe>`. |
| **Coming soon** | Music section: EP teaser card — title, copy, and artwork (`images/OML - Superpowers.jpeg`). |
| **YouTube** | Videos section: set `data-youtube-id` on each `iframe.youtube-embed` (the ID from `youtube.com/watch?v=…`). Update captions. |
| **Shows** | `#shows` list: add `<li class="show-list__item">` rows (copy pattern from [mconradi.com](https://mconradi.com)). |
| **Hero + gallery** | Add optimized images to `images/` — see `images/README.md`. |
| **Social footer** | Replace `href="#"` on Instagram, YouTube, and Spotify icons. |
| **Media kit PDF** | Optional: add `images/One_Million_Likes_Media_Kit.pdf` and uncomment the footer link in `index.html`. |

Source photos live in `../tobiastschepe_OML_Bilder_und_so` — copy and rename into `images/` as needed.

## Deploy on GitHub Pages

1. Push this repository to GitHub.
2. Repo → **Settings** → **Pages**.
3. **Build and deployment**: Source = **Deploy from a branch**, Branch = `main`, folder = **`/ (root)`**.
4. Save. The site will be at `https://<username>.github.io/<repo>/` until a custom domain is configured.

`CNAME` is set to `onemillionlikes.band` for GitHub Pages custom domain.

## Custom domain (onemillionlikes.band)

1. In GitHub Pages settings, set **Custom domain** to `onemillionlikes.band` and enable **Enforce HTTPS** after DNS propagates.
2. At your DNS host, add the records GitHub documents for apex and `www` ([GitHub Pages custom domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)).

No build step is required.
