# Donut Palace site — progress (saved Thu Nov 26, 2026, 12:10 PM CT)

Finishing run scheduled for **Fri Nov 27, 5:00 AM CT**.

## Done
- Hero video made in Higgsfield (Seedance 2.5, its top-tier model; free 720p bonus seconds).
  Key stills: Higgsfield Soul Cinema 2K, used as both first and last frame for a true loop.
  - Landscape: `hero-landscape-720.mp4` (raw, this branch)
  - Portrait (phones): `hero-portrait-720.mp4` (raw, this branch)
- Loops cleaned up (0.75 s tail-to-head crossfade, seam = normal frame step) and upscaled
  720p -> 1080p (lanczos + light CAS). Web encodes in `wip-progress.zip`:
  - `land-crf25.mp4` 1920x1080 H.264 (~0.8 MB), `port-crf25.mp4` 1080x1920 H.264 (~0.7 MB)
  - AV1 versions (`land-av1*.mp4`, `port-av1.mp4`) for browsers that support it
  - Posters (first frame of each loop)
- Display-case stills for the About section: `case-1.jpg`, `case-2.jpg`
- Logo: crowned glazed donut mark (`logo/mark.svg`, apple/maskable icon variants)
- Fonts (self-hosted WOFF subsets): TeX Gyre Bonum (Bookman-style display) + TeX Gyre Heros / Heros Cn

## Confirmed facts (Google Maps listing)
- Donut Palace, 732 N Pine St, DeRidder, LA 70634 (30.8571297, -93.2886828; plus code VP46+VG)
- Phone (337) 463-9800 (also on the shop's menu board: "for large order please call in advance")
- Hours: Mon–Sat 4:30 AM–12 PM, Sun 5 AM–12 PM (holiday hours may differ)
- Dine-in, takeout; no delivery. $1–10 per person. 4.6 stars on Google.
- Menu + prices: from the Google menu (Drinks, Donuts, Kolache, Croissant, Others)

## Design plan
- Palette: pre-dawn ink #141C33, glaze gold #E7A548, cherry tile #A3243B, tile white #FBFAF6, cocoa #2B1B16
- Type: Bonum Bold/Bold Italic for display; Heros for text; Heros Cn for the letterboard menu
- Sections: hero (video + bokeh layer + content, 3-depth parallax) / checker band / about /
  letterboard menu / 3 verbatim Google reviews / hours (live open-closed) + location / footer
- Reviews (verbatim): Stephanie G. "The donuts are always fresh, soft, and full of flavor."
  Tina G. "Very sweet customer service! 1st time coming will return."
  Carla M. "The store was clean and the cashier was super friendly."

## Next (5 AM run)
1. Build index.html (inline CSS/JS), icons, OG image, sitemap, JSON-LD
2. Test locally in headless Chrome (desktop + phone sizes, reduced motion)
3. Commit site to `main` (GitHub web upload)
4. Deploy: Cloudflare Pages direct upload -> donutpalace-deridder.pages.dev
5. Verify live: video autoplay/loop/poster, parallax, tel:/Maps links, performance
