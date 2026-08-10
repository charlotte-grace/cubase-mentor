# Bounce Review

Evidence priority, always: (1) bounce analysis, (2) screenshots, (3) the user's words.
Ask for a screenshot only when the question is Cubase-mechanics ("show me the insert
chain on that channel"), not as a substitute for listening.

## Procedure

1. The user supplies a bounce (any format ffmpeg reads; short excerpts are fine and
   encouraged pre-M2).
2. Run the music-analysis skill's full listen on the bounce.
3. Build the comparison:
   - **With a reference:** set the bounce's read against the cached
     `<track-name>.reference-analysis.json`. Compare energy contour shape, onset/groove
     character, structural contrast, tension movement, overall timbral brightness.
     NEVER compare BPM as a target — tempo is the user's choice.
   - **Without a reference:** read the bounce absolutely against the intent statement
     in `active-track.md`: does what it does match what they said it should become?
     Plus sanity reads: is there sub-bass at all, does anything clip, is the energy flat?
4. **With phantom installed** (optional provider): add the engineering layer — frequency
   masking flags, phase issues, tonal balance vs reference, loudness. Weight these
   heavily at M3, lightly before it.
5. Pick **exactly one prioritized teaching point** — the single change that most moves
   this bounce toward the current milestone. Everything else you noticed: hold it. It will
   still be true next bounce.
6. Deliver per the teaching stages and the user's skill level: question first at low
   skill levels, verdict first at L7.

## Reading deltas honestly

- The analysis stack's structure labels are similarity labels; its emotion reads are
  explainable proxies. Cite them as evidence, not verdicts. The user's ears outrank
  the numbers when they conflict — say so when it happens.
- Calm/ambient material: BPM and beat-grid numbers are untrustworthy (the tracker
  imposes a metronome). Compare energy, structure, and tension only.
- A bounce that measures "worse" but sounds better to the user at their stated intent
  is a conversation, not a correction.

## The one-teaching-point rule

One point per review. Not two. A list of five fixes teaches none of them.
The point names: what to change, why it matters for the current milestone, and where in
Cubase to do it (cubase-map.md) — depth per level.
