---
tags: [reference, taxonomy, meta]
aliases: [CTF Reference, Categories, Tags, Fields]
role: admin
created: 2026-04-01
status: active
type: reference
---

# CTF Reference — Categories, Tags & Fields

## Conventions

- **Master taxonomy:** the `000XXX` ref codes. The cross-app work-item set is `R`.
- **Label format** (where a label is shown to users): `000XXX — Name` (em dash). Names per Code Reference.

## Per-app current state

### Dolibarr

**Categories** (`llx_categorie`, per object type):

| Object (type) | Holds | Format |
|---|---|---|
| ticket (12) | ref (R) + TOGAF phase/deliverable | `000XXX — Name` (ref) |
| project (6) | ref (R) + TOGAF | `000XXX — Name` (ref) |
| knowledgemanagement (13) | ref (R) | `000XXX — Name` |
| actioncomm (10) | ref | legacy `000XXX - Name` |
| supplier/vendor (1) | ref | contextual |
| customer (2) | ref | contextual |
| contact (4) | ref | contextual |
| product (0) | ref | contextual |
| member (3) | — | contextual |
| website_page (11) | subject tags (WP mirror) | n/a |

**Ticket dictionaries** (drive the ticket-create GUI):
- `c_ticket_type` (**Request Type**) — ref codes, labels `000XXX — Name`, plus `AGENT_TASK / FORUM_POST / WIKI_BLOG`. Dolibarr defaults (COM/HELP/ISSUE/…) inactive.
- `c_ticket_category` (**Ticket Group**) — agent/role codes (separate routing axis).
- `c_ticket_severity` — `BLOCKING HIGH LOW NORMAL`.

**Fields:** `service_code` extrafield (actioncomm) = ref options. Native ticket fields incl. `type_code, category_code, severity_code, fk_project, fk_soc, fk_user_assign`.

### Nextcloud
- **System tags = ref codes only** (no subject vocabulary).
- No category primitive; structure = groups + shared folders. Per-tag fields: `display-name`, `user-visible`, `user-assignable`.

### WordPress
- **Categories** = ref-code top-level + wiki-structure children + `Uncategorized`.
- **Tags** = ref-code + loose subject tags (kept as potential wiki-reference vocabulary).

### Flarum
- **Tags** = TOGAF phase tags + utility (`general tasks announcements dev`). Tags are the category system; no ref codes needed.

### Obsidian *(the master)*
- Frontmatter `tags`: full master ref codes + subject + note-type tags.

### GitHub
- Repos named by ref code. Labels = stock GitHub set only.
