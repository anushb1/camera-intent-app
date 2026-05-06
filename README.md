# 90-Day GCP Pilot — Feedback, SE Motion & Post-Sales Roadmap

### Templates (fill-in artifacts)

| File | Use |
|------|-----|
| [templates/pilot-charter.md](templates/pilot-charter.md) | Scope, metrics, RACI, commercials, sign-off |
| [templates/kpi-dictionary.md](templates/kpi-dictionary.md) | Finance-aligned definitions + deck footnote |
| [templates/workshops.md](templates/workshops.md) | Definitions + tech/security agendas; follow-up email stub |
| [templates/handover-pack-checklist.md](templates/handover-pack-checklist.md) | Post-sales BAU handover |

---

## 1. Client voice — second pass on the pitch

**What I’d sign off mentally:** You showed you did homework on *our* business. The stack story is sane. Twelve weeks is credible.

**What still makes me pause:**

1. **I’m buying an outcome, not four deliverables.** Translate each deliverable into one line: “So on Monday I can ___.”
2. **Numbers without footnotes feel like theatre.** Put methodology in the footer: period, grain, profit formula. If you can’t, say “illustrative on sample data” and I’ll respect honesty more than precision I can’t audit.
3. **The discount and region stories need an owner.** Name who changes behavior if we trust this (Pricing? Regions?). Without that, this is analytics tourism.
4. **Tell me how we’ll know the pilot worked.** Three metrics max, with baseline and target. I shouldn’t have to ask.
5. **Risk:** data residency, PII, who’s on-call, what we get if we stop—four bullets, not a whitepaper.
6. **Money:** why $500 cap vs $180 estimate, what’s in “funded SE,” and one concrete phase-2 example so phase 2 isn’t a cliff.

**What would make me say “book the workshop”:** A one-page charter draft with success criteria + RACI + a proposed definitions session date. Slides alone don’t advance the deal.

---

## 2. SE next steps — tightened

**14-day objective:** Signed or verbally committed **pilot charter** + **KPI dictionary v0** + **sandbox spike** + **security path** identified.

| Day | Action | Owner |
|-----|--------|--------|
| 0 | Send follow-up: 3 bullets (heard / next artifact / **workshop date**) | SE |
| 1–3 | Book: **Definitions** (Finance + data, 90m) + **Tech/security** (platform + sec, 90m) | SE + AE |
| 3–7 | Run workshops → **KPI dictionary (1 page)** + **data-access request** (minimal slice first) | SE |
| 5–10 | **Spike:** land one entity, one BQ view, one BI tile (or export); document IAM gaps | SE + CE |
| 7–14 | Circulate **charter v1** (scope, metrics, RACI, commercials); **security checkpoint** before prod-like data | SE |

**Minimum viable charter (one page):** Scope / non-goals → 3 success metrics (baseline → target) → milestone weeks 4 / 8 / 12 → RACI → spend cap + exit note.

**Teams to pull (customer):** Sponsor · Finance · Data platform · Security · BI · (Pricing or Regions if stories are central) · Procurement when paper is warm.

**Teams to pull (Google):** AE/CSA · CE for spikes · Trust/compliance if questionnaire gates.

**If stuck:** Smaller data slice, “pilot basis” single profit definition, BI = their standard tool if Looker isn’t real.

---

## 3. Pre-sales checklist (short)

- [ ] Workshop invites sent (definitions + tech/security)
- [ ] KPI dictionary v0 + charter v1 in one folder
- [ ] Spike: ingest + consume in their project
- [ ] Security: classification + path to wider access
- [ ] Sponsor steering cadence on calendar

---

## 4. Post-sales roadmap (after signature)

Use this from **contract/start date** through **handoff to BAU**. Adjust weeks to your SOW.

### Phase A — Kickoff & land (weeks 0–2)

| Week | Focus | Outputs |
|------|--------|---------|
| 0 | Kickoff with sponsor; confirm RACI, comms, escalation | RAID log, meeting cadence |
| 0–1 | Environments: projects, IAM groups, billing alerts, repo/folders | Runbook link, access list |
| 1–2 | Ingest to landing; **pilot data** aligned to KPI dictionary | Reconciliation note vs source |

**Exit criteria:** Daily/weekly jobs run once end-to-end; Finance signs “pilot basis” numbers for one month.

### Phase B — Build core (weeks 3–8)

| Track | Milestone |
|--------|-----------|
| **Trusted KPI** | Mart + refresh SLA; Looker/BI content in draft |
| **Margin guardrail** | Report drillable by dimensions agreed in charter |
| **Forecast** | ARIMA_PLUS trained; backtest metrics vs target |
| **Classifier** | BOOSTED_TREE v1; flag-only workflow documented |

**Cadence:** Biweekly steering (demo + risks); weekly eng sync.

**Exit criteria:** All four in **staging** with documented definitions; UAT list with named testers.

### Phase C — Harden & UAT (weeks 9–11)

- Performance/cost review (slots, partitions, query patterns).
- Security: least privilege, audit sample, PII checks.
- UAT sign-off from Finance + BI owner; training session(s).
- Go-live checklist: rollback, on-call for 2 weeks.

**Exit criteria:** Production cutover; sponsor acknowledgment of success metrics snapshot.

### Phase D — Hypercare & handoff (weeks 12–14+)

| Activity | Detail |
|----------|--------|
| Hypercare | Triage bugs vs enhancements; weekly stability note |
| Handover pack | Architecture diagram, data dictionary, job list, runbooks, model cards (inputs, refresh, limitations) |
| BAU owner | Named maintainer for jobs, dashboards, model retrain policy |
| Expansion gate | Short readout: hit/miss on metrics, phase-2 options (streaming, Vertex, enterprise Looker) |

**SE role post-pilot:** Thin out after handoff; CE or PS for depth; AE owns renewal/expansion narrative.

---

## 5. Reference — first-pass client gaps (detail)

Use when expanding slides or security appendix: methodology footnote; discount lever + threshold defense; regional ROI framing; success table; Cloud SQL vs BQ + PII + exit + on-call; enterprise IdP/BI fit; ML limits (backtest, cold start, flag vs automate); logo/CTA.

---

*Internal planning doc — tailor names, regions, and week numbers to the account and SOW.*
