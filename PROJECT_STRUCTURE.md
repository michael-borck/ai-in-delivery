# Project Structure — AI in Delivery

How this repo is organised. The repo is a **Quarto website** (`type: website`)
that renders the companion site into `docs/`, which GitHub Pages serves.

> Revamped June 2026. The previous version of this course (and this document)
> described a four-activity structure with role/constraint/crisis cards and a
> `render-all.sh` build — all superseded. The current course is the five
> differences + three sprints; the build is `scripts/build-site.sh`.

## Source vs. generated

- **Edit:** the `.qmd`/`.md`/`.scss` source at the repo root and in
  `readings/`, `activities/`, `handouts/`, `content/`.
- **Generated:** everything in `docs/` — produced by `scripts/build-site.sh`.
  Don't hand-edit `docs/`.

## What renders into the site

`_quarto.yml`'s `render:` list controls what becomes site pages:

| Source | Becomes | Notes |
|---|---|---|
| `index/before/workshop/frameworks/team.qmd` | the site's pages | nav defined in `_quarto.yml` |
| `readings/*.qmd` | pre-reading pages | listed on `before.qmd` |
| `activities/initiative-cards/*.md` | the 4 initiative pages | listed on `workshop.qmd` |
| `activities/worksheets/*.md` | the 3 sprint worksheets | listed on `workshop.qmd` |
| `handouts/**/*.md` | take-home frameworks | listed on `frameworks.qmd` |
| `content/slide-deck.md` | the deck | rendered **separately** by `build-site.sh` into `docs/content/` (not a nav page) |
| `course-bot.html` | global chatbot embed | injected on every page via `include-after-body` |

**Not rendered / not published:** `instructor-materials/` (facilitator guide,
the RetailFlow document answer-key, crisis walkthroughs, feedback),
`COURSE-ALIGNMENT-MAP.md`, `PROJECT_STRUCTURE.md`, `README.md`. Theme lives in
`brand.scss`.

## Theming & front matter

- Site theme: `_quarto.yml` → `theme: [cosmo, brand.scss]`.
- Listing pages (`before`, `workshop`, `frameworks`) pull `title` + `description`
  from each content file's YAML front matter — keep those fields when adding
  material.

## Build & deploy

```bash
./scripts/build-site.sh     # clean docs/, render website + deck, add .nojekyll
# then:
git add -A && git commit -m "..." && git push   # Pages serves main /docs
```

Local preview: `open docs/index.html`.

## Related, but separate repos

- **`sites/retailflow`** → `retailflow.eduserver.au` — the fictional company:
  storefront, internal document repository (the dossiers; access code
  `pilot2024`), and the 7 leadership chatbots. Its own Quarto-rendered
  `chatbots/` + static storefront/documents. Bot setup in
  `chatbots/_setup/`.
- **AnythingLLM** (`chat.eduserver.au`) — hosts the 7 RetailFlow staff bots and
  the course-assistant bot. Managed with `botstash` (`pip install botstash`).

## Adding material (common tasks)

- **A new reading:** add `readings/my-reading.qmd` with `title`, `description`,
  `order` front matter → it appears on *Before the day* automatically.
- **A new handout:** add `handouts/frameworks/my-handout.md` with `title` +
  `description` → appears under *Frameworks*.
- **Edit the deck:** edit `content/slide-deck.md`, then `./scripts/build-site.sh`.
- After any change: `./scripts/build-site.sh`, then commit + push.
