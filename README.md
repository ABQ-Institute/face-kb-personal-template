# Your Personal Knowledge Base (FACE L0)

> Your career-wide, portable knowledge base — built on
> [ABQ's FACE](https://abq.institute/face). **You own it.** It follows you from
> job to job; employers connect to slices of it and lose access when you part
> ways — never the other way around.

This KB is yours and it is ready to use. Nothing here needs configuring before
you start writing.

## The two domains

```
🏠 PERSONAL — never leaves this KB
├── 1-brain/          expertise, judgment style, heuristics, learnings
└── 2-workspace/      notes, contacts, personal projects, working memory

💼 PROFESSIONAL — shareable with company agents, per YOUR grant
├── 3-professional/   curated expertise you offer to company agents
├── 4-credentials/    career history, certifications, attestations
└── 5-marketplace/    skill cards and AI skills you offer publicly

access.yaml           the exposure rules — you own them
```

The boundary that matters: a **company agent** (your employer's) can use your
*professional* folders — but only through a grant you give in
[access.yaml](access.yaml) (managed visually in FACE Studio → Connections),
revocable by you at any time. Your *personal* folders are structurally
non-grantable: FACE Studio refuses to expose them no matter what.

## Start here

The KB is empty until you put yourself in it. In rough order of payoff:

1. **[Judgment Style](1-brain/1-judgment-style.md)** — how you decide and what
   you optimise for. Highest impact by far: it's what makes an agent act like
   *you* rather than like a generic assistant.
2. **[Methods & Heuristics](1-brain/2-methods-and-heuristics.md)** — your
   working methods and rules of thumb.
3. **[Expertise Profile](3-professional/1-expertise-profile.md)** — the
   curated version you're willing to share with an employer's agents.

Write in your own words, in whatever language you think in. Short and true
beats long and tidy — you can always come back.

## What goes where

| I want to write down… | It goes in… |
|---|---|
| How I make decisions, my heuristics, lessons learned | [1-brain/](1-brain/README.md) |
| Notes, people I know, side projects, running memory | [2-workspace/](2-workspace/README.md) |
| Expertise I'm happy for my employer's agents to use | [3-professional/](3-professional/README.md) |
| CV facts, certifications, employer attestations | [4-credentials/](4-credentials/README.md) |
| Skills I offer publicly (skill cards) | [5-marketplace/](5-marketplace/README.md) |

Configuration — your name, language, owner — lives in
[0-meta/](0-meta/README.md); it is already filled in.

## Working with it

- **In FACE Studio** (`/me/kb`) — visual editor, grant management, and search.
- **From your own AI agents** — every folder has a README, and
  [AGENTS_BOOT.md](AGENTS_BOOT.md) boots any coding agent against this KB.

## Learn more

- Framework definition: FACE §3.23 — Personal KB Layer (L0)
- The template family: company · department · project · **personal** (this one)

## Created this copy outside FACE Studio?

FACE Studio does the following for you when it creates your KB at `/me/kb`. If
you instead used GitHub's **Use this template** button yourself, do them once:

1. Set the repository's visibility to **Private**. The template is public; your
   copy holds your professional brain and your working notes.
2. Name the repository `kb-personal`.
3. Fill in the `TODO` values in [0-meta/kb-config.yaml](0-meta/kb-config.yaml).
