# Changelog

Versions match the `version` field in `.claude-plugin/plugin.json` and are tagged in git.

## 1.3.1 — 2026-08-10
- Lookup ladder made DAW-neutral: the DAW map file now declares its DAW name and official documentation source, and the skill reads both from there.

## 1.3.0 — 2026-08-10
- Lookup ladder for unknowns: own references, then the user's screen, then official docs on the web, then an honest "I don't know". Bluffed answers are banned.
- The mentor may offer to correct the DAW map when a real session proves it wrong (only with the user's consent).

## 1.2.1 — 2026-08-10
- Profile migration rule: after any level renumbering, the stored label wins over the stored ID and the mentor fixes the profile silently.

## 1.2.0 — 2026-08-10
- New level L2 "Returning dabbler" (used an older DAW years ago, has not studied music). Previous L2 to L6 renumbered to L3 to L7.

## 1.1.0 — 2026-08-10
- Packaged as a Claude Code plugin marketplace (one-command install).
- Prerequisites extracted into their own reference file; the mentor offers consent-gated installs of missing tools.
- References enriched: low-end rules, key-choice constraint, rule of threes, M3 readiness checks, music theory file, mastering translation section.

## 1.0.0 — 2026-08-10
- Initial release: milestone gates, bounce review, escalation ladder, six levels, bounded two-file memory, Cubase map, install for Claude Code and Codex.
