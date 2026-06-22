# imihtisham.dev

Personal portfolio — a single static `index.html` (no build step). Hosted on Cloudflare Pages.

## Edit

Everything lives in [`index.html`](index.html). Update the placeholder content:

- **Projects** — the 2nd and 3rd cards are placeholders; replace with real projects and links.
- **Project links** — the `href="#"` on the Counssel card (Live / Code) need real URLs.
- **LinkedIn** — verify the URL in the footer (`linkedin.com/in/ihtisham-ul-haq`) points to your actual profile.

## Local preview

Just open `index.html` in a browser, or:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy (Cloudflare Pages)

1. Push this repo to GitHub.
2. Cloudflare dashboard → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**.
3. Pick this repo. Build settings: **Framework preset = None**, **Build command = (empty)**, **Output directory = `/`** (root).
4. Deploy. Then **Custom domains** → add `imihtisham.dev` (one click, since the domain is already in your Cloudflare account).

Every `git push` to the default branch auto-deploys.
