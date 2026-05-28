# gearCOMP — Cycling Gear Speed Calculator

A single-file, dependency-free web app for comparing bicycle drivetrain speeds across
chainring + cassette combinations. Open it anywhere — no server, no build step, no internet
required (charts are hand-drawn SVG).

**Live site:** https://dscohen.github.io/gearCOMP/

## Features
- **Speed at every gear** = (chainring ÷ cog) × wheel circumference × cadence.
- **Adjustable cadence** (default 100 RPM) with error bars spanning ±20 RPM.
- **Chainrings:** SRAM/Shimano 2x presets (standard, semi-compact, compact, subcompact,
  GRX) and 1x rings (36–48T), plus custom teeth entry.
- **Cassettes:** Shimano 11/12-speed road & GRX, SRAM road 12-speed, SRAM XPLR (incl.
  Garbaruk 10-44), SRAM Eagle mullet — plus custom cog lists.
- **Tire/wheel** circumference selector (700×25 → 700×40, 650b) and custom mm entry.
- **Units:** mph / km/h.
- **Compare mode:** two full drivetrains (A vs B) overlaid — shared bike/cadence — with a
  metrics summary and both full speed grids.
- **Sort modes** for the charts:
  - *Speed* — by actual speed.
  - *Gear #* — physical cassette progression (per ring, small → big cog).
  - *Realistic* — single front-shift model: small ring for the easier half, big ring for the
    harder half, cross-chained combos dropped, so the jumps reflect real-world shifting.
- **Avg gear step by thirds** (easy / middle / hard) of the range.
- Responsive layout that works on phones and tablets.

## Usage
Just open `index.html` in any browser, or visit the live site above. Everything updates live
as you change controls — no submit button.

## Development
It's one file: [`index.html`](index.html). Edit and refresh.
