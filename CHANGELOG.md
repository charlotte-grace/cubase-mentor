# Changelog

Versions match the `version` field in `.claude-plugin/plugin.json` and are tagged in git.

## 1.3.2 (2026-08-10)
- Escalation ladder renamed to teaching stages, with four plain-spoken names: Coach, Model, Assist, Answer. Stage numbers and milestone codes (M1–M4) are barred from user-facing speech; the mentor now speaks the substance instead ("your arrangement skeleton is there," not "you've hit M2").
- "Persona" renamed to level throughout; the level table gained a Profile/Field Experience/DAW-Tool Familiarity structure with clearer labels (e.g. "Musical Novice," "DAW Switcher").
- Stored level data renamed from profile block to learner block, resolving a naming collision with the level table's own Profile column.
- Level question now has a plain-text fallback for interfaces that cap how many options a question can show; all seven levels stay equally reachable instead of the last three being demoted to an "other" catch-all.
- Every milestone (not just the rough mix) now has an explicit readiness checklist.
- "Lookup ladder" and "gate" retired in favor of lookup order and milestone, for consistency with the teaching-stage rename.
- SKILL.md readability pass: explained what a route is, removed leftover code-style naming (SKILL_DIR, genre-agnostic) from user-facing prose, and untangled a run-on session-close instruction.

## 1.3.1 (2026-08-10)
- Lookup ladder made DAW-neutral: the DAW map file now declares its DAW name and official documentation source, and the skill reads both from there.

## 1.3.0 (2026-08-10)
- Lookup ladder for unknowns: own references, then the user's screen, then official docs on the web, then an honest "I don't know". Bluffed answers are banned.
- The mentor may offer to correct the DAW map when a real session proves it wrong (only with the user's consent).

## 1.2.1 (2026-08-10)
- Profile migration rule: after any level renumbering, the stored label wins over the stored ID and the mentor fixes the profile silently.

## 1.2.0 (2026-08-10)
- New level L2 "Returning dabbler" (used an older DAW years ago, has not studied music). Previous L2 to L6 renumbered to L3 to L7.

## 1.1.0 (2026-08-10)
- Packaged as a Claude Code plugin marketplace (one-command install).
- Prerequisites extracted into their own reference file; the mentor offers consent-gated installs of missing tools.
- References enriched: low-end rules, key-choice constraint, rule of threes, M3 readiness checks, music theory file, mastering translation section.

## 1.0.0 (2026-08-10)
- Initial release: milestone gates, bounce review, escalation ladder, six levels, bounded two-file memory, Cubase map, install for Claude Code and Codex.
