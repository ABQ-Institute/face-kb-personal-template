# Personal Knowledge Base — Agent Instructions

> Built on ABQ's FACE. Skills are served centrally and are always current.
> This is a **Personal KB (L0)** — it belongs to one individual, not to a company.

## Boot

Read `0-meta/kb-config.yaml` (identity, language) and `access.yaml` (exposure rules).

## Load the FACE skills (one call, cache for the session)

Fetch this ONCE at the start of your session and keep it in context — do **not**
re-fetch per operation:

    https://face.abq.institute/api/skills/face-kb/bundle?platform=git

It returns the full skill set in one document. The response is version-stamped
(`ETag` and `X-Skills-Version`). Re-fetch only when a new session starts or you
learn the version changed; a conditional request (`If-None-Match: "<version>"`)
returns `304 Not Modified` when it is unchanged.

(API agents: `curl` it. Web tools: open the URL and paste the contents in.)

## This KB groups its folders by who can see them — treat them differently

| Group | Folders | Rule |
|---|---|---|
| **Only you** | `1-life/`, `2-brain/`, `3-orgs/`, `4-workspace/` | **Never leaves this KB.** Do not quote, summarise, or copy its content into any company KB, external message, or shared surface. |
| **Whoever you grant** | `5-professional/`, `6-credentials/` | May be exposed to company agents — but **only** via FACE Studio grants declared in `access.yaml`, never by you directly. |
| **Anyone** | `7-marketplace/` | Meant to be served publicly; until public serving exists, shared only by grant, like the folders above. |

You are the *individual's own* agent. Company agents never read this repo:
they receive granted professional folders through the FACE Studio broker.
The non-grantability of `1-life/`, `2-brain/`, `3-orgs/` and `4-workspace/`
is enforced by Studio's grant schema — but respect it at your layer too:
defence in depth.

## Non-negotiable rules

- Never write directly to `main`. All changes go through a branch + PR
  (the owner is their own reviewer — FACE Studio offers one-click merge).
- Exception: `access.yaml` edits made through FACE Studio's Connections UI
  land as direct commits (a revocation must take effect immediately).
- Never copy Only-you content (`1-life/`, `2-brain/`, `3-orgs/`, `4-workspace/`) outside this KB.
- Write KB content in the language set in `kb-config.yaml`.

---
*Skill content lives in FACE Studio (served at /api/skills/*), not in this file.*
*Framework definition: FACE §3.23 Personal KB Layer (L0).*
