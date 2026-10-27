# My Personal KB

Everything your own agent knows about you — your life and your work — in one private repo on your GitHub account. Folders are grouped by who can see them. Nothing moves between groups without you.

## Only you

Your life, how you think, your position in each organisation, your working notes. Never shared — no grant can name these folders.

Folders: [`1-life`](1-life/README.md) (Life) · [`2-brain`](2-brain/README.md) (How you think) · [`3-orgs`](3-orgs/README.md) (Your organisations) · [`4-workspace`](4-workspace/README.md) (Workspace)

## Whoever you grant

What a company's agents may use as context — folder by folder, only after you grant it, revocable any time.

Folders: [`5-professional`](5-professional/README.md) (Professional) · [`6-credentials`](6-credentials/README.md) (Credentials)

## Anyone

What you offer publicly. Public serving isn't live yet — until it is, this folder is shared only by grant, like the ones beside it.

Folders: [`7-marketplace`](7-marketplace/README.md) (Marketplace)

## Sealed folders

`1-life/3-health` is sealed: it will be encrypted on your own devices, so neither GitHub nor ABQ can read it. Sealing isn't available yet, so a sealed folder accepts no writes for now — keep those notes where they are today.

## How things get here

Your agent turns what you give it — a journal entry, a check-in, a transcript — into changes across these folders. Those that pass every check publish on their own; anything shared, anything in `2-brain` and anything unusual waits for you under Change requests.

---

## Working with it

- **In FACE Studio** (`/me/kb`) — visual editor, grant management, and search.
- **From your own AI agents** — every folder has a README, and
  [AGENTS_BOOT.md](AGENTS_BOOT.md) boots any coding agent against this KB
  ([CLAUDE.md](CLAUDE.md), [AGENTS.md](AGENTS.md) and [GEMINI.md](GEMINI.md)
  point to it).

Configuration — your name, language, owner, sealed folders — lives in
[0-meta/](0-meta/README.md); who may use what lives in [access.yaml](access.yaml).

## Created this copy outside FACE Studio?

FACE Studio does the following for you when it creates your KB at `/me/kb`. If
you instead used GitHub's **Use this template** button yourself, do them once:

1. Set the repository's visibility to **Private**. The template is public; your
   copy holds your life, your professional brain and your working notes.
2. Name the repository `kb-personal`.
3. Fill in the `TODO` values in [0-meta/kb-config.yaml](0-meta/kb-config.yaml).
