# AGENTS.md

- Static site with no build step. `index.html` is the whole site; `netlify.toml` publishes the repo root.
- `index.html` holds the Open Graph meta tags used for WhatsApp/social previews, plus a meta-refresh and a JS redirect to the catalog at a Claude artifact URL.
- Keep `og:image` pointed at a direct image file URL (e.g. `https://i.ibb.co/.../file.jpg`), not an ImgBB page URL, so previews render.
- If the catalog URL changes, update it in all three places: `og:url`, the meta refresh, and the script.
