# rlv-code

Engineering hub for RL Ventures LLC. Single-file static HTML companion to [rlv-lol](../rlv-lol/) (business/LLC landing).

- **Live:** https://code.rlv.lol (target — not yet configured)
- **Source:** `index.html` — single file, no build step
- **Aesthetic:** IBM Plex Mono + warm accent, mirrors rlv-lol

## Content

- **Now** — what's actively shipping this week
- **Projects** — curated engineering portfolio (Stull Atlas, Orton Cone Sim, Ceramic Engine, Crystal VR, minarealm, Howell Brain, ConduitBridge, myclaystudio)
- **Engineering Principles** — verify / local-first / boring-version / ground-the-abstract
- **Stack** — languages, web, backend, compute, dev loop, AI
- **Contact** — consulting pitch

## Deploy

Two options — decide when DNS is picked:

1. **Porkbun Static + subdomain `code.rlv.lol`** — add `_deploy.py` mirroring the minarealm / cuub.help ftplib.FTP_TLS pattern. Requires Porkbun to host `rlv.lol` (currently appears to point elsewhere — verify before wiring).
2. **GitHub Pages + CNAME** — `CNAME` file already contains `code.rlv.lol`. Push to a `gh-pages` repo under `rlv-ventures` org, enable Pages.

Domain decision deferred — author was AFK at scaffold time. Default choice recorded: `code.rlv.lol` subdomain.

## Relationship

```
RL Ventures LLC
├── rlv-lol/       LLC hub · rlventures.com         (business)
└── rlv-code/      engineering index · code.rlv.lol (this repo)
```

## Gotchas

- `index.html` hardcodes live numbers (12,880 glazes, 1302.34 °C, 314 Lean proofs, 99 KG entities) — these are accurate as of Apr 23, 2026 per user memory. Re-verify before each redeploy.
- No `brain/` gated dashboard like rlv-lol — this repo is fully public.
