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

- **000STR** — a string: single step → `{app}-{object}-{type}`
- **000PAT** — a pattern: strings joined together (multi-step repeatable sequence)
- **000FLO** — a flow: patterns joined (end-to-end flow)

---

## 000CLA – Claude (CTO Agent)

---

### Session

**String**
`dol-tic-ses` — create CLA session ticket in Dolibarr

**Pattern**
`dol-tic-ses → llm-tsk-pln` — open session ticket → write task plan

**Flow**
`dol-tic-ses → llm-tsk-pln → dol-tic-end` — open → plan → close session

---

### Vault Documentation

**Strings**
`obs-not-doc` — write Obsidian documentation note
`obs-not-cfg` — update config/schema in vault
`obs-not-ref` — update reference file in vault

**Pattern**
`obs-not-doc → obs-not-cfg → obs-not-ref` — write doc → update config → update reference

**Flow**
`obs-not-doc → ncl-fil-doc → fla-dis-doc` — write → share to Nextcloud → post to forum

---

### Planning

**Strings**
`llm-tsk-pln` — write task plan
`win-scr-cfg` — configure Windows script/tooling

**Pattern**
`llm-tsk-pln → win-scr-cfg` — plan → implement tooling

**Flow**
`llm-tsk-pln → win-scr-cfg → dol-tic-end` — plan → implement → close ticket

---

### Code & Scripts

**Strings**
`git-rpo-rev` — review code in GitHub repo
`win-scr-cfg` — configure Windows script/tooling
`git-rpo-cfg` — configure repo settings

**Pattern**
`git-rpo-cfg → git-rpo-rev → win-scr-cfg` — set up repo → write code → configure locally

**Flow**
`llm-tsk-pln → git-rpo-rev → cpl-adm-mig

---

### TOGAF Phase

**Strings**
`obs-not-doc` — write TOGAF deliverable in Obsidian
`tog-doc-rev` — review TOGAF deliverable
`fla-dis-doc` — post phase update to forum

**Pattern**
`obs-not-doc → tog-doc-rev → fla-dis-doc` — write → review → publish

**Flow**
`obs-not-doc → ncl-fil-doc → fla-dis-doc → tog-doc-rev → fla-dis-doc` — write → share → post → ABA reviews → post phase complete

---

### Agent Coordination

**Strings**
`dol-tic-end` — create or update agent ticket in Dolibarr
`fla-dis-doc` — post to forum for agents
`fla-dis-rev` — post review/feedback to forum

**Pattern**
`dol-tic-end → fla-dis-doc` — assign ticket → post forum instruction

**Flow**
`llm-tsk-pln → dol-tic-end → fla-dis-doc → fla-dis-rev` — plan → assign → instruct → review agent output

---

### Vault Taxonomy (Meta)

**Strings**
`obs-not-str` — document a string in the vault
`obs-not-pat` — document a pattern in the vault
`obs-not-flo` — document a flow in the vault

**Pattern**
`obs-not-str → obs-not-pat → obs-not-flo` — document string → pattern → flow

**Flow**
`obs-not-str → obs-not-pat → obs-not-flo → obs-not-ref` — build taxonomy → update reference

