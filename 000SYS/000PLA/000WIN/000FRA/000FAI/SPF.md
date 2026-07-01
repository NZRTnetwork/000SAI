---
tags: [reference, schema, reference-codes, taxonomy]
aliases: [Strings Patterns Flows, SPF]
role: admin
created: 2026-04-01
status: active
type: reference
---


# Strings, Patterns & Flows

> Maps common operations across three tiers


## Tiers

- **000STR** — a string: single step → `{agent}-{app}-{object}-{type}`
- **000PAT** — a pattern: strings joined together (multi-step repeatable sequence)
- **000FLO** — a flow: patterns joined (end-to-end business flow)

---

## 000CLA – Claude (CTO Agent)

---

### Session

**String**
`cla-dol-tic-ses` — create CLA session ticket in Dolibarr

**Pattern**
`cla-dol-tic-ses → cla-obs-not-pln` — open session ticket → write working plan

**Flow**
`cla-dol-tic-ses → cla-obs-not-pln → cla-dol-tic-adm` — open → plan → close session

---

### Vault Documentation

**Strings**
`cla-obs-not-doc` — write Obsidian documentation note
`cla-obs-not-cfg` — update config/schema in vault
`cla-obs-not-ref` — update reference file in vault

**Pattern**
`cla-obs-not-doc → cla-obs-not-cfg → cla-obs-not-ref` — write doc → update config → update reference

**Flow**
`cla-obs-not-doc → cla-ncl-fil-doc → cla-fla-pst-doc` — write → share to Nextcloud → post to forum

---

### Planning

**Strings**
`cla-obs-not-pln` — write plan to Obsidian vault
`cla-win-scr-cfg` — configure Windows script/tooling

**Pattern**
`cla-obs-not-pln → cla-win-scr-cfg` — plan → implement tooling

**Flow**
`cla-obs-not-pln → cla-win-scr-cfg → cla-dol-tic-adm` — plan → implement → close ticket

---

### Code & Scripts

**Strings**
`cla-git-rpo-scr` — write or review code in GitHub repo
`cla-win-scr-cfg` — configure Windows script/tooling
`cla-git-rpo-cfg` — configure repo settings

**Pattern**
`cla-git-rpo-cfg → cla-git-rpo-scr → cla-win-scr-cfg` — set up repo → write code → configure locally

**Flow**
`cla-obs-not-pln → cla-git-rpo-scr → dan-cpl-adm-mig` — plan → code → DAN deploys

---

### TOGAF Phase

**Strings**
`cla-obs-not-doc` — write TOGAF deliverable in Obsidian
`cla-tog-doc-rev` — review TOGAF deliverable
`cla-fla-pst-doc` — post phase update to forum

**Pattern**
`cla-obs-not-doc → cla-tog-doc-rev → cla-fla-pst-doc` — write → review → publish

**Flow**
`cla-obs-not-doc → cla-ncl-fil-doc → cla-fla-pst-doc → aba-tog-doc-rev → cla-fla-pst-doc` — write → share → post → ABA reviews → post phase complete

---

### Agent Coordination

**Strings**
`cla-dol-tic-adm` — create or update agent ticket in Dolibarr
`cla-fla-pst-doc` — post to forum for agents
`cla-fla-pst-rev` — post review/feedback to forum

**Pattern**
`cla-dol-tic-adm → cla-fla-pst-doc` — assign ticket → post forum instruction

**Flow**
`cla-obs-not-pln → cla-dol-tic-adm → cla-fla-pst-doc → cla-fla-pst-rev` — plan → assign → instruct → review agent output

---

### Vault Taxonomy (Meta)

**Strings**
`cla-obs-not-str` — document a string in the vault
`cla-obs-not-pat` — document a pattern in the vault
`cla-obs-not-flo` — document a flow in the vault

**Pattern**
`cla-obs-not-str → cla-obs-not-pat → cla-obs-not-flo` — document string → pattern → flow

**Flow**
`cla-obs-not-str → cla-obs-not-pat → cla-obs-not-flo → cla-obs-not-ref` — build taxonomy → update reference

