# palco_landing_page

Single-file, responsive landing page for **Palco Video**, a commercial production house in India (est. 1985) serving brands, government ministries and creators from Delhi, Chandigarh and Mumbai. Content is sourced from the parent site, [palcovideo.com](https://www.palcovideo.com/).

## Page narrative
1. **Hero**: positioning, key facts, and an animated camera-viewfinder visual
2. **Trusted-by marquee**: ministries, PSUs and brands
3. **Who we are**: what Palco is and who it serves (brands, government & PSUs, creators)
4. **Services**: Video Production, Social Media Management and Creator Management, each with its deliverables
5. **Process**: brief → pre-production → shoot → post → delivery & distribution
6. **Capabilities**: Broadcast, Institutional and Creator-era pillars
7. **Clients**: NTPC and BRO highlights, plus per-ministry and per-brand work descriptions
8. **By the numbers**
9. **Selected work**: 7 films and 8 Shorts/Reels, all linking to YouTube
10. **Our story**: timeline, founders and crew roster
11. **Engagement models**, **FAQ**, **Contact** (form, hours, offices with map links)

## Tech stack
- Pure HTML5, CSS3 and vanilla JavaScript in a single `index.html`, with no build step
- Typography: Google Fonts (Bebas Neue, Inter, JetBrains Mono)
- Light studio theme (`#F8F8F6`) with amber accent (`#C88A22`) and dark ink bands (`#121316`)
- Motion: headline mask reveal, viewfinder open and running timecode, client marquee, scroll-scrubbed intro text, process rail fill, staggered reveals, scroll progress bar. All of it respects `prefers-reduced-motion`.
- WebP images served via `<picture>` with JPG/PNG fallbacks
- Semantic, accessible markup and JSON-LD `LocalBusiness` structured data

## Known gaps
- The contact and newsletter forms open a pre-filled email (`mailto:`). Neither has a submission backend yet.
- Shorts thumbnails are loaded from YouTube (`i.ytimg.com`).
