# Facilitator Key — RetailFlow document repository

The internal portal (retailflow.eduserver.au → Internal, code `pilot2024`) holds ~26 documents across the four initiatives plus company-wide records. Groups are **not** told which documents matter — discerning relevance is part of the exercise (the same skill as handing an AI a folder and asking "what's relevant here?"). This key tells *you* what's signal, what's a trap, and the "needle" buried in the noise docs.

**Legend:** ✅ relevant · ⚠️ relevant but contains a trap to read critically · 🎣 red herring / noise (with any buried nugget noted) · ❌ outdated/superseded trap.

## Company-wide
| Doc | | Note |
|---|---|---|
| Company fact sheet | ✅ | Core background, all initiatives. |
| Leadership org chart | ✅ | Maps to the chatbots; identifies sponsors/owners. |
| IT & data systems overview | ✅ | Most relevant to inventory & pricing (legacy systems, fragmentation). |
| Responsible AI principles (draft) | ✅ | Governance context for all four; note it's only a draft. |
| The RetailFlow Buzz (newsletter) | 🎣 | Pure noise — store opening, wellness day, footy tipping. No delivery relevance. |
| Strategy offsite notes (2024) | ❌ | **Trap.** Dated 2024, says "AI not a near-term priority," different budgets. Superseded by the 2026 funded decision. Groups must spot the date. |

## Customer-service chatbot ($450K)
| Doc | | Note |
|---|---|---|
| Board funding memo | ✅ | The mandate + board commitments (26h→<4h). |
| Data readiness profile | ✅ | **Key doc** — good transcript data, but scattered policies; grounding is the critical path. |
| Vendor proposal | ⚠️ | Gotchas: per-conversation pricing balloons at scale; "97.8% accuracy" on the vendor's own corpus; offshore data residency. |
| Returns & refunds policy | ✅ | Ground truth the bot must be grounded in (30-day, sale items final, etc.). |
| CS team email thread | 🎣 | Mostly chatter. **Needle:** Raj's note that the bot told a customer "14 days" when it's 30 — the live wrong-answer incident, corroborating the grounding risk. |
| AI pilot dashboard (Week 6) | ✅ | Real metrics; AI nails order-tracking (94%), struggles with sizing (78%). |

## Dynamic pricing ($850K)
| Doc | | Note |
|---|---|---|
| Board funding memo | ✅ | Mandate + "this year" board expectation (timeline tension). |
| Data readiness profile | ✅ | **Key doc** — no competitor feed; fragmented demand; backtest ≠ live. |
| Vendor proposal | ⚠️ | Gotchas: backtest on RetailFlow's own history; guardrails off by default; needs a clean competitor feed they lack. |
| Pricing & markdown governance | ✅ | Hard constraint — approval thresholds, brand/price rules. Contradicts the vendor's "autonomous" default. |
| Strategy memo on pricing (2023) | ❌ | **Trap.** Dated 2023, argues *against* dynamic pricing. Superseded. Groups must notice it's stale. |

## Inventory optimisation ($1.1M)
| Doc | | Note |
|---|---|---|
| Board funding memo | ✅ | Mandate; milestone-gated budget, pilot-first first tranche. |
| Data readiness profile | ✅ | **Key doc** — siloed data, ~22% SKUs need cleanup; recommends single-category (homewares) pilot. |
| Legacy systems note (IT) | ✅ | Marcus's feasibility note — no API, batch lag, out-of-support inventory system, key-person risk. |
| Stock replenishment policy | ✅ | The manual process AI would replace. |
| Warehouse operations email | 🎣 | Mostly noise (forklift safety, farewell, car park). **Needle:** chronic nil-stock on homewares candles in regional stores — points at the pilot category. |

## Fraud detection ($650K)
| Doc | | Note |
|---|---|---|
| Board funding memo | ✅ | Mandate + explicit board constraint: don't cut losses by wrongly declining legit customers. |
| Data readiness profile | ✅ | **Key doc** — buy-not-build; team shouldn't own it; real risk is threshold tuning. |
| Vendor proposal | ⚠️ | Gotchas: ~8% of orders flagged, ~1 in 6 of those legitimate; black-box model; per-transaction fees; benchmarked on others' data. |
| Chargeback & refund policy | ✅ | Current manual process; notes they can't currently measure the false-block rate (the baseline to beat). |
| Finance team email | 🎣 | Mostly EOQ/audit chatter. **Needles:** the FY25 fraud-loss figure ($3.2M, up from $2.4M), and the complaint that legit customers are wrongly held today. |

---

**How to use in the room:** the "relevance" judgement is itself markable. A strong group reads its own folder *and* the company-wide docs, spots the trap (the stale strategy memo / the vendor gotcha), and finds the needle in the noise doc. A weak group takes the vendor proposal at face value or treats the outdated memo as current. Tie it back to the trust tool: deciding what to trust applies to *documents and vendors*, not just AI output.
