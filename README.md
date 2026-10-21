# Structure AI (SAI)

Structure AI is a structure methodology for AI agents, includes the **Crowned Model** and **Framework AI (FAI)**. This repository is an [Obsidian](https://obsidian.md) vault that defines the reference-code taxonomy and folder structure from which the operational vault is derived.



## Inside SAI

An environment — each level lives inside the one above it:

1. **System (SYS)** — user device
2. **Platforms (PLA)** — Windows (WIN) install and cPanel (CPL) web-hosting plan
3. **Frameworks (FRA)** — FAI (the reference-code framework), TOGAF (TOG), Blockchain (BCH), Kubernetes (K8S)

### Framework AI (FAI)

**Folders**

- **Organization (ORG)**
  - **Governance (GOV)**
  - **Operations (OPS)** → Agents (AGT) → Code (COD), Integrations (ITG), Personas (PER), Skills (SKI), Workflows (WFL); Business Units (BUS)
  - **Wiki (WIK)** → Applications (APP), Knowledge Bases (KBS)

**Files**

| File | Code | Contents |
|------|------|----------|
| `COD.md` | COD | App codes, app objects, object types |
| `CTF.md` | CTF | Categories, tags, fields |
| `SPF.md` | SPF | Strings, patterns, flows |

## Conventions

- **Folders:** bare 3-letter uppercase code (e.g. `DOL`)
- **Node file:** each ref-code node holds one summary file named after its lowercase code (e.g. `dol.md` under `DOL`)
- **Content prefix pattern:** `{CODE}-{qualifier}` → `WOR-PGT-CAS` = WordPress page for Customer & Sales
- **Hierarchical doc refs (body only, never as tags):** `WPS-DOL-BUS-ICS` chains codes with `-`; tags stay flat (`WPS`, `BUS`)
- **Frontmatter:** include the reference code as a tag, e.g. `tags: [dolibarr, DOL, config]`

## Repository layout

```
000SAI/
├── SAI.md                          Vault root — methodology overview
├── Crowned_Model.png               The Crowned Model diagram
└── SYS/                            System (user device)
    └── PLA/                        Platforms
        ├── CPL/                    cPanel (web hosting)
        └── WIN/                    Windows (local machine)
            └── FRA/                Frameworks
                ├── BCH/            Blockchain
                ├── FAI/            Framework AI (reference-code framework)
                │   ├── COD.md      Code reference
                │   ├── CTF.md      Categories, tags & fields
                │   ├── SPF.md      Strings, patterns & flows
                │   └── ORG/                Organization
                │       ├── GOV/            Governance
                │       ├── OPS/            Operations
                │       │   ├── AGT/        Agents
                │       │   │   ├── COD/    Code
                │       │   │   ├── ITG/    Integrations
                │       │   │   ├── PER/    Personas
                │       │   │   ├── SET/    Setup
                │       │   │   ├── SHA/    Shares
                │       │   │   ├── SKI/    Skills
                │       │   │   └── WFL/    Workflows
                │       │   └── BUS/        Business Units
                │       └── WIK/            Wiki
                │           ├── APP/        Applications
                │           └── KBS/        Knowledge Bases
                ├── K8S/                    Kubernetes
                └── TOG/                    TOGAF (enterprise architecture)
```

---

Created and maintained by Nathan Livingstone.
