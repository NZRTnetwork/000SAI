---
tags:
  - reference
  - meta
  - taxonomy
  - SAI
  - VLT
aliases:
  - Structure AI
  - SAI
role: admin
created: 2026-04-01
status: active
type: reference
---

# Structure AI (SAI)

Structure AI is a structure methodology for AI agents, includes the Crowned Model and Framework AI (FAI). The SAI folder is an Obsidian (OBS) vault (VLT) — folders use bare `XXX` code naming.

Each ref-code node holds a single summary file named after its lowercase code (e.g. `win.md` under WIN, `dol.md` under DOL) — a condensed reference of what is actually used/configured for that node, not general product documentation.

## Crowned Model

The SAI node essentials.

![[CDM-IMG.png]]

| # | Code | Name | Type | Node |
|---|------|------|------|------|
| 1 | CPL | cPanel | PLA | Web-hosting platform |
| 2 | RPO | Repositories | — | `RPO-SAI` → GitHub |
| 3 | OBS | Obsidian | APP | Markdown notes app — the vault `VLT-SAI` |
| 4 | WOR | WordPress | APP | CMS — public website, centre |
| 5 | NCL | Nextcloud | APP | File storage and collaboration |
| 6 | EXT | External / extras | — | FLA (Flarum) and extras |
| 7 | DOL | Dolibarr | APP | ERP / CRM — tickets, tags |

## Triad

Three roots.

![[TRI-IMG.png]]

| Code | Name | Root | Holds |
|------|------|------|-------|
| CBR | Chamber | `C:\CBR-SAI` | Concept files (`*-cpt.html`) and credentials |
| VLT | Vault | `C:\VLT-SAI` | Knowledge — the Obsidian (OBS) vault |
| RPO | Repositories | `C:\RPO-SAI` | Code — mirrored to GitHub |

## Structure

An environment — each level lives inside the one above it.

1. **System (SYS)** — user device
2. **Platforms (PLA)**
   - cPanel (CPL) — web-hosting plan
   - Windows (WIN) — local machine
3. **Frameworks (FRA)** — installed under Windows (WIN)
   - FAI — reference-code framework (part of SAI)
   - TOGAF (TOG) — enterprise architecture
   - Blockchain (BCH), Kubernetes (K8S)

### FAI folders

- **(a) Organization (ORG)**
  - **(a1) Governance (GOV)**
  - **(a2) Operations (OPS)**
    - **(a2a) Agents (AGT)** — tasker agents, each with a distinct function — Integrations (ITG), Personas (PER) incl. each agent's Code Portfolio, Skills (SKI)
    - **(a2b) Business Units (BUS)**
  - **(a3) Wiki (WIK)**
    - **(a3a) Applications (APP)** — each holds a single summary file
    - **(a3b) Knowledge Bases (KBS)**

### FAI files

- **(1) COD** — App Codes, App Objects, Object Types — [[COD]]
- **(2) CTF** — Categories, Tags, Fields — [[CTF]]
- **(3) SPF** — Strings, Patterns, Flows — [[SPF]]

---

Nathan Livingstone is the creator and developer of this vault and documentation.
