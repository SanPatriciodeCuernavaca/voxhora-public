# voxhora-public

Marketing website + signup form for [Voxhora](https://voxhora.app) — voice-first hourly billing for attorneys.

Hosted at **https://voxhora.app** via GitHub Pages. Source = static HTML + CSS, no framework, no build step. `git push main` is the deploy.

## Repurposed 2026-05-19

This repo was originally reserved for a "Phase 4 App Store edition" of Voxhora (a generic, configurable version any attorney could buy). That concept was superseded — `voxhora-ios` + `voxhora-mac` are themselves shipping publicly via TestFlight + Sparkle, with jurisdiction support pluggable in the existing codebase rather than as a separate "public edition" fork.

This repo now serves Phase 2 of the [Distribution and Public-Launch Plan](https://github.com/SanPatriciodeCuernavaca/voxhora-docs) (see `voxhora-docs/Voxhora - Distribution and Public-Launch Plan 2026-05-19.md`): the marketing website that attorneys land on to download Mac or request iPhone access.

## Structure

| File | Purpose |
|---|---|
| `index.html` | Landing page with motto + value props |
| `download.html` | Mac DMG download + install instructions (links to voxhora-mac GitHub Releases) |
| `request-access.html` | TestFlight invite request form (mailto: based; Phase 3 swaps for Cloudflare Worker + ASC API) |
| `setup.html` | First-install walkthrough per platform |
| `whats-coming.html` | Roadmap + release cadence + contact |
| `privacy.html` | Privacy policy (beta version) |
| `terms.html` | Terms of service (beta version) |
| `styles.css` | All styling. Voxhora brand: voxPaper #faf8f3, voxInk #1a2f4a, voxGold #b08d57. Lora serif headlines, system sans body. |
| `favicon.svg` | V mark in voxGold on voxPaper |
| `CNAME` | `voxhora.app` — tells GitHub Pages what custom domain to serve at |

## Local preview

```
cd ~/voxhora-public
python3 -m http.server 8000
open http://localhost:8000
```

## Distribution Phase context

- **Phase 1 — Sparkle for Mac** — shipped 2026-05-19 (see voxhora-mac repo).
- **Phase 2 — voxhora.app signup website MVP** — this repo, 2026-05-19.
- **Phase 3 — Automated TestFlight invites** — Cloudflare Worker + App Store Connect API (next).
- **Phase 4 — How-to video library** — ongoing.
- **Phase 5 — Path D pre-public-launch hardening** — i18n, a11y, App Store screenshots, multi-jurisdiction.

## Sister repos

- [voxhora-ios](https://github.com/SanPatriciodeCuernavaca/voxhora-ios) — iPhone / iPad / Watch (canonical app source) — private
- [voxhora-mac](https://github.com/SanPatriciodeCuernavaca/voxhora-mac) — Mac (Sparkle distribution) — public
- [voxhora-docs](https://github.com/SanPatriciodeCuernavaca/voxhora-docs) — Obsidian design canon (DA Log, handoffs, playbook, distribution plan)
- [voxhora-android](https://github.com/SanPatriciodeCuernavaca/voxhora-android) — Android port placeholder
