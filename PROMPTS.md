# Prompts Used

These are the exact prompts used to generate this design in [Claude Design](https://claude.ai/design).

---

## Prompt 1 — Initial design request

> Create a 45-second animated video explaining how Israel is building underwater datacenters off the Mediterranean coast to cool the next wave of AI compute. 16:9.
>
> Structure:
> - 0-5s: Cold open. Title card "The AI compute race is going underwater." Wave animation in the background.
> - 5-15s: The problem. Animated stat reveal: "AI datacenters will consume 945 TWh by 2030." Show a row of land-based datacenters lighting up with a thermal overlay as heat builds.
> - 15-30s: The solution. Animated cross-section of a sealed server capsule descending off the coast of Tel Aviv. Seawater flows around it as passive cooling. Small fish swim past. Bubbles rise.
> - 30-40s: Three stat cards slide in, one after the other: "40% lower cooling costs." "Zero freshwater used." "8x closer to European users."
> - 40-45s: Closing card. "Israel's underwater datacenter race. Starts 2026." Leave room for a logo bottom-right.
>
> Visual style: clean tech, thin-line illustrations, Mediterranean blue + sand beige + pure white palette. Kinetic typography for every stat. Smooth camera pans, no hard cuts. No stock footage. No emoji. Serif for titles, sans-serif for body.

---

## Prompt 2 — Layout bug fix

*(After automated verifier check)*

> Fix both issues. The "TWh" overlap is because of the flex baseline alignment with negative letter-spacing — switch to inline-block with proper spacing. For Scene 3 captions, widen them and reduce title size.

**What changed:** Switched the TWh suffix from `flex-baseline` to `inline-block` with `whiteSpace: nowrap`. Widened Scene 3 caption containers to 480–500px and dropped the title font size to 46px.

---

## Prompt 3 — Suffix collision fix

*(After second verifier check)*

> Fix the italic-glyph collision in both Scene 2 and the Scene 4 stat cards.

**What changed:** Restructured the suffix to use `flex` with explicit `gap` and `padding` rather than relying on `margin` inside a letter-spaced parent.

---

## Prompt 4 — Stat card spacing

*(After third verifier check)*

> Widen the stat card gap and add padding on the suffix to clear the italic side-bearing collision in Scene 4.

**What changed:** Widened stat card gap to 56px, added `paddingLeft: 24` on the suffix span.

---

## Prompt 5 — Export to PDF

> Save this design as a PDF: Underwater Datacenters.html

**Result:** A separate print file (`Underwater Datacenters-print.html`) was generated as a 6-frame storyboard contact sheet — one keyframe per scene laid out on a single landscape page.

---

## Prompt 6 — Implementation

*(In Claude Code, after exporting the design bundle)*

> I exported this design from Claude Design. Read README.md in this workspace, then the chats/ transcripts, and implement the designs as described there. Implement Underwater Datacenters.html.

**What changed:** The three-file prototype (`Underwater Datacenters.html` + `animations.jsx` + `scenes.jsx`) was merged into a single self-contained HTML file that works without a web server.

---

*Full conversation exported from Claude Design · Implemented with Claude Code*
