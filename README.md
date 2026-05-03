# voxhora-public

**Voxhora — App Store edition.** The general-audience version of Voxhora that any attorney can buy and configure for their own jurisdiction, billing rules, and (optionally) practice management software.

## Status

🚧 **Placeholder.** No code yet. This repo exists to reserve the URL and as a destination for ideas as they accumulate.

Coding will start after the Phase 3 soak test on Patrick's personal version (`voxhora-ios` + `voxhora-mac`) confirms the trunk is solid for daily attorney use.

## Architecture target

Single codebase, configuration-driven. The current `voxhora-ios` + `voxhora-mac` repos already use a `Jurisdiction` protocol so Travis County is one implementation among many. The public version extends that with onboarding UI, runtime jurisdiction editing, per-attorney CloudKit, and a generic API-key strategy.

Detailed design lives in the docs repo: `voxhora-docs/Voxhora - Phase 4 Public App Architecture.md`. (Patrick's friend with read access to `voxhora-docs` can see it; everyone with access to this repo can read it via the cross-reference.)

## Sister repos

- [voxhora-ios](https://github.com/SanPatriciodeCuernavaca/voxhora-ios) — Patrick's iPhone app (canonical Travis County implementation)
- [voxhora-mac](https://github.com/SanPatriciodeCuernavaca/voxhora-mac) — Patrick's Mac app
- [voxhora-android](https://github.com/SanPatriciodeCuernavaca/voxhora-android) — Android port (sister builds out)
- [voxhora-docs](https://github.com/SanPatriciodeCuernavaca/voxhora-docs) — Obsidian design canon (DA Log, handoffs, playbook, IP doc, this design's Phase 4 doc)

## How to add ideas while soak-testing

Patrick or his Claude can drop ideas into `~/Obsidian/Voxhora/Voxhora - Phase 4 Public App Architecture.md` whenever they pop up. They'll auto-sync to the `voxhora-docs` repo on GitHub. When soak-test ends and we're ready to start building, the design doc is the launching point.
