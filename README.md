# SLIMETIME

A little countdown site for moments worth waiting for. Live at **[slime-time.at](https://slime-time.at/)**.

## Use it

- Switch between **SLIME TIME IN X MIN** and **SLIME TIME AT HH:MM**.
- Tap a quick preset (15 minutes to 2 hours), or pick a custom local date/time.
- Copy a link to share the exact target moment and display mode.
- Put the countdown into fullscreen for a bigger display.

The countdown runs in the browser and updates every second. It saves your last future target in local storage, and existing shared URLs using `?at=<unix-milliseconds>&mode=in|at` continue to work. Times shown in `AT` mode are localized to each viewer's device.

## Run it

Open `index.html` in a browser, or serve the folder locally:

```bash
python -m http.server 8080
```

No build step, backend, API keys or package dependencies. The display font comes from Google Fonts with local fallbacks.

## Deploy

GitHub Pages publishes the `main` branch at the root. The `CNAME` file is intentionally preserved so Pages continues using **slime-time.at**. Merge a PR to deploy a new version.

## Design approach

Version 2 is built around one hand-drawn slime character and an oversized green countdown, like an old event flyer or sticker. Controls use subdued greens instead of neon glows, competing gradients and constant floating animations. Focus, pressed, validation, arrival, and reduced-motion states are handled explicitly.

Design review drew on [unslop by Damir Sokolovsky](https://github.com/heydamir/unslop) (CC BY 4.0) and [Anti-Slop Frontend Skill](https://github.com/ItsRealAJ/Anti-Slop-Frontend-Skill). No source files from those projects are bundled here.