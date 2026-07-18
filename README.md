# VARUNA

**Autonomous Multi-Agent UAV System for AI-Powered Flood Intelligence & Survivor Prioritization**

HackShastra · Zone C — Analysis & Reconnaissance · Round 2

Built by **Rudra Pratap Singh** (Team Lead) and **Himanshu Singh**.

## What this is

`varuna.html` is a single, self-contained showcase page for the VARUNA project — built from the Round 2 submission deck (`HackShastra_ZoneC_R2.pptx`). It's meant for a portfolio: open the file directly in any browser, no build step, no server.

VARUNA itself is a VTOL quad-plane that autonomously surveys 5+ km² of flood terrain, cross-verifies survivors using fused RGB + thermal imagery, and delivers a geotagged survivor list, Flood Extent Map, and Damage Assessment Report to rescue command — all within one uninterrupted, unpiloted sortie.

## What's on the page

- **Hero** — mission framing, team credit, headline specs
- **Stat strip** — survey area, endurance margin, MTOW, thrust-to-weight
- **Mission concept** — the core objective and how Round 2 builds on Round 1
- **Detection pipeline** — the thermal-verified, two-sensor voting system, with an animated scan-line diagram illustrating how a candidate gets confirmed
- **Airframe & propulsion** — structural mass, CG management, motor sizing math
- **Structural & flight simulation** — FEA (joint stress, safety factor) and CFD (cruise aerodynamics) results
- **System architecture** — all 6 subsystems: power/propulsion, flight core, perception/AI, comms, ground segment, payload bay
- **Mission timeline** — T+0 launch through T+75 report delivery
- **Simulated sortie log** — a representative telemetry trace showing survivor confirmations and a rejected false positive
- **Constraint compliance** — all 4 Zone C requirements matched against VARUNA's solution
- **Feasibility & cost** — full BOM-style cost breakdown, ₹2,01,000 total

## How to use it

1. Open `varuna.html` directly in a browser — that's it.
2. To host it, upload the single file anywhere that serves static HTML (GitHub Pages, Netlify, Vercel, or as an attachment).
3. To edit content, all copy lives in the HTML body; all styling is in the `<style>` block at the top using CSS custom properties (`--bg-deep`, `--thermal`, `--water`, etc.) so colors and spacing can be changed from one place.

## Tech notes

- Zero dependencies beyond three Google Fonts (Space Grotesk, Inter, JetBrains Mono), loaded via `<link>` in the `<head>`.
- All interactivity (scan-line animation, telemetry log) is vanilla JavaScript, no libraries.
- Respects `prefers-reduced-motion`, keyboard focus is visible throughout, and the nav/timeline/architecture grid are all responsive down to mobile.
