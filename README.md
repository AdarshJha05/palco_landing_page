# palco_landing_page

Single-file, responsive landing page for **Palco Video**, a commercial production house in India (est. 1985) serving brands, government ministries and creators from Delhi, Chandigarh and Mumbai. Content is sourced from the parent site, [palcovideo.com](https://www.palcovideo.com/).

## Page narrative
1. **Hero**: positioning and key facts over a muted film loop (a still shows on mobile, on data saver and with reduced motion)
2. **Trusted-by marquee**: ministries, PSUs and brands
3. **What is Palco Video?**: a plain-language answer, the studio's heritage, and who it serves (brands, government & PSUs, creators)
4. **Services**: Video Production, Social Media Management and Creator Management, each with its deliverables
5. **Process**: brief → pre-production → shoot → post → delivery & distribution, with typical timelines
6. **Why Palco**: production and distribution in one house, proof points, and the Broadcast, Institutional and Creator-era pillars
7. **Clients**: NTPC and BRO highlights, plus per-ministry and per-brand work descriptions
8. **By the numbers**
9. **Selected work**: 7 films and 8 Shorts/Reels, all linking to YouTube
10. **Our story**: timeline, founders and crew roster
11. **Engagement models**, **FAQ**, **Contact** (form, hours, offices with map links)

## Tech stack
- Pure HTML5, CSS3 and vanilla JavaScript in a single `index.html`, with no build step
- Brand: matches palcovideo.com. See `DESIGN.md` for the tokens.
- Typography: Google Fonts (Archivo, Instrument Serif, Manrope, JetBrains Mono)
- Cream ground (`#F1EBEB`) with red accent (`#C21E2B`), black bands, and soft red (`#FF6A78`) for accents on black
- Motion: headline mask reveal, viewfinder open and running timecode, client marquee, scroll-scrubbed intro text, pinned service card stack, sticky process counter and rail fill, word-by-word section titles, shutter-style image reveals, count-up stats, a timeline that draws on scroll, a header slate naming the current chapter, and a scroll progress bar. All of it respects `prefers-reduced-motion`.
- WebP images served via `<picture>` with JPG/PNG fallbacks
- Semantic, accessible markup and JSON-LD `LocalBusiness` structured data

## Known gaps
- The contact and newsletter forms open a pre-filled email (`mailto:`). Neither has a submission backend yet.
- Shorts thumbnails are loaded from YouTube (`i.ytimg.com`).
