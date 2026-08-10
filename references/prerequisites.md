# Prerequisites

Checked silently at session start. Surface anything missing in one sentence, state
what degrades, then make the install offer — once per session, never silently, and
never attempt anything needing privileges or a package manager that isn't present:
hand the user the exact command instead.

## Required

| Tool | Why | Install |
|------|-----|---------|
| music-analysis skill | Listening to bounces and reference tracks — the objective half of every review | Copy `plugins/adam-researchh--music-analysis/skills/music-analysis/` from https://github.com/dvcrn/openclaw-skills-marketplace into the skills directory, or `npx skillfish add dvcrn/openclaw-skills-marketplace music-analysis` |
| ffmpeg | All audio handling (bounces, reference conversion) | macOS `brew install ffmpeg` · Windows `winget install ffmpeg` · Linux `sudo apt install ffmpeg` |

**Missing required tool = degraded mode:** say plainly that bounce review falls back
to screenshots + the user's descriptions until it's installed. Never silently
pretend to have heard audio.

**Python deps note:** the music-analysis scripts need `librosa`, `numpy`,
`soundfile`. On externally-managed Pythons (PEP 668 — Homebrew, Debian), install
them into a venv colocated in that skill's folder and run its scripts with the venv
python (check the folder for a LOCAL-SETUP.md). A plain `python3` call failing with
`ModuleNotFoundError: librosa` means exactly this.

## Optional

| Tool | Adds | Install |
|------|------|---------|
| yt-dlp | Reference tracks from URLs | `brew install yt-dlp` / `winget install yt-dlp` / pipx |
| music-generation skill | MIDI teaching artifacts at teaching stage 3 (Assist) | aiskillstore marketplace (`skills/cam10001110101/music-generation`) |
| phantom | Engineering diagnostics (masking, phase, loudness) at M3 | `uv tool install "phantom-audio[all]"` (Python 3.13) |

Mention an optional tool only when the moment would actually use it — never as a
shopping list.
