# Memory Contract

All memory lives in `progress_dir` (from `config.yaml`). Exactly two live files,
one archive folder, and cached analysis JSON. Nothing else is ever written.
Growth is structurally capped: templates are overwritten in place, never appended forever.

## `active-track.md` — one track's state, overwritten at every session close

```markdown
# Active track: <track-name>

- **Target:** <reference: path + one-line stated goal | intent: the written intent statement>
- **Reference analysis:** <path to cached JSON, or "none — intent-driven">
- **Milestone:** <M1|M2|M3|M4> — <one line: what passing looks like for THIS track>
- **Last bounce verdict:** <the one teaching point, or "no bounce yet">
- **Decisions:** <bullet list, pruned to what still matters — max 10 lines>
- **Next action:** <exactly one>
- **Next up (parked):** <one line, or empty>
```

On M4 pass: move to `archive/<track-name>.md`, start fresh.
On track switch: move to `archive/<track-name>-shelved.md` and append a resume block:

```markdown
## Shelved <YYYY-MM-DD>
- **At milestone:** <M#>
- **What was hard:** <one honest line — the answer to the switch question>
- **Resume note:** <one line: where to pick up>
```

Resuming a shelved track: move the file back to `active-track.md`, re-enter at the saved milestone.

## `concepts.md` — profile block + concept table

```markdown
# Profile
- **Level:** <L1–L6> — <label from levels.md>
- **Set:** <YYYY-MM-DD>  **Updated:** <YYYY-MM-DD>
- **Note:** <one optional line, e.g. "strong ears, DAW-new">

# Concepts
| Concept | Status | Last touched | Hook |
|---------|--------|--------------|------|
| <name> | introduced / shaky / clicked | <YYYY-MM-DD> | <one line> |
```

Session open: glance at `shaky` rows; weave ONE into the work when natural — never as a quiz.
Pruning: `clicked` and untouched for three consecutive sessions → delete the row.
(Optional practice for knowledge-base keepers: flush pruned concepts into your own
notes before deleting. This is documentation, not protocol.)

## Cached reference analysis

At intake with a reference, store the music-analysis JSON as
`<track-name>.reference-analysis.json` in `progress_dir`. Analyze once; never re-run
for the same reference.

## Shelf count

At session open, if `archive/*-shelved.md` files exist, name the count in one clause
("two tracks shelved") — visibility, never a lecture.
