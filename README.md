# cubase-mentor

An agent skill that acts as your music production mentor inside Cubase. It coaches you from a first loop to a finished track, reviews the audio you export, and answers any Cubase or production question. It works in Claude Code and in Codex.

No genre is built in. You give it a reference track (or describe what you want to make) and it measures your progress against that.

## What it does

- **Coaches real tracks.** Four milestones: an 8-bar loop, a full arrangement, a rough mix, a finished bounce. You make every creative decision. It keeps you moving toward done.
- **Listens to your exports.** Upload a bounce and it analyses the audio, compares it to your reference, and gives you one clear thing to improve. Not a list, one thing.
- **Teaches at your level.** On first use it asks where you are (seven options, from complete beginner to advanced) and adjusts its language and patience to match.
- **Helps without taking over.** It asks questions first, explains concepts second, and only hands you exact settings when you are stuck and ask. It never edits your project.
- **Lets you switch tracks.** Want to start something new mid-project? It asks one honest question, shelves your current track so you can resume it later, and moves on with you.
- **Answers quick questions.** "Where do I chop a sample?" gets a direct answer, no ceremony.

## Install

**Claude Code** (one command):

```
/plugin install github:charlotte-grace/cubase-mentor
```

**Codex CLI** (one command, then restart Codex):

```bash
npx skills add charlotte-grace/cubase-mentor -g -a codex
```

**Codex in the ChatGPT desktop app** (no terminal needed). Paste this into Codex:

> Install a skill for me: clone https://github.com/charlotte-grace/cubase-mentor into ~/.codex/skills/cubase-mentor and confirm SKILL.md is there.

Then quit and reopen the app.

**Manual, any harness:**

```bash
git clone https://github.com/charlotte-grace/cubase-mentor ~/.claude/skills/cubase-mentor   # Claude Code
git clone https://github.com/charlotte-grace/cubase-mentor ~/.codex/skills/cubase-mentor    # Codex
```

**No git at all:** use the green **Code** button above, choose **Download ZIP**, unzip, rename the folder to exactly `cubase-mentor`, and move it into `~/.claude/skills/` or `~/.codex/skills/`.

To update later: run `git pull` in the skill folder, or reinstall the same way you installed.

## First run

1. It asks your level (once, never again).
2. It checks its audio tools. If something is missing it offers to install it. Say yes and it handles the rest.
3. Tell it what you are working on, or hand it a reference track.

## What it needs

| Tool | Used for | Required? |
|------|----------|-----------|
| [music-analysis skill](https://github.com/dvcrn/openclaw-skills-marketplace) | listening to your bounces and references | Yes. Without it, feedback relies on screenshots and your descriptions. |
| ffmpeg | audio file handling | Yes |
| yt-dlp | reference tracks from URLs | Optional |
| music-generation skill | MIDI examples to study | Optional |
| [phantom](https://github.com/fadelabs/phantom) | mix diagnostics (masking, phase, loudness) | Optional |

The skill offers to install all of these for you on first run. It only installs after you say yes.

## Configuration

`config.yaml` has one setting that matters:

```yaml
progress_dir: ./cubase-mentor-data
```

This is where the mentor keeps its memory: your active track's state, a small table of concepts you have covered, and an archive of finished and shelved tracks. Point it at any folder you like.

## Using another DAW

`references/cubase-map.md` is the only Cubase-specific file. To retarget the mentor, replace it with a map for your DAW. Your replacement must declare the DAW name and its official documentation site in the header, because the skill reads both from there.

## Acknowledgements

Parts of the reference knowledge are distilled from community resources, including [music-chips.com](https://music-chips.com/) (Apache-2.0).
