# Suno v5.5 Prompt Structure Research: Two Findings Nobody Seems to Be Talking About

I spent a full day running controlled tests on Suno v5.5 output quality and discovered two things that surprisingly few people seem to be discussing.

## Research Background

I got tired of inconsistent results and started wondering whether the structure of prompts—not just the words themselves—affects audio quality.

To test this, I designed a controlled experiment and measured every output using audio analysis tools.

- Same genre
- Same references
- Same model
- Only the prompt format changed

---

# Finding 1 — How You Structure Your Prompt Matters More Than What You Say

I tested three approaches:

### Approach A — Standard Tag List (Control)

text afro house, Black Coffee, 122 BPM, female vocals, no autotune... 

### Approach C — Partial Structure

- Structured lyrics field only
- Tag list remains in style field

### Approach D — Full Structure

- Both fields fully structured
- Explicit categories throughout

### Measured Metrics

Outputs were evaluated across 11 audio metrics:

- Spectral centroid
- Sub-bass percentage
- Midrange percentage
- Dynamic range
- LUFS
- LRA
- Vocal presence
- Vocal/sub ratio
- Masking ratios
- Harmonic content
- Overall mix quality

| Approach | Centroid | Sub Bass | Mids | Dynamic Range | Score |
|-----------|-----------|-----------|-----------|-----------|-----------|
| A — Tag List | 199 Hz | 72.5% | 1.8% | 8.8 dB | 4/11 |
| C — Partial Structure | 293 Hz | 66.8% | 3.5% | 7.5 dB | 4/11 |
| D — Full Structure | 401 Hz | 41.3% | 16.0% | 11.6 dB | 10/11 |

The difference is not subtle.

- Sub-bass dominance dropped from 72.5% → 41.3%
- Midrange presence increased from 1.8% → 16.0%
- Overall quality score improved from 4/11 → 10/11

All of this occurred with zero mastering applied.

## Why This Might Work

When you group related instructions into named categories, the model appears to interpret them as a hierarchical creative brief rather than a flat list of tags.

For example:

text vocal:   - confident   - low register   - breathy   - behind the beat   - no tuning 

communicates something fundamentally different from scattering the same words across a tag list.

The category name acts as a semantic anchor.

### Practical Observation

The Style field (1,000 characters) is too short for a fully structured brief, but it works well as a compressed key:value document.

The Lyrics field (5,000 characters) can contain the full production document:

- Creative universe
- Mastering intent
- Vocal direction
- Hook architecture
- Song structure
- Lyrics
- Anti-prompt framework

All organized into named sections.

---

# Finding 2 — Server Load Is Killing Your Quality

While running tests, I noticed output quality degrading later in the day.

I began logging timestamps.

Using four identical structured prompts, I observed the following:

| Time (CET) | Quality Score |
|------------|------------|
| 07:17 | 10/11 |
| 10:29 | 7/11 |
| 11:05 | 6/11 |
| 15:06 | 3/11 |

Same prompt.

Same genre.

Same model.

Consistent decline as U.S. traffic increased.

### The 15:06 Generation

Compared with the morning version:

- Dynamic range collapsed from 11.6 dB → 4.2 dB
- Midrange content dropped to 1.7%
- Structural instructions were largely ignored
- Random ad-libs appeared
- Song architecture was disregarded

## Recommendation

Generate between 02:00–07:00 CET.

At this point, I no longer consider this a theory. It was consistent across every test I ran.

## Working Hypothesis

Under peak load, Suno may reduce inference compute per request:

- Fewer processing steps
- More aggressive internal compression
- Reduced attention to detailed instructions

The degradation follows a consistent pattern:

1. Sub-bass bloats
2. Midrange disappears
3. Structure collapses

This doesn't look random.

It looks systematic.

---

# The Hook Architecture I Use

I also developed a four-layer hook framework that I explicitly specify in every prompt.

## Hook I — Melodic

The vocal line that remains memorable even without lyrics.

Defined by:

- Register
- Contour
- Emotional arc

Typically arrives later rather than immediately.

## Hook II — Rhythmic

A vocal phrase or chop locked tightly to the groove.

Works even without pitch.

The body remembers it before the mind does.

## Hook III — Instrumental

A simple 2–3 note motif that identifies the track without any vocal content.

Functions as the DJ-playable anchor point.

## Hook IV — Textural

A subliminal signature element:

- Breath
- Room sound
- Percussive detail
- Unique texture

Once heard, its absence becomes noticeable.

### Result

Most prompts specify one hook type, sometimes two.

Explicitly defining all four gives the model a much more complete creative brief and noticeably improves output coherence.

---

# The Anti-Prompt Structure

Grouping negatives by category consistently outperformed a flat "NO" list.

### Categorized Version

yaml no_structure:   - EDM drop   - festival drop   - build and release   - risers  no_vocal:   - autotune   - pitch correction   - vocal polish   - AI vocal texture  no_rhythm:   - trap hihats   - 808 bass   - quantized grid timing  no_mix:   - over-bright highs   - muddy mids   - sub-dominated mix  no_master:   - loudness war   - squashed dynamics   - brickwall limiting 

### Flat Version

text NO EDM drop NO autotune NO trap hihats NO bright highs ... 

The categorized version appears to tell the model why something is unwanted, not merely what is unwanted.

---

# Current Status

This is still early-stage research.

### Sample Size

- Approximately 10 tracked generations
- One day of testing

### Confidence Level

~45%

I consider this directional evidence rather than proof.

## What Still Needs Testing

### Condition A Baseline

- Same sonic DNA
- Pure tag list
- Morning generation only

### Platform Comparison

- iOS vs Web
- Same prompts
- Same load conditions

### Genre Independence

Does this hold for:

- Tech House
- Neo Soul
- Melodic Techno
- Other genres?

---

# Looking for Additional Data

If anyone wants to run parallel tests using the same sonic DNA, I'm happy to share:

- Prompt templates
- Test methodology
- Analysis workflow

The more data points we gather, the stronger the conclusions become.

Questions for the community:

1. Have you noticed structured prompts outperforming tag lists?
2. Have you experienced quality variations based on time of day?
3. What testing methods are you using to evaluate output quality?