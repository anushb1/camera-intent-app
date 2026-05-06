# Handover pack — checklist (post-sales)

Use at **week 11–14** before BAU takes ownership.

## Documentation

- [ ] Architecture diagram (current state): sources → landing → Cloud SQL / BQ → BI
- [ ] Data dictionary for pilot marts (tables, keys, grain)
- [ ] KPI dictionary **final** (version aligned to prod)
- [ ] Job inventory: name, schedule, owner, runbook link, last success
- [ ] IAM: groups, roles, break-glass note
- [ ] Cost: rough monthly breakdown + tuning notes (partitions, slots)

## ML (if applicable)

- [ ] Model cards: features, training window, refresh cadence, known limits
- [ ] Prediction/forecast tables: schema, SLA, consumer list
- [ ] Retrain policy: who triggers, how often, acceptance criteria

## Operations

- [ ] On-call / escalation for first 30 days BAU
- [ ] Monitoring: alerts, dashboards, log links
- [ ] DR / backup: what is backed up, RPO/RTO expectation (pilot-appropriate)

## Knowledge transfer

- [ ] Recorded walkthrough (BI + data flow)
- [ ] Office hours scheduled (×2) with named maintainers

## Sign-off

- [ ] BAU owner name and date acknowledged
- [ ] Sponsor “pilot complete” note tied to charter success metrics
