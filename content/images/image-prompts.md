# Image prompts: the two deck visuals

For the rebuilt `slide-deck.md`. Generate each, save into this folder with the
exact filename, then add `![](./images/<filename>)` to the relevant slide
(replace the `<!-- NEW VISUAL NEEDED -->` comment for the trust-tool one; add the
five-differences image under the `# The five differences` heading).

**Shared style:** clean, flat, modern corporate-infographic look; generous
whitespace; muted business palette: **blue `#2563eb`, green `#10b981`, amber
`#f59e0b`**, dark text `#1f2937` on white; 16:9, high resolution.

> ⚠️ **Text caveat.** These are *diagrams with specific labels*, and most image
> generators garble multi-word text. Two reliable routes: (a) use a model that
> renders text reasonably (gpt-image-1 / DALL·E 3) and keep the baked-in labels
> SHORT; or (b) generate a clean, **label-free** background from the prompt and
> add the real text in your slide tool. Better still for crisp text: ask me to
> build these as SVGs: perfect labels, on-brand, no garbling.

---

## 1. `five-differences-summary.png`
**Use:** the "The five differences" summary slide.

**Prompt:**
> A clean, flat 16:9 corporate infographic, white background, titled "Why AI delivery is different". Five evenly-spaced horizontal rows. Each row has three zones connected by thin arrows: a left chip (a normal-project assumption), a centre chip (why AI breaks it), and a right chip in a bolder colour (the leadership move). Row 1: "'Done' is specifiable" → "Non-deterministic" → "Manage a distribution". Row 2: "A demo means nearly done" → "Demo-to-production gap" → "Progress is illusory". Row 3: "Requirements are the uncertainty" → "The data is, discovered" → "Run it as discovery". Row 4: "QA is a phase" → "Verification is the product" → "Design where judgement lives". Row 5: "More throughput = value" → "Generic is the baseline" → "Protect human variation". Left chips light grey, centre chips soft blue, right chips green; numbered 1–5 down the left in amber circles. Minimal, lots of whitespace, modern flat vector style, muted blue/green/amber palette.

---

## 2. `trust-tool-matrix.png`
**Use:** the "A tool for the hardest call: when to trust AI" slide.

**Prompt:**
> A clean, minimal 2×2 matrix diagram, 16:9, white background, flat modern vector style. Title at top: "The trust tool: when to trust AI". X-axis labelled left-to-right "Average → Precise" (how exact the answer must be). Y-axis labelled bottom-to-top "Small → Large" (stakes & scope). Four quadrants: bottom-left (Average + Small) filled soft green, label "Lean in, let AI run"; top-right (Precise + Large) filled soft amber, label "Keep a human in the loop"; the two off-diagonal quadrants light grey, each labelled "Judgement call". Thin blue axis lines and arrowheads, rounded quadrant corners, generous whitespace, minimal text, muted blue/green/amber business palette.

---

## Existing deck images (for visual consistency)
`content/images/` already has the deck's other diagrams (traditional-vs-ai-paths,
pilot-program, speed-dating, scale-pivot-kill-decision-tree, etc.), so match their
flat, muted, professional style so the new two don't stand out.
