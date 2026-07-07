# My Room, Planned — Wayfair Workstream 2 prototype

A **"done-for-you" budget-fit room planner**. The customer shares a brief (room,
budget, timeline, style, and what they already own); the tool returns a complete,
shoppable **Budget-Fit Room Plan** — hero pieces to buy now, accents to defer to
a later phase — that lands inside their budget.

**Live demo:** https://manojkumaraiproductlead.github.io/Wayfair-product/

## Flow

1. **Project intake** — a 3-step wizard: room selection, budget slider + timeline,
   style + inspiration + constraints ("I already have a gray sofa").
2. **Generate** — a skeleton-loader state simulates the budget-fit engine
   (a manual concierge in Q1; the customer graph in Q2).
3. **Budget-fit plan** — mood-board header, Phase 1 (Buy now) and Phase 2
   (Buy later) sections, and a live budget card with a spend progress bar.
4. **Review & tweak** — per-item **Swap** (curated alternatives), **Lock**
   (kept on regenerate), and **Remove**; **Regenerate** re-rolls only the
   unlocked pieces; **Add to cart** on any item or all buy-now pieces at once.

## Q1 fake-door metrics instrumented in the flow

Intake completion (>60%) · Plan acceptance — kept vs. swapped hero pieces (>50%) ·
Project-to-cart conversion (>20%).

## Build

Single self-contained `index.html` — HTML5 / CSS3 / vanilla JS, no dependencies,
inline SVG product art (renders offline). Adheres to Wayfair brand tokens
(purple `#7F187F`, Figtree). Static JSON simulates the plan data.

*Product case artifact — not affiliated with Wayfair.*
