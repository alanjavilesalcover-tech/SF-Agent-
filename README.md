# Sntledge.app

A simple static landing page for Sntledge with a blog powered by the
[Soro](https://trysoro.com) embeddable blog widget.

## Structure

| File | Purpose |
| --- | --- |
| `index.html` | Landing page (hero, features, CTA) |
| `blog.html` | Blog page containing the Soro embed |
| `styles.css` | Shared styles (light + dark) |

## The Soro blog embed

The blog is rendered by pasting the Soro widget snippet into `blog.html`:

```html
<div id="soro-blog"></div>
<script src="https://app.trysoro.com/api/embed/48d6c064-0473-44d0-a091-c5cf49927df5" defer></script>
```

The `<div id="soro-blog">` is where Soro injects the rendered blog, and the
`<script>` loads the embed bundle for workspace
`48d6c064-0473-44d0-a091-c5cf49927df5`. To use a different Soro blog, replace
that embed URL with the one shown in your Soro dashboard.

## Run locally

No build step. Open `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Push to any static host (Vercel, Netlify, GitHub Pages, Cloudflare Pages) —
the repository root is the site root.
