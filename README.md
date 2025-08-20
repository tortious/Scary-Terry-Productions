# Scary-Terry-Productions
My jams I have made from AI Music Lab. Below is a Manual I had made for effects and vocals specifically re AIMusicLabs


# AI Music Lab Prompt & Lyric Formatting Handbook

A practical, copy-pasteable guide to writing prompts and lyrics that reliably work in **AI Music Lab**. Written for GitHub Markdown—clean tables, concrete examples, and production-ready templates.

> **Why this matters:** Getting structure, tags, and descriptors right dramatically improves results and reduces retries. AI Music Lab supports lyrics and instrumental modes, style selection, tempo/mood controls, and a lyrics field with a **3,000-character limit**—so formatting and economy count. ([AI Music Lab][1])

---

## Contents

* [Core Concepts](#core-concepts)
* [Global Header (One-Liner)](#global-header-one-liner)
* [Section Tags (Song Layout)](#section-tags-song-layout)
* [Vocal Direction Tags](#vocal-direction-tags)
* [Instrument & Mix Tags](#instrument--mix-tags)
* [Dynamics & Arrangement Tags](#dynamics--arrangement-tags)
* [Character Limits & Smart Trimming](#character-limits--smart-trimming)
* [Common Pitfalls & Debugging](#common-pitfalls--debugging)
* [Copy-Paste Templates](#copy-paste-templates)
* [Full Examples](#full-examples)
* [Appendix: Reference Tables](#appendix-reference-tables)

---

## Core Concepts

* **Two places you “talk” to the model**

  1. **Global header line** at the very top (concise descriptors), and
  2. **Square-bracketed tags** inside the lyrics to mark sections and give directions.
* **Square brackets** (`[...]`) are the safest way to mark instructions/sections so they don’t leak into the sung text. (Parentheses can be misread as singable text by some lyric models; brackets reduce that risk.) ([Suno Wiki][2], [Reddit][3])
* **Stay under 3,000 characters** in the Lyrics box. (The Create page UI shows `0/3000`.) ([AI Music Lab][1])
* AI Music Lab lets you **choose styles/genres, adjust tempo/mood, and do instrumental-only tracks**—your formatting should align with those controls. ([AI Music Lab][4])

---

## Global Header (One-Liner)

Put a short descriptor **above everything**. Use `[]` and `key: value` pairs separated by pipes `|`.

```text
[BPM: 86 | Style: Hip-Hop / Trap-soul | Mood: Confident, nocturnal | Vocals: Female lead (clear, melodic), Male ad-libs | Key: B minor]
```

**Notes**

* **BPM** helps steer tempo; **Style** should match what you select in the UI (e.g., Pop, Rock, Hip-Hop, Jazz). ([AI Music Lab][4])
* **Mood** and **Vocals** guide performance and timbre.
* Optional extras: `Time Sig: 4/4`, `Energy: medium`, `Swing: light`.

### Quick Header Examples

| Goal               | Header       |                            |                          |                                                              |                  |
| ------------------ | ------------ | -------------------------- | ------------------------ | ------------------------------------------------------------ | ---------------- |
| Dark cinematic rap | \`\[BPM: 78  | Style: Hip-Hop / Cinematic | Mood: Menacing, spacious | Vocals: Male low register (laid-back), female hook (airy)]\` |                  |
| Upbeat summer pop  | \`\[BPM: 112 | Style: Pop                 | Mood: Bright, carefree   | Vocals: Female lead (crisp), stacked harmonies               | Key: D major]\`  |
| Smoky lounge jazz  | \`\[BPM: 84  | Style: Jazz                | Mood: Smoky, intimate    | Vocals: Male croon (breathy)                                 | Swing: medium]\` |

---

## Section Tags (Song Layout)

Mark parts with square-bracketed **section tags** on their own lines:

```text
[intro]
[verse 1]
[pre-chorus]
[chorus]
[post-chorus]
[verse 2]
[bridge]
[outro]
```

Add **brief directions** after a colon if helpful:

```text
[chorus: anthemic, wider harmonies, clap accents]
```

> Most lyric models respond well to explicit sectioning (verse/chorus/bridge). If you ask for “instrumental break/solo”, the engine may interpret creatively, so be concise. ([Reddit][5])

### Section Tag Quick Reference

| Tag                    | Purpose                | Direction Examples               |
| ---------------------- | ---------------------- | -------------------------------- |
| `[intro]`              | Set vibe before vocals | `low-passed beat, distant piano` |
| `[verse n]`            | Narrative/detail       | `tight flow, minimal ad-libs`    |
| `[pre-chorus]`         | Lift into hook         | `build, rising melody`           |
| `[chorus]`             | Main hook              | `anthemic, stacked harmonies`    |
| `[post-chorus]`        | Tag/chant              | `vocal chops, simpler lyric`     |
| `[bridge]`             | Contrast/release       | `new chords, softened drums`     |
| `[breakdown]`          | Minimal section        | `half-time drums, sparse bass`   |
| `[instrumental break]` | No vocals              | `8 bars, lead sax`               |
| `[outro]`              | Wrap up                | `fade elements, ad-lib trail`    |

---

## Vocal Direction Tags

Use **role-specific** tags to steer performance:

```text
[Lead Vocal: clear diction, relaxed delivery, intimate mic]
[Hook Vocal: airy female, doubled L/R, subtle plate reverb]
[Ad-libs: low volume, call-and-response, sporadic]
[Harmony: 3-part, tight thirds, only in chorus]
```

| Tag                   | What it does                           | Example                                   |
| --------------------- | -------------------------------------- | ----------------------------------------- |
| `[Lead Vocal: ...]`   | Guides the main singer’s tone/delivery | `warm chest voice, light grit`            |
| `[Rap Flow: ...]`     | Flow & cadence hints                   | `melodic rap, mid-tempo, internal rhymes` |
| `[Hook Vocal: ...]`   | Chorus voice style                     | `female bell-tone, wide doubles`          |
| `[Ad-libs: ...]`      | Punctuations/fills                     | `sporadic echoes on line ends`            |
| `[Choir/Stacks: ...]` | Layering instructions                  | `quad stack, soft blend`                  |
| `[Duet: ...]`         | Two leads                              | `female lead, male answer phrases`        |

> Brackets are favored to keep these from appearing in the sung text. ([Suno Wiki][2])

---

## Instrument & Mix Tags

Inline **instrument** or **mix** cues nudge arrangement:

```text
[Drums: tight 808s, crisp hats, light swing]
[Bass: sub with clean sidechain]
[Piano: detuned, felt pedal, sparse voicings]
[Sax: smoky lead, 8-bar solo in the bridge]
[FX: vinyl crackle, gentle tape wow/flutter]
```

| Category   | Examples                                                         |
| ---------- | ---------------------------------------------------------------- |
| Rhythm     | `808s`, `Boom-bap kit`, `Four-on-the-floor`, `Half-time`         |
| Harmony    | `Jazz piano`, `Warm Rhodes`, `Guitar arpeggios`, `String pad`    |
| Melody     | `Sax lead`, `Synth lead (saw)`, `Whistled hook`                  |
| Texture/FX | `Lo-fi noise`, `Plate/Room reverb`, `Tape delay`, `Filter sweep` |

> AI Music Lab supports selecting styles/genres and adjusting tempo/mood; these tags help the model interpret your intent within those settings. ([AI Music Lab][4])

---

## Dynamics & Arrangement Tags

Short, **plain-English** cues work best:

```text
[Build: add claps + tambourine]
[Drop: full drums, thicker bass]
[Crescendo: bars 5–8, strings swell]
[Breakdown: remove kick + bass for 4 bars]
[Re-intro: bring back opening piano riff]
```

> Keep cues brief and neutral (no overly technical plugin/signal-chain jargon).

---

## Character Limits & Smart Trimming

* **Target ≤ 3,000 characters** in the Lyrics field. (Shown as `0/3000` on the Create page.) ([AI Music Lab][1])
* Prefer **concise lines** (6–12 syllables) and reuse choruses.
* Optional shorthand that models usually parse fine (use sparingly for readability):

| Long                        | Short                   |
| --------------------------- | ----------------------- |
| and                         | `&`                     |
| to / too                    | `2`                     |
| for / four                  | `4`                     |
| with / without              | `w/` / `w/out`          |
| you / you’re / your         | `u` / `ur` / `ur`       |
| before / tonight / tomorrow | `b4` / `2nite` / `tmrw` |

> These are community-proven lyric shorthands from lyric-driven AI workflows; they’re not “official,” but they help fit under limits without harming output. Keep directions in brackets to avoid being sung. ([Reddit][6], [How to Prompt Suno][7])

---

## Common Pitfalls & Debugging

| Issue                         | Why it happens                         | Fix                                                                                                   |
| ----------------------------- | -------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| Instructions get sung         | Model mistook instructions as lyrics   | Put **all** directions in `[]`; avoid parentheses for directives. ([Suno Wiki][2])                    |
| Sections ignored / rearranged | Generators exercise creative structure | Keep section labels simple (`[verse 1]`, `[chorus]`), and avoid long prose inside tags. ([Reddit][5]) |
| Tempo feels off               | Style choice + vague tempo             | Specify `BPM` up top and choose a style aligned to that tempo. ([AI Music Lab][4])                    |
| Too wordy                     | Exceeds time budget                    | Shorten lines, repeat hooks, use trimming table above.                                                |
| Vocal tone wrong              | Ambiguous vocal cues                   | Add `[Lead Vocal: …]` and `[Hook Vocal: …]` with concrete adjectives (clear, airy, gritty).           |

---

## Copy-Paste Templates

### 1) Modern Rap / Melodic Trap

```text
[BPM: 84 | Style: Hip-Hop / Melodic Trap | Mood: Confident, nocturnal | Vocals: Male lead (clear, laid-back), female hook (airy) | Key: A minor]

[intro: filtered keys, distant vox chops]

[verse 1]
Line 1
Line 2
Line 3
Line 4

[pre-chorus: lift, add claps]
Line 1
Line 2

[chorus: anthemic, doubled hook]
Hook line A
Hook line B
Hook line A (repeat)

[verse 2]
Line 1
Line 2
Line 3
Line 4

[bridge: breakdown, no kick, airy pad]
Short contrasting idea

[outro: re-intro piano, soft ad-libs]
```

### 2) Pop (Upbeat)

```text
[BPM: 112 | Style: Pop | Mood: Bright, carefree | Vocals: Female lead (crisp), stacked harmonies | Key: D major]

[intro: palm-mute guitar, handclaps]

[verse 1]
...

[pre-chorus: rising melody, tom build]
...

[chorus: widest harmonies, clap on 2&4]
...

[post-chorus: chant hook]
...

[bridge: new chords, half-time]
...

[outro: tag the hook, fade]
```

### 3) Jazz / Lounge (Vocal)

```text
[BPM: 84 | Style: Jazz | Mood: Smoky, intimate | Vocals: Male croon (breathy), soft brush kit | Swing: medium]

[intro: upright bass + brushed kit, Rhodes comp]

[verse 1]
...

[chorus: warmer, add sax pad]
...

[bridge: sax lead 8 bars]
...

[outro: piano tag, hush]
```

### 4) Instrumental-Only

```text
[BPM: 100 | Style: Electronic / Chillhop | Mood: Warm, lo-fi, lazy afternoon | Vocals: none]

[intro: vinyl crackle, Rhodes + soft kick]
[instrumental break: 16 bars, add guitar licks]
[drop: full drums, sidechained pad]
[breakdown: remove bass 8 bars]
[outro: filter sweep down]
```

> AI Music Lab supports **instrumental mode** and style/tempo controls—this template pairs well with those settings. ([AI Music Lab][4])

---

## Full Examples

### Example A — Clear, Melodic Rap with Female Hook

```text
[BPM: 86 | Style: Hip-Hop / Trap-soul | Mood: Confident, nocturnal | Vocals: Male lead (clear, melodic), female hook (airy), low ad-libs | Key: B minor]

[intro: low-passed beat, distant piano riff]

[verse 1]
City lights flicker as the bassline breathes
Late drive thinking on the wins and fees
Small circle shining where the doubt once was
Grit on the meter, grace in the glove

[pre-chorus: lift, add claps + tambourine]
Heartbeat syncing with the skyline glow
Step to the edge, let the old weights go

[chorus: anthemic, doubled hook]
All night, we rise on a silver wave
Bright eyes, no fear of the leap we take
Hold tight, this fire’s gonna light our way
All night, all night—we’re wide awake

[verse 2]
Doorways open when you claim your name
Quiet focus cutting through the rain
Stacked faith humming like a new-tuned string
Every small promise turning into a wing

[bridge: breakdown, soft pad, no kick]
Let the echoes clear, feel the room expand
Breath meets rhythm in an open hand

[outro: bring back intro piano, soft ad-libs]
```

### Example B — Upbeat Pop

```text
[BPM: 118 | Style: Pop | Mood: Bright, breezy | Vocals: Female lead (crisp), tight harmonies | Key: G major]

[intro: guitar palm-mutes, clap on 2&4]

[verse 1]
Sun finds our windows, dancing down the hall
Coffee steam halos, notes along the wall
Laugh lines in motion, colors start to bloom
Today turns a corner, racing out the room

[pre-chorus: tom build, rising melody]
Feet on the pavement, timing feels aligned
Seconds start singing, falling into time

[chorus: widest harmonies, big snare]
Run with me, daylight in our shoes
Spin with me, nothing left to lose
Say we will, write it in the blue
Run with me—run with me, we do

[post-chorus: chant hook]
Hey-ey, hey-ey (we do)

[bridge: half-time, new chords]
Slow it, hold it—catch the glow we chose

[outro: tag the hook, fade]
```

### Example C — Lounge Jazz

```text
[BPM: 82 | Style: Jazz | Mood: Night-warm, intimate | Vocals: Male croon (breathy), close mic | Swing: light]

[intro: upright bass walk, brushed snare, Rhodes comp]

[verse 1]
Streetlamps hum in amber time
Footsteps fold in velvet lines
Windows lean to hear the tune
Summer’s echo, winter’s loom

[chorus: sax pad, widened piano voicings]
Hold me near the midnight breeze
Keep the hush between the keys
Name the stars we always knew
Pour the light like honey through

[bridge: sax solo 8 bars]
(Instrumental)

[outro: piano tag, hush the room]
```

---

## Appendix: Reference Tables

### A. Header Keys (Cheat-Sheet)

| Key                | Accepted Style                | Examples                               |
| ------------------ | ----------------------------- | -------------------------------------- |
| `BPM`              | integer                       | `BPM: 78`                              |
| `Style`            | free text matching UI choices | `Pop`, `Hip-Hop`, `Jazz`, `Electronic` |
| `Mood`             | adjectives (2–4)              | `Brooding, cinematic`                  |
| `Vocals`           | role + tone                   | `Female lead (airy), male ad-libs`     |
| `Key`              | optional                      | `Key: B minor`                         |
| `Swing` / `Energy` | optional                      | `Swing: medium`, `Energy: high`        |

> Align `Style` & tempo with what you pick in AI Music Lab’s UI (genres, tempo/mood controls). ([AI Music Lab][4])

### B. Section Tags

| Tag                    | Alias          | Tip                            |
| ---------------------- | -------------- | ------------------------------ |
| `[intro]`              | —              | Keep it short (2–8 bars)       |
| `[verse n]`            | `[v1]`, `[v2]` | Number verses                  |
| `[pre-chorus]`         | `[pre]`        | Short lift into hook           |
| `[chorus]`             | `[hook]`       | Repeat exact text to reinforce |
| `[post-chorus]`        | `[tag]`        | One-line chant works great     |
| `[bridge]`             | —              | Contrast harmony/rhythm        |
| `[instrumental break]` | `[solo: sax]`  | Name the instrument            |
| `[outro]`              | —              | Echo intro or chorus motif     |

### C. Direction Tags (Grab-Bag)

| Area     | Examples                                                                        |
| -------- | ------------------------------------------------------------------------------- |
| Vocals   | `Lead Vocal: clear diction`, `Hook Vocal: airy`, `Rap Flow: melodic, mid-tempo` |
| Drums    | `Drums: tight 808s`, `Boom-bap kit`, `Four-on-the-floor`, `Half-time`           |
| Bass     | `Sub 808`, `Picked electric`, `Acoustic upright`                                |
| Harmony  | `Piano felt`, `Warm Rhodes`, `Guitar arps`, `String pad`                        |
| Melody   | `Sax lead`, `Analog synth lead`                                                 |
| FX       | `Plate reverb`, `Tape delay`, `Vinyl crackle`, `Filter sweep`                   |
| Dynamics | `Build`, `Drop`, `Breakdown`, `Crescendo`, `Diminuendo`                         |

---

## Sources / Further Reading

* **AI Music Lab** — Create page (shows lyrics field and character counter; Custom vs Prompt modes). ([AI Music Lab][1])
* **AI Music Lab** — Docs overview (features, styles/genres, instrumental mode, tempo/mood controls). ([AI Music Lab][4])
* **Bracket usage for instructions** — General guidance for lyric AIs favoring square brackets to avoid singing directives. ([Suno Wiki][2], [Reddit][3])
* **Community notes on structure adherence** — Why simple tags work best and engines may reinterpret complex structures. ([Reddit][5])
* **Prompt-structure best practices** (genre/mood/instrument clarity; widely applicable to lyric AIs). ([How to Prompt Suno][7])

---

### Final Tips

* Keep the **header concise** (≤ 120 chars).
* Use **one idea per line**; recycle the chorus to save space.
* Prefer **square brackets** for any instruction or section name.
* Match your **Style** and **BPM** to the UI choices for best alignment. ([AI Music Lab][4])

Copy these templates into **AI Music Lab**, tweak the header, and you’re ready to generate polished results fast.

[1]: https://aimusiclab.co/create "AI Music Lab - Create AI-Generated Music"
[2]: https://sunoaiwiki.com/tips/2024-06-19-guide-suno-with-prompts-for-better-music/?utm_source=chatgpt.com "Guide Suno with Prompts for Better Music"
[3]: https://www.reddit.com/r/udiomusic/comments/1d5y415/adding_indications_in_brackets_about_how_to_sing/?utm_source=chatgpt.com "Adding indications in brackets about how to sing the song - Reddit"
[4]: https://aimusiclab.co/docs "AI Music Lab - Create AI-Generated Music"
[5]: https://www.reddit.com/r/SunoAI/comments/1donx5a/about_song_structure_instructions/?utm_source=chatgpt.com "About Song Structure Instructions... : r/SunoAI - Reddit"
[6]: https://www.reddit.com/r/SunoAI/comments/1c2wiwh/beginners_guide_at_making_songs_with_sunoai/?utm_source=chatgpt.com "Beginner's guide at making songs with Suno.ai : r/SunoAI - Reddit"
[7]: https://howtopromptsuno.com/making-music?utm_source=chatgpt.com "How to structure prompts for Suno AI"
