# Donut Palace — DeRidder, LA

One-page website for Donut Palace, 732 N Pine St, DeRidder, LA 70634.

**Live:** https://donutpalace-deridder.pages.dev

## What's here
- `index.html` — the whole page (inline CSS and JS, no build step)
- `assets/` — hero video loops (AV1 + H.264, wide and tall), posters, display-case photos, icons
- `assets/fonts/` — self-hosted WOFF subsets of TeX Gyre Bonum and Heros (GUST Font License)
- `og.jpg`, `manifest.webmanifest`, `sitemap.xml`, `robots.txt`, `_headers` (Cloudflare Pages cache headers)

## Notes
- Hero video: generated in Higgsfield with Seedance 2.5 (first frame = last frame for a true loop),
  crossfaded at the seam and upscaled to 1080p. Raw generations are on the `raw-assets` branch.
- Hours, phone, menu and prices come from the shop's Google Maps listing (Nov 2026).
  Update the hours table, the `OPEN` array in the script and the JSON-LD together if hours change.
- Parallax and the video respect `prefers-reduced-motion`.

## Deploy
Cloudflare Pages project `donutpalace-deridder` (direct upload): zip the files in this repo's root
and upload them as a new deployment in the Cloudflare dashboard.
