# AI in Delivery: Leading Projects That Ship

Course 3 of the **AI Capability Lifecycle Series** (Curtin exec-ed). A one-day masterclass for project managers and delivery leads on shipping AI projects without the predictable failures. Formerly "AI Leadership & Project Management Masterclass", fully revamped June 2026.

This repo holds the teaching materials **and** builds the companion website (Quarto → GitHub Pages).

## The course in brief

**Spine: why AI delivery is different.** Five things every project manager assumes that AI breaks: (1) "done" can't be specified, (2) a working demo is a trap, (3) the data is the uncertainty and it's discovered not specified, (4) verification *is* the product, (5) generic competence is the baseline, and the edge is human judgement. Anchored on the **trust tool** (Average/Precise × Small/Large) from *Conversation, Not Delegation*.

**Shape: one project, three sprints.** Participants are the delivery lead for one funded RetailFlow initiative and carry it through: **Sprint 1** scope it against reality · **Sprint 2** stakeholders & human-in-the-loop · **Sprint 3** roadmap, risk & the go/no-go. They scope and stress-test by interviewing the RetailFlow leadership team: live AI chatbots. They leave with a delivery design (scope, roadmap with gates, stakeholder + HITL plan, risk register).

## Repo layout

```
_quarto.yml            Quarto website config (type: website, output-dir: docs)
brand.scss             Site theme — tokens, light navbar, hero, icon cards, dark mode
_includes/fonts.html   Brand fonts (Fraunces + Inter), loaded site-wide
index.qmd              Landing page (the five differences + what you leave with)
before.qmd             Pre-readings landing (lists readings/)
workshop.qmd           The three sprints + initiative cards (listings)
frameworks.qmd         Trust tool, DDCD, Scale/Pivot/Kill + take-home handouts
team.qmd               Links to the RetailFlow staff chatbots
course-bot.html        Site-wide course-assistant chatbot embed (include-after-body)
readings/              3 pre-reading pages (.qmd)
activities/
  initiative-cards/    The 4 funded initiatives (one per group)
  worksheets/          The 3 sprint worksheets
handouts/              Take-home frameworks
content/slide-deck.md  The slide deck (rendered separately into docs/content)
instructor-materials/  Facilitator guide, the RetailFlow document answer-key,
                       crisis walkthroughs, past feedback (NOT published)
scripts/build-site.sh  Build the site (website + deck) into docs/
docs/                  Generated site (GitHub Pages serves main /docs)
```

## Build & deploy

```bash
./scripts/build-site.sh      # renders the Quarto website + deck into docs/
```

Deploy: commit and push. GitHub Pages serves `main` `/docs` at
`michael-borck.github.io/ai-in-delivery`. (`scripts/render-all.sh` is the old
build and is deprecated; use `build-site.sh`.)

## The RetailFlow case study & chatbots (separate)

The fictional company **RetailFlow** lives in its own repo (`sites/retailflow` →
`retailflow.eduserver.au`): a storefront, an internal document repository (the
dossiers students discern through, code `pilot2024`), and **7 leadership
chatbots**. Those bots, plus the **course-assistant bot** on this site, run on
AnythingLLM (`chat.eduserver.au`) and were built/maintained with
[botstash](https://pypi.org/project/botstash/). See
`sites/retailflow/chatbots/_setup/` for how the bots are configured.

## Instructor materials

In `instructor-materials/` (kept out of the published site): the facilitator
quick-reference, the **RetailFlow document answer-key** (which dossier docs are
signal vs. red herring), crisis walkthroughs, and feedback from prior cohorts.

## License

Developed for Curtin University. MIT (see LICENSE). Last revamped June 2026.
