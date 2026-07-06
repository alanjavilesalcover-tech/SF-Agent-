# Sntledge blog

A single, minimal blog page powered by the
[Soro](https://trysoro.com) embeddable blog widget.

`index.html` contains the whole page — a heading and the Soro embed:

```html
<div id="soro-blog"></div>
<script src="https://app.trysoro.com/api/embed/48d6c064-0473-44d0-a091-c5cf49927df5" defer></script>
```

The `<div id="soro-blog">` is where Soro renders the blog; the `<script>`
loads the embed. Swap the embed URL to point at a different Soro blog.

## Run locally

No build step. Open `index.html`, or serve the folder:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```
