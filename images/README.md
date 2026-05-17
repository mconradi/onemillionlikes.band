# Images

Add optimized photos here (WebP or JPEG). Keep file sizes small for fast loads on mobile.

Suggested files (update paths in `index.html` if you rename):

| File | Purpose |
|------|---------|
| `hero.jpg` | Main hero band photo (~1200px wide). |
| `logo-header.jpg` | Nav mark (128×128; crop from band logo). |
| `favicon-16.png`, `favicon-32.png`, `apple-touch-icon.png` | Tab / home-screen icons (generate from logo). |
| `og-1200x630.jpg` | Social preview image (~1200×630). |
| `gallery-01.jpg` … `gallery-03.jpg` | Photo strip (square or landscape; add more figures in HTML if needed). |
| `OML - Superpowers.jpeg` | EP teaser artwork (square) in the Music section. |
| `One_Million_Likes_Media_Kit.pdf` | Optional footer download. |

**Source folder:** copy from `../tobiastschepe_OML_Bilder_und_so` (e.g. band photos, studio session, Boila 2023) and rename to match the table above.

**Tips:** Export at 72–85% JPEG quality or use WebP. Compress with [Squoosh](https://squoosh.app/) before committing.

**Favicons from logo (macOS example):**

```bash
sips -z 128 128 YourLogo.jpg --out logo-header.jpg
sips -z 32 32 logo-header.jpg --out favicon-32.png
sips -z 16 16 logo-header.jpg --out favicon-16.png
sips -z 180 180 logo-header.jpg --out apple-touch-icon.png
```
