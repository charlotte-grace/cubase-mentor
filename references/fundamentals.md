# Production Fundamentals

The teaching base for concept explanations (teaching stage 2, Model). Distilled, opinionated,
genre-free. Teach one section at a time, never the file.

## Sound selection

The mix starts at the sound you pick, not the processing you apply. A well-chosen
sample or patch needs almost nothing; a badly chosen one cannot be EQ'd into being
right. If a sound needs more than ~6 dB of corrective EQ, stop and pick a different
sound. Audition candidates IN the track, not solo'd — the right sound in isolation
is often wrong in context, and vice versa. Fewer, better-chosen elements beat many
mediocre ones stacked. When layering for fullness, give each layer one job and one
range (sub / body / top) — layers that overlap fight, and you're back to EQ surgery
you didn't need.

## Gain staging

Keep channel averages around −18 dBFS; peaks well under 0. Loudness comes at the END
(M4/master), never from pushing channels. If a mix feels quiet, turn the monitors up,
not the faders. Headroom is where a mix breathes; clipping on the way in cannot be
fixed later.

## EQ

Subtractive first: cut what masks before boosting what's missing — cuts clean,
boosts colour. Rough map (guides, not laws):
- 20–60 Hz: sub. Feel more than tone. High-pass what doesn't need it.
- 60–250 Hz: body and warmth. Too much = boom.
- 250–500 Hz: mud lives here. First place to cut when things blur.
- 2–5 kHz: presence and attack. Ears are most sensitive here — small moves.
- 5–10 kHz: edge/harshness below, air above.
One instrument owns a range at a time; two fighting for the same range is an
arrangement problem before it is an EQ problem.

## Low end

The hardest part of most mixes, so it gets its own rules:

- **The sub has a playable range.** Fundamentals around E1–G1 (~41–49 Hz) reproduce
  on most systems; D1–Eb1 are acceptable; much below that most systems cannot
  reproduce the note at all, and much above the sub sounds thin. This constrains
  KEY CHOICE — see the theory reference.
- **Starting balance, then ears:** kick around −6 dB on the meter, bass sitting
  −12 to −15 relative to it. Loop the reference's kick+bass section and measure the
  same relationship there before trusting any numbers.
- **The sub moves slower than the bass.** A busy bassline over a sub holding long
  notes on the fundamental reads as one fat instrument; a sub copying every 16th
  reads as mud.
- **Kick tail length is a groove decision:** roughly 25–50% of the bar. Longer
  fights the bass; shorter leaves a hole.
- **Mono below ~120 Hz, and check phase** between kick, bass, and sub — an out-of-
  phase pair cancels exactly where the power should be.

## Compression

A compressor turns dynamics into density. Four controls that matter first:
threshold (when), ratio (how much — 2:1 gentle, 4:1 firm, 8:1+ is an effect),
attack (slow lets transients through = punch; fast clamps them = smooth),
release (time it lets go — too fast pumps, too slow chokes).
Starting point for almost anything: 3:1, medium attack, release timed so the meter
returns to zero on the beat, 2–4 dB of gain reduction. Adjust by ear from there.

## Saturation

Saturation adds harmonics — perceived loudness, warmth, and presence without adding
level. It is the tool that makes a sound feel *dense* where compression makes it
feel controlled. Three jobs it does that nothing else does as well: makes bass
readable on small speakers (the added harmonics carry the pitch when the sub can't
be reproduced), glues sterile digital sources, and pushes an element forward without
a fader move. Apply in small amounts at several stages rather than one big smash;
the type (tape, tube, soft-clip) matters far less than the amount when starting out.
If everything is saturated, nothing is — contrast is the point.

## Carving space in time (sidechain ducking)

Two elements fighting for the same range can share it by taking turns instead of
being EQ'd apart. Duck one under the other: a compressor on the bass, triggered by
the kick, with fast attack and release timed to the tempo, lets the kick punch
through and the bass breathe back in between hits. The same move at lower intensity
tucks pads and atmospheres under lead elements. When both elements genuinely need
the same frequencies, carving in time beats carving in frequency — an EQ cut is
permanent, a duck only exists when the conflict does. Overdone, ducking becomes an
audible pumping rhythm of its own; that's a creative choice — make it on purpose,
not by accident.

## Space (reverb & delay)

Space is depth: dry = close, wet = far. Choose ONE main space per section and send
instruments into it at different amounts rather than a different reverb per channel.
Pre-delay separates the source from its tail (keeps clarity). Delays in tempo
divisions add size without wash. If the mix blurs, the space is too long or too loud —
tails must fit the gaps.

## Stereo

Anchor low end in mono — sub and kick centred, always. Place other elements
deliberately (think Left-Centre-Right, not a smear). Width is contrast: something
must stay narrow for wide to read. Check the mix in mono once per session; what
disappears in mono has a phase problem.

## Groove

A perfectly quantised grid reads as mechanical because it is. The cheapest humanity
is velocity variation: no two consecutive hits at the same velocity, accents on the
beats that matter, ghost notes (very low velocity hits) filling between. Swing moves
every second subdivision late by a controlled amount — small values change feel long
before they're consciously audible. Keep the anchors (kick, downbeats) on the grid
and let everything else drift slightly; groove is a stable skeleton with loose flesh.
Repetition with tiny variation is the engine: clone the loop, then change one hit
per bar.

## Movement & automation

A static mix dies over three minutes even when every element is right. Automation is
what arrangement feels like inside a section: a filter slowly opening across eight
bars, a send creeping up before a transition, width narrowing into a drop and
snapping wide after. Rule of thumb: at least one parameter moving per section, and
builds made of *motion* (rising filter, tightening delay) read stronger than builds
made only of added elements. Automate the mix last — movement applied to a broken
balance just moves the brokenness.

## A theory floor

Enough theory to make choices on purpose: pick a key and stay in it until leaving is
a decision. The minor scale is the common default and nothing is wrong with staying
inside it for a long time. Bass on the root is always safe; root–fifth–octave is a
bassline before any melody exists. Chords create tension by moving away from the
home chord and resolution by returning — a two-chord loop (home ↔ away) is a
complete harmonic engine. Melody: repetition with ONE change per phrase beats
constant novelty; the ear wants to predict and be slightly wrong. When stuck, use
the DAW's chord tools to explore — then delete the training wheels once the part
exists.

## Critical listening

Solo lies. A sound only matters as heard in context — judge and process with the
track playing, solo only to hunt a specific defect. Ears recalibrate fast: twenty
minutes loud and everything sounds balanced whether it is or not — work at moderate
level, check loud briefly, break often. Before touching any control, name what's
wrong in words ("the bass is masking the kick", "the top end is harsh at 4k") — if
it can't be named, the move is a guess, and articulating it is how the naming gets
easier. Volume-match every before/after comparison; the louder version always wins
otherwise.

## Loudness

Targets are for the FINAL bounce only, and the number follows the destination.
Streaming platforms normalise playback to around −14 LUFS integrated — mastering
louder there just gets turned down. Tracks destined for DJ or club play meet no
normalisation at all: master those to the *measured* loudness of the reference
track (one loudness pass on it — never guess), or the track vanishes next to
everything played beside it. True peak under −1 dBTP either way. Do not chase
loudness while writing or mixing — a dynamic rough mix at −20 LUFS is healthier
than a squashed one at −10. Loudness is the last decision, not a mixing style.

## Translation

A finished bounce must survive systems that cannot reproduce it: cars, phone
speakers, earbuds over Bluetooth, club rigs that sum everything to mono. Most
translation is decided in the MIX — mastering cannot un-collide a kick and bass.

- **Mono fold-down = the club check.** Fold the bounce to mono; whatever
  disappears had a phase problem (widened bass, dual-mono effects, wide synths).
  Below ~120 Hz stays mono; one element owns the sub at a time.
- **Small speakers reproduce no sub** — the bass reads there only through its
  harmonics. Saturate the bass so energy exists an octave or two up and the ear
  reconstructs the fundamental. A pure-sine bassline doesn't exist on a phone.
- **A/B against the reference at matched loudness, always.** Louder always
  sounds better; unmatched comparisons measure volume, not quality. Compare
  tonal tilt, low-end weight, transient feel.
- **Keep 2–5 kHz slightly polite** — cheap speakers exaggerate exactly that band.
- **The listening protocol:** work on the most familiar system, check at low
  volume, bounce a 128 kbps preview and audition over Bluetooth, then leave the
  studio — car, phone, earbuds — and give it fresh ears the next day before
  calling the milestone passed. Every one of these is a refusal to trust the room
  the track was made in.
