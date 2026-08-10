# Production Fundamentals

The teaching base for concept explanations (ladder rung 2). Distilled, opinionated,
genre-free. Teach one section at a time, never the file.

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

## Compression

A compressor turns dynamics into density. Four controls that matter first:
threshold (when), ratio (how much — 2:1 gentle, 4:1 firm, 8:1+ is an effect),
attack (slow lets transients through = punch; fast clamps them = smooth),
release (time it lets go — too fast pumps, too slow chokes).
Starting point for almost anything: 3:1, medium attack, release timed so the meter
returns to zero on the beat, 2–4 dB of gain reduction. Adjust by ear from there.

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
  calling the gate passed. Every one of these is a refusal to trust the room
  the track was made in.
