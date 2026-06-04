I spent a full day running controlled tests on Suno v5.5 output quality. Two things I found that nobody seems to be talking about. [RESEARCH]

BACKGROUND

I got tired of inconsistent results and started wondering whether the \*structure\* of prompts — not just the words — affects audio quality. So I designed a controlled experiment and measured every output with audio analysis tools.

Same genre. Same references. Same model. Only the prompt format changed.

FINDING 1 — HOW YOU STRUCTURE YOUR PROMPT MATTERS MORE THAN WHAT YOU SAY

I tested three approaches:

\- \*\*Approach A\*\* — Standard tag list (control): \`afro house, Black Coffee, 122 BPM, female vocals, no autotune...\`  
\- \*\*Approach C\*\* — Structured lyrics field only, tag list in style  
\- \*\*Approach D\*\* — Both fields fully structured with explicit categories

Measured across 11 audio metrics: spectral centroid, sub bass %, mids %, dynamic range, LUFS, LRA, vocal presence, vocal/sub ratio, masking ratios, harmonic content.

| Approach | Centroid | Sub Bass | Mids | DR | Score |  
|---|---|---|---|---|---|  
| A — Tag list | 199 Hz | 72.5% | 1.8% | 8.8 dB | 4/11 |  
| C — Partial structure | 293 Hz | 66.8% | 3.5% | 7.5 dB | 4/11 |  
| D — Full structure | 401 Hz | 41.3% | 16.0% | 11.6 dB | 10/11 |

The difference is not subtle. Sub bass dominance dropped from 72.5% to 41.3%. Mids went from nearly absent (1.8%) to genuinely present (16%). The overall mix quality score went from 4/11 to 10/11 — with zero mastering applied.

\*\*Why does this work?\*\* When you group related instructions into named categories, the model reads them as a hierarchical brief rather than a flat list of tags. \`vocal: \[confident, low register, breathy, behind the beat, no tuning\]\` communicates something fundamentally different to the model than the same words scattered across a tag list. The category name acts as a semantic anchor.

The style field (1000 chars) is too short for full structure but works well as a compressed key:value brief. The lyrics field (5000 chars) takes the full production document — universe, mastering intent, vocal direction, hook architecture, song structure, lyrics, and anti-prompt — all in named sections.

\*\*FINDING 2 — SERVER LOAD IS KILLING YOUR QUALITY BUT NOT MANY TALK ABOUT IT\*\*

While running tests I noticed output degrading later in the day. I started logging timestamps. Here's what I found across four identical structured prompts:

| Time (CET) | Quality Score |  
|---|---|  
| 07:17 | 10/11 |  
| 10:29 | 7/11 |  
| 11:05 | 6/11 |  
| 15:06 | 3/11 |

Same prompt. Same genre. Same model. Consistent decline as US traffic peaks.

The 15:06 generation was almost unrecognizable — dynamic range collapsed to 4.2 dB (from 11.6 dB in the morning), mids dropped to 1.7%, and the model ignored structural instructions entirely, adding random ad libs and ignoring the song architecture I'd specified.

\*\*Generate between 02:00–07:00 CET. This is no longer a theory — it's consistent across every test I ran.\*\*

My working explanation: under peak load, Suno reduces inference compute per request — fewer processing steps, more aggressive internal compression, less attention to detailed instructions. The output degrades in a very specific way: sub bass bloats, mids disappear, structure collapses. It's not random degradation. It's a consistent signature.

\---

\*\*THE HOOK ARCHITECTURE I USE\*\*

I also developed a four-layer approach to hooks that I specify explicitly in every prompt:

\- \*\*Hook I — Melodic\*\*: The vocal line that's hummable without lyrics. Defined with register and emotional arc. Arrives late, not upfront.  
\- \*\*Hook II — Rhythmic\*\*: A vocal phrase or chop locked to the groove. Works without pitch — the body remembers it before the mind does.  
\- \*\*Hook III — Instrumental\*\*: A 2–3 note motif that identifies the track without any vocal. DJ-playable anchor point.  
\- \*\*Hook IV — Textural\*\*: A subliminal sound signature — a breath, a room sound, a specific percussive detail. Once heard, its absence is felt.

Specifying all four explicitly gives the model a complete creative brief. Most prompts give it one, maybe two. The difference in output coherence is significant.

\---

\*\*THE ANTI-PROMPT STRUCTURE\*\*

Grouping negatives by category also outperforms a flat NO list:

\`\`\`  
no\_structure: EDM drop, festival drop, build and release, risers  
no\_vocal: autotune, pitch correction, vocal polish, AI vocal texture  
no\_rhythm: trap hihats, 808 bass, quantized grid timing  
no\_mix: over-bright highs, muddy mids, sub dominated mix  
no\_master: loudness war, squashed dynamics, brickwall limiting  
\`\`\`

Vs just: \`NO EDM drop, NO autotune, NO trap hihats, NO bright highs...\`

The categorized version tells the model \*why\* you don't want something, not just \*what\* you don't want.

\---

\*\*WHERE I AM WITH THIS\*\*

This is one day of testing — around 10 tracked generations. I'm treating it as directional research, not proof. For statistical confidence I need \~50 generations across 5 conditions. Current confidence: \~45%.

What I still need to test:  
\- Condition A proper baseline (same DNA, pure tag list, morning generation)  
\- Platform comparison: iOS vs web under the same load conditions  
\- Genre agnosticism: does this hold across Tech House, Neo Soul, Melodic Techno?

If anyone wants to run parallel tests with the same sonic DNA I'll share the full prompt templates. The more data points the better.

Happy to share templates and the test protocol. What are your experiences with prompt structure vs tag lists? And has anyone else noticed the time-of-day quality variation?