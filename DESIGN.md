# Design

The landing page inherits the palcovideo.com brand. Values below were read from the live site's stylesheet on 2026-11-04. If that site changes, it wins.

## Colour

| Role | Value |
|---|---|
| Accent | `#C21E2B` |
| Accent hover | `#A81828` |
| Accent deep | `#7A1220` |
| Accent on black | `#FF6A78` |
| Ground | `#F1EBEB` |
| Alternate ground | `#F7F3F0`, `#EDE7E2` |
| Card | `#FFFDFC` |
| Ink | `#1A1A1A` |
| Body text | `#3A3A3A` |
| Muted text | `#5F5F63` |
| Dark band | `#000000` |

Red text on black fails contrast, so dark bands redefine `--accent` to the soft red. Primary buttons always use `#C21E2B` with white text (6:1).

The parent's muted text is `#6B6B6F`. This page uses `#5F5F63` so that it clears 4.5:1 on the cream ground.

## Type

| Voice | Face | Use |
|---|---|---|
| Display | Archivo 800/900, tracking -0.035em | Headings and numbers |
| Accent | Instrument Serif italic 400 | One emphasised word or phrase in a heading, in the accent colour |
| Body | Manrope 400 to 700 | Text |
| HUD | JetBrains Mono, uppercase, tracked | Buttons, film HUD, small data labels |

## Components

- **Buttons:** pill, mono uppercase, 48px tall (44px small). Primary is red, secondary is an ink outline, ghost is a white outline on film.
- **Cards:** `#FFFDFC`, 20px radius, 1px border, no resting shadow.
- **Logo:** rotated red square plus "PALCO VIDEO" in Archivo.
- **Header slate:** names the current chapter under the logo. It replaces section eyebrows, so headings stand alone.

## Motion

Easing is `cubic-bezier(.2, .8, .2, 1)`, from the parent site. Content is visible without JavaScript, and all motion respects `prefers-reduced-motion`.
