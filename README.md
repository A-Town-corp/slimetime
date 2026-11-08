# SLIMETIME 🧪

A gooey neon-green countdown website. Set a time, pick how it's displayed, and share the drop.

## Features

- **SLIME TIME IN X MIN** — live countdown with seconds and a progress bar.
- **SLIME TIME AT HH:MM** — show the target time in the viewer's local time zone.
- Quick presets and a custom date/time picker.
- Fullscreen stage for projecting or streaming.
- Shareable links with the target timestamp and display mode.
- Responsive desktop/mobile layout, animated slime visuals, and local preference persistence.

## Run locally

Open `index.html` in a modern browser. No build system or backend is required.

Alternatively, run a static HTTP server in the repository:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploy

Host `index.html` with any static-site provider such as GitHub Pages or Cloudflare Pages. No environment variables or server-side components are needed.

**GitHub Pages:** After merging, go to **Settings → Pages** in the repository, choose **Deploy from a branch**, then select `main` and `/(root)`. Your site will be served from the Pages URL after deployment.

**Sharing:** Once hosted over HTTPS, use **COPY DROP LINK** to share the exact target time and selected display mode. When opening the HTML as a local file, the button copies a human-readable time instead.

## Notes

- Times entered through the picker use the browser's local time zone.
- The countdown updates once a second and rounds up the remaining minutes.
- The site uses Google Fonts where available and falls back to system fonts.
