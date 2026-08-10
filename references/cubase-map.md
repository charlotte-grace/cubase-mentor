# Cubase Map

DAW: **Cubase** (Pro 13/14 naming) · Official documentation for web lookups:
**steinberg.help** (Steinberg's manuals)

Task → where it lives in Cubase. This is the only DAW-specific file in the skill;
swapping it re-targets the mentor to another DAW — a replacement map MUST declare
its own DAW name and official-docs source in this header, because the lookup
order in SKILL.md reads them from here.

| I want to… | In Cubase |
|------------|-----------|
| Sketch chord progressions with help | Chord Track (Project > Add Track > Chord) + Chord Pads (Lower Zone); Chord Assistant suggests next chords |
| Try different arrangements non-destructively | Arranger Track — define A/B/C events, chain them, then Flatten when decided |
| Draw/edit MIDI notes | Key Editor (double-click a MIDI part; Lower Zone or full window) |
| Program drums | Drum Editor (MIDI part > Drum Editor when a drum map is set) or Key Editor |
| Chop and mangle a sample | Sampler Track (drag audio onto Project > Add Track > Sampler) — slice, loop, pitch modes |
| Time-stretch audio to the project tempo | AudioWarp (Sample Editor > Musical Mode) |
| Commit a heavy synth/effect to audio | Render in Place (Edit > Render in Place) |
| Bounce the whole track or a section | Export Audio Mixdown (File > Export); set the range with the Left/Right Locators |
| Mark and export loops/sections | Cycle Markers (Marker Track) — name sections; exportable ranges in Export Audio Mixdown |
| Batch-export stems | Export Audio Mixdown > Channel Selection (choose multiple channels) or Export Queue |
| Find sounds/presets/samples | MediaBay (F5) — tag-based browsing |
| Basic subtractive synth | Retrologue |
| Granular/texture synth | Padshop |
| Sampler/rompler workhorse | HALion Sonic |
| Group related channels for shared processing | Group Channel Track; route channel outputs to it |
| Add a shared reverb/delay | FX Channel Track + Sends on each channel |
| Per-channel EQ | Channel EQ in the MixConsole channel strip, or the Frequency plugin for surgical work |
| Compress a channel | Compressor (strip or insert); Squasher for simple multiband |
| Meter loudness (LUFS/true peak) | SuperVision plugin on the master; Control Room meters |
| Process one clip only, not the channel | Direct Offline Processing (F7) |
| Keep alternate takes/versions of a track | Track Versions (track header dropdown) |
| A/B my mix against a reference file | Import the reference to its own channel routed straight to the master (post-fader listen), or use Control Room Reference feature |
| Save a reusable track setup | Track Presets (right-click track > Save Track Preset) |
| Fix timing of audio hits | Hitpoints in the Sample Editor → slice or quantize |
| Undo mixer moves (not project edits) | MixConsole History tab |
