# Meadows Run · Beaverton Toyota × Mt. Hood Meadows

Mobile-first endless ski run for Beaverton Toyota × Mt. Hood Meadows. Static HTML — no build step.

## Live demo

**https://pinheij.github.io/meadows-run/**

GitHub Pages deploys from `main` (root). Every push to `main` rebuilds the live URL (usually within a minute).

## Local play

```bash
cd ~/ski-game   # or clone path
python3 -m http.server 8765
# open http://localhost:8765
```

Or open `index.html` directly in a browser.

## Edit → live update

```bash
# from repo root
git add -A
git commit -m "describe the change"
git push origin main
```

Then hard-refresh the Pages URL (or wait ~30–60s).

## Embed

```html
<div style="position:relative;width:100%;max-width:480px;height:720px;margin:0 auto;border-radius:16px;overflow:hidden;box-shadow:0 12px 40px rgba(0,0,0,.45);">
  <iframe
    src="https://pinheij.github.io/meadows-run/"
    style="width:100%;height:100%;border:none;"
    title="Meadows Run"
    allow="autoplay"></iframe>
</div>
```

## Files

| File | Role |
|------|------|
| `index.html` | Game (CSS + JS in one file) |
| `toyota-badge-96.png` | In-run collectible / howto icon |
| `toyota-badge-128.png` | Higher-res badge asset |
