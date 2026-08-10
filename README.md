# cubase-mentor

An agent skill that acts as an expert music-production mentor teaching through Cubase. It coaches you from an 8-bar loop to a finished, rendered track — measured against a reference track you supply or an intent you state — and answers standalone Cubase and production questions in between. Genre-agnostic by design: your reference carries the taste, the skill carries the craft.

Works in Claude Code and OpenAI Codex CLI. Pure markdown — no server, no scripts.

## What it does

- **Milestone gates**: 8-bar core loop → arrangement skeleton → rough mix → done-enough bounce. Gates pass on bounced audio evidence, not good intentions. It will name your scope creep and park it.
- **Bounce review**: analyzes your exported audio, compares it to your reference (or reads it against your stated intent), and gives you **exactly one** teaching point per bounce.
- **Escalation ladder**: question → concept → teaching artifact → exact settings. It guides; it never does the work for you, and it never touches your project.
- **Level-aware**: on first run it asks where you are (six personas, from complete beginner to producer-switching-DAWs to advanced) and tailors vocabulary, patience, and directness to match.
- **Track switching is never refused** — it just asks one honest question and shelves your current track resumably.
- **Quick-question mode**: "where do I chop a sample?" gets a direct answer, no ceremony.

## Install

Claude Code:

```bash
git clone https://github.com/charlotte-grace/cubase-mentor ~/.claude/skills/cubase-mentor
```

Codex CLI (restart Codex afterwards):

```bash
git clone https://github.com/charlotte-grace/cubase-mentor ~/.codex/skills/cubase-mentor
```

Invoke with `/cubase-mentor` (Claude Code) or `$cubase-mentor` (Codex), or just start talking about your track — the description triggers it.

Update later with `git pull` in the same folder.

### No git? Two easier ways

**Let your agent install it** (you're installing an agent skill, so you have one) — paste this into Claude Code:

> Install the skill from https://github.com/charlotte-grace/cubase-mentor by cloning it into ~/.claude/skills/cubase-mentor

**Or download manually:** the green **Code** button above → **Download ZIP** → unzip → rename the folder from `cubase-mentor-main` to `cubase-mentor` → move it into `~/.claude/skills/` (macOS Finder: Cmd+Shift+G, type `~/.claude/skills`). The folder name must be exactly `cubase-mentor`. To update, re-download the ZIP.

## Prerequisites

| Tool | Needed for | Required? |
|------|-----------|-----------|
| [music-analysis skill](https://mcpmarket.com/tools/skills/music-analysis-audio-intelligence) | listening to your bounces and reference tracks | **Yes** — without it, feedback degrades to screenshots + your descriptions |
| ffmpeg | audio handling | **Yes** |
| yt-dlp | reference tracks from URLs | Optional |
| music-generation skill | MIDI teaching examples | Optional |
| [phantom](https://github.com/fadelabs/phantom) | engineering diagnostics (masking, phase, loudness) at the mix stage | Optional |

## Configuration

`config.yaml`:

```yaml
progress_dir: ./cubase-mentor-data
```

`progress_dir` is where the mentor keeps its memory — two small files (your active track's state and a concept-tracking table) plus an archive of finished and shelved tracks. Point it anywhere; a folder in your notes system works well.

## Using it with another DAW

`references/cubase-map.md` is the only Cubase-specific file. Replace it with an equivalent map for your DAW and the rest of the skill follows.

## Acknowledgements

Parts of the reference knowledge are distilled from community resources, including [music-chips.com](https://music-chips.com/) (Apache-2.0).
