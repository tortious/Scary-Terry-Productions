SUNO CREATION PLAYBOOK
FINAL DEPLOYABLE EDITION
April 11, 2026

Purpose:
This playbook is a front-facing guide for building, routing, diagnosing, and revising Suno song-creation work.
It combines the method guide and the live-use operator manual into one portable reference.

Who this is for:
- creators starting from scratch
- creators refining prompts
- creators trying to decide between prompting and native Suno workflows
- collaborators who need a clean starting point for understanding the method

How to use this playbook:
- Read Part I to understand the framework.
- Use Part II during live work.
- Route first, lint second, generate third, troubleshoot fourth.

Core rule:
Do not use a fresh generation prompt to solve an edit, preservation, or remix problem when Suno already gives you a native workflow for that job.

Evidence posture:
This playbook is built from a mixed research base:
- official Suno product and help documentation
- public surfaced songs used as success-proxy examples
- community guide threads
- user-reported failure patterns

Use it as a practical operating framework, not as a claim of absolute causal proof.
Public surfaced songs are success proxies, not proof that one prompt element caused the result.
Failure threads are negative-space evidence, not controlled laboratory studies.
The point is practical signal, not mythology.

==================================================
TABLE OF CONTENTS
==================================================

PART I — METHOD GUIDE
PART II — OPERATOR FIELD MANUAL

==================================================
PART I — METHOD GUIDE
==================================================

Created April 10, 2026
Purpose: Rebuilt operating manual for creating stronger, more repeatable Suno prompts with clearer priorities, tighter field logic, and data-backed prompt habits.

Revision note:
REV 6 is a true method rewrite.
It does not merely append new findings to the older structure.
It reorders the guide around what now appears to matter most in practice:
- performability
- front-person identity
- motion engine
- payoff design
- one memorable flourish
- adjacent positive reinforcement
- field-aware prompt construction
- working limit discipline
- Suno's recurring structural habits

This file treats the older detailed field material as supporting reference rather than the first organizing principle.

==================================================
1. CORE AIM
==================================================

The goal is not to write the most decorative prompt.
The goal is not to write the most technical-looking prompt.
The goal is not to describe every detail in existence.

The goal is to build a prompt that gives Suno:
- a clear public-facing song identity
- a clear motion engine
- a clear reward moment
- one distinct flavor worth remembering
- enough freedom to sound alive
- enough structure to avoid dissolving into mush

A strong Suno prompt should make the song legible at the points that matter most.

Practical translation:
A good prompt should let you answer, quickly:
- Who is on stage?
- What moves the body?
- Where does the payoff land?
- What one thing makes the song worth remembering?

If the prompt cannot answer those questions cleanly, it is probably not ready.

==================================================
2. HARD RULES
==================================================

Field-limit note:
Suno's official help confirms separate Title, Lyrics, and Styles fields in Custom mode and confirms richer prompting in the Lyrics box for v4.5-style workflows.
The exact character counts below are preserved here as current working limits observed in live use and testing, not as quoted official help-center counts.
Re-check these if Suno changes the UI.

Current working limits:
- Style box (sometimes called the Prompt box): 1000 characters
- Lyrics box: 5000 characters
- Song title / working title: 80 characters

Core hard rules:
1. No artist name-dropping.
2. The Style box must stay within 1000 characters.
3. The Lyrics box must stay within 5000 characters.
4. The song title / working title must stay within 80 characters.
5. The 1000-character limit is a real ceiling, not a suggestion.
6. The 5000-character limit is high, but it is not permission to become bloated.
7. Use the available space intentionally, not wastefully.
8. Use positive direction first.
9. Use negative restrictions sparingly and surgically.
10. One primary genre neighborhood only unless deliberate hybrid tension is the whole point.
11. Adjacent descriptors beat contradictory ones.
12. Do not stack too many unrelated genre identities at once.
13. Do not mistake technical-looking language for real control.
14. Do not mistake density for precision.
15. Change one variable at a time when testing.
16. Do not leave title length to memory or guesswork; check it before generation.
17. Do not assume section tags or shorthand cues mean exactly the same thing across all songs.
18. Do not confuse a good prompt with a good song; curation still matters.

==================================================
2A. OFFICIAL PRODUCT BEHAVIOR VS COMMUNITY CONVENTION
==================================================

Keep this distinction bright.

Official product behavior means:
- documented Suno surfaces and workflows
- known fields like Title, Style, and Lyrics
- native tools like Add Vocals, Add Instrumental, Cover, Extend, Stem workflows, Voices, Personas, Inspire, and Remix/Edit

Community convention means:
- bracket habits
- meta-tag formatting
- pipe-separated stacks
- [Genre:], [Vocal Style:], [Structure:], and similar community scaffolds
- other creator habits that may help but are not formal parser law

Important rule:
A convention can be useful without being officially supported.
Use community scaffolding when it improves clarity.
Do not mythologize it into secret syntax.

==================================================
3. WHAT WE NOW KNOW ABOUT SUNO
==================================================

The following findings come from repeated live generation tests and public-surface prompt review.

1. Suno is easier to steer on surface identity than deep structure.
It responds well to:
- genre lane
- vocal casting
- instrumentation
- arrangement cues
- mood
- cinematic function

It is harder to steer on:
- exact micro-timing
- unusual meter
- sustained anti-pop structure
- deep rhythmic rebellion across the whole song

2. Suno tends to normalize toward a standardized 4/4 feel.
Even when prompted toward stranger rhythmic ideas, the model often regularizes the result back into a familiar four-beat pulse or a 4/4-adjacent feeling.
Treat this as a strong working tendency, not an absolute law.

3. Suno also tends toward a familiar song chassis.
A common default structure is:
- verse 1
- pre-chorus that often thins or half-times
- chorus that pays off
- midpoint break or reset
- return chorus
- outro

Anything else is possible, but this chassis is sticky.
Prompt against it only one seam at a time.

4. Suno tends to obey content and dramatic function better than stopwatch timing.
Timestamps can help as loose anchors, but the model often follows:
- event order
- phrase emphasis
- section role
- release wording
better than exact second marks.

5. Section labels matter.
The model responds better when local behavior is staged clearly with sections or movements than when all control is buried in one abstract paragraph.

6. The model often wants to crown a lead singer.
Even when you ask for choir or collective voice, Suno may promote a singular featured vocalist unless you reduce solo opportunities and structure the vocal sections more aggressively.

7. Some lanes are naturally more compatible with the tool than others.
The free-tier sweet spot often favors:
- clear pulse
- clear hook
- clear front-person
- clear payoff
- polished or cinematic surface
- strong genre costume

==================================================
4. THE REAL X-FACTOR
==================================================

The strongest recurring pattern is not "the longest prompt wins."
It is not "the most technical prompt wins."
It is not "the most poetic prompt wins."

The hidden common denominator is this:

The better prompts reduce ambiguity at the exact points where both the listener and the model make snap judgments.

Those points are:
1. Front-person identity
2. Motion engine
3. Payoff placement
4. Signature flourish

This is the real x-factor.

The best-performing prompts usually do not try to control the whole song.
They lock down the song's public-facing identity and dramatic spine, then let Suno improvise the interior.

Put bluntly:
They make the song easy to perform convincingly.

==================================================
5. NEW BUILD ORDER
==================================================

Old prompt logic often starts with:
- genre
- subgenre
- mood
- sonic traits
- maybe voice
- maybe structure

That still can work.
But the stronger operating order now looks like this:

1. Front-person
Who is delivering the track?
Not just "vocals," but a real performer silhouette.

2. Motion engine
What physically drives the song?
What makes the body move or the pulse lock in?

3. Payoff design
Where does the listener get rewarded?
What is the hook event, chorus event, drop event, or reveal?

4. Signature flourish
What one thing makes this track memorable?

5. Genre neighborhood
What house does the song live in?
What nearby descriptors reinforce that house?

6. Field split
What belongs in the Style box and what belongs in the Lyrics box?

7. Supporting detail
Only after the core is stable:
- mix stance
- extra arrangement detail
- section-local behavior
- scene/world language
- restraint if truly needed

This order is not decorative.
It is practical.
It reflects what Suno seems most responsive to when songs actually come out replayable.

==================================================
6. THE X-FACTOR PROMPT TEST
==================================================

Use this before you generate.
Score each line 0 or 1.

1. Front-person test
Can you instantly picture who is delivering the song?
Examples:
- husky female lead
- airy duet
- chanty choir mass
- tense male clean verse with strained chorus
- talk-sung showgirl lead

Stronger version:
Can you picture the singer as a person rather than a checkbox?
The best front-person cues often use narrow descriptors plus one vivid image or role:
- cigarette-frayed baritone with a dry, exhausted delivery
- glittering city-pop lead who sounds like she is smiling through danger
- shy, breathy male vocal that feels too intimate for the size of the room

If the voice could belong to anybody, this fails.

2. Motion-engine test
Do you know what moves the track?
Examples:
- slap bass and tight drums
- rolling trance bassline
- brass stabs and swing drums
- rigid downtuned chugs
- bright arps and kick pulse

If the prompt has mood but no engine, this fails.

3. Payoff test
Do you know where the listener's reward moment is?
Examples:
- explosive chorus
- delayed drop
- instrumental hook
- fusion solo
- chant refrain
- half-time breakdown into final return

If there is no obvious payoff, this fails.

4. Signature-flourish test
Does the song have one thing that makes it memorable?
Examples:
- glitch-chopped vocals
- diner-brass sparkle
- metallic throat chirps
- Latin choir over metal
- arcade-sugar synth lead

Do not chase ten.
One strong flourish is enough.

5. Adjacency test
Are the genre and influence words from the same neighborhood?
Good:
- electro-swing + retro dance brass + funk-pop
- dream pop + indie pop + alt-pop
- dark orchestral + symphonic metal + gothic industrial

Bad:
- city pop + doom metal + bossa nova + witch house + folk gospel

If the descriptors pull toward different cities, this fails.

6. Performability test
Can you imagine this being performed?
If the prompt makes you picture a body, stage, crowd, and emotional role, it passes.
If it only sounds like analysis, it fails.

7. Surface-to-depth ratio test
Does the prompt lock down the public-facing identity and dramatic spine while still leaving the model room to breathe?
Too little = generic.
Too much = stiff, swollen, or internally conflicted.

Scoring:
- 6 to 7 = very strong
- 4 to 5 = workable
- 2 to 3 = mush risk
- 0 to 1 = costume pile

Fast repair order:
If a prompt is failing, do not add three more adjectives first.
Repair in this order:
1. who is singing
2. what drives the motion
3. where the payoff lands
4. what one thing makes the song memorable

One-line rule:
A strong Suno prompt should tell you who is on stage, what moves the body, where the payoff lands, and what one thing makes the song worth remembering.

==================================================
7. FIELD MODEL — TITLE VS STYLE BOX VS LYRICS BOX
==================================================

These fields do not do the same job.

TITLE / WORKING TITLE
Working limit: 80 characters.
Purpose:
- naming
- mood cue
- memorability
- branding
- searchability inside your own working library

Use rule:
The title is part of the prompt package and should be treated that way.
Check it before generation.
Do not leave it to memory or guesswork.
An overdramatic title is useless if it breaks the cap.

STYLE / PROMPT BOX
Working limit: 1000 characters.
Purpose:
- global identity
- genre neighborhood
- front-person silhouette
- motion engine
- broad emotional world
- core sonic palette
- broad production/mix stance
- top-level arrangement promise

The Style box should answer:
What is this song overall?

LYRICS BOX
Working limit: 5000 characters.
Purpose:
- actual lyrics
- section tags
- local arrangement behavior
- local vocal routing
- transitions, pauses, breaks, and impact events
- phrase-level delivery cues
- high-resolution section staging

The Lyrics box should answer:
What happens where?

Core field rule:
The Style box should describe the song's overall world.
The Lyrics box should stage the song's local events.

==================================================
8. LIMIT-AWARE BUILD DISCIPLINE
==================================================

Treat the three fields as different pressure zones.

TITLE / WORKING TITLE
- hard working limit: 80 characters
- should be checked before generation, not after
- long theatrical titles are allowed only if they survive the cap
- if a title must be cut, shorten wording without losing the core flavor

STYLE / PROMPT BOX
- hard working limit: 1000 characters
- use for global identity only
- every phrase must earn its place
- adjacent reinforcing descriptors beat decorative overflow
- compress aggressively when the identity is already clear

LYRICS BOX
- hard working limit: 5000 characters
- use for section tags, lyrics, local arrangement notes, and high-resolution control
- the high ceiling is room for clarity, not permission for sprawl
- a bigger box should produce cleaner staging, not more sludge

Compression rule:
If you are running out of room, cut in this order:
1. duplicate adjectives
2. redundant genre labels
3. decorative scene language that adds no control
4. over-explained negatives
5. extra technical wording that does not change the song

Do not cut:
- singer identity
- motion engine
- payoff placement
- one memorable flourish

==================================================
9. THE STYLE BOX — WHAT BELONGS THERE
==================================================

The Style box should usually contain:

1. Front-person / performer identity
Examples:
- lively female lead with a smiling tone
- deep broken male vocal
- massed low choir
- no vocals
- fragmented non-lead vocals only

Use note:
When there is a singer, make them feel inhabited.
A strong front-person description usually combines:
- voice body
- emotional posture
- stage role
- one vivid distinguishing detail

Examples:
- bruised baritone, restrained and bitter, like he is trying not to lose composure on stage
- airy female lead with polished city-night confidence and a teasing edge
- trembling intimate tenor, soft-spoken until the chorus tears open
- collective ritual choir, severe, faceless, and non-individual

Do not confuse this with writing a whole character sheet.
You usually only need one or two rich details, as long as they narrow the performer into a specific human or specific collective presence.

2. Genre neighborhood
Examples:
- electro-swing, retro dance brass, funk-pop
- Japanese post-modern electropop, glossy digital pop chaos
- dark orchestral ritual metal, symphonic metal
- deep house with late-night underground tension

3. Motion engine
Examples:
- slap-heavy bass and tight drums
- hard four-on-the-floor with brass bounce
- rolling bassline and trance pulse
- rigid downtuned chug pattern
- filtered industrial pulse and sub pressure

4. Broad emotional world
Examples:
- playful and dazzling
- claustrophobic and wounded
- sacred and wrathful
- dreamlike and chemically bright
- nocturnal and elegant

5. Core sonic palette
Examples:
- brass stabs, upright bass, piano sparkle
- supersaw leads, rolling bassline, metallic stabs
- strings, brass, organ, bell, downtuned guitars
- glassy plucks, arcade synths, digital error textures

6. Broad production / mix stance
Examples:
- polished and bright
- clear but not overcompressed
- wide cinematic contrast
- dry tense verses, larger chorus impact
- glossy modern sheen

7. One top-level arrangement promise
Examples:
- mostly instrumental chorus hook
- delayed drop
- haunted orchestral intro that later ruptures into metal
- instrumental break after second chorus
- sparse opening into bigger payoff

What the Style box should not do:
- explain every section in detail
- carry every lyric-side event
- become a giant blacklist
- try to do the whole song alone

==================================================
10. THE LYRICS BOX — WHAT BELONGS THERE
==================================================

The Lyrics box is the fine-control layer.

It should usually contain:
- section tags
- actual lyrics
- section-local instrumental behavior
- local vocal routing
- local delivery changes
- impact cues
- breaks, pauses, and transitions
- experimental local instructions when needed

Good uses:
- [Verse 1] [Female Vocal]
- [Chorus] [Full Choir]
- [Instrumental Break]
- [build: drums thin out]
- [first line nearly alone, second line cues drop]
- [collective choir only, no soloist]
- [no vocals here]

Weak uses:
- re-describing the overall genre
- repeating the Style box with slightly different words
- stuffing giant mood paragraphs where event cues would be cleaner

Bracket rule:
If you are using control text, section staging, timestamps, or behavior notes, keep them bracketed so Suno does not misread them as singable lyrics.

==================================================
11. TIMESTAMPS, RANGES, AND EVENT CUES
==================================================

Use timestamp language carefully.

What testing suggests:
- Suno often treats exact time as advisory
- Suno is more faithful to content, order, and dramatic role than to second-by-second precision
- strong local event cues tend to work better than obsessive micro-timing

Better uses:
- around 0:20-0:30 vocals begin
- early chorus line lands nearly alone
- second line triggers the drop
- midpoint break strips the beat
- final hook returns heavier

Best working principle:
Prompt for event order and function, not exact clock obedience.

Timestamps are useful when they help stage:
- early / middle / late entries
- breaks
- fake-outs
- returns
- drops
- pauses
- local texture changes

Do not ask Suno to behave like a DAW timeline if the model is not acting like one.

==================================================
12. STRUCTURE BIAS — WORK WITH IT OR PUSH ONE SEAM AT A TIME
==================================================

Suno often defaults toward a familiar song frame.
In practice, many tracks behave like:

verse -> pre-chorus -> chorus -> midpoint break -> return chorus -> outro

The pre-chorus often:
- thins out
- half-times
- drops the beat
- acts as pressure valve

The midpoint often:
- strips layers
- resets energy
- prepares the second big payoff

This means:
- the model is easier to steer on costume than on skeleton
- a lot of "variation" is really ornament on the same structural chassis

Practical rule:
If you want to push structure, attack one seam at a time.

Examples of good seam-pushes:
- make the chorus instrumental
- delay the first vocal
- deny the second chorus a full return
- open with orchestral movements instead of verse labels
- make the break happen early
- hard-stop the outro instead of resolving
- blur verse and chorus together
- remove the pre-chorus

Do not try to overthrow every structural habit at once unless you are prepared for the model to snap back into standard song behavior.

==================================================
13. DATASET-DRIVEN PATTERNS FROM PUBLIC SUNO SURFACES
==================================================

Reference note:
This section preserves the practical findings drawn from a proxy review of public Suno surfaces, including Suno's Trending playlist, official Best Of playlists, and other public curation surfaces visible at the time of review.
Treat this as a pattern-reference aid, not as definitive chart science.
The goal is not to prove universal law.
The goal is to preserve repeated traits that appeared often enough to be useful.

Core repeated findings:

1. Adjacent-genre clustering beats genre pile chaos.
Popular or surfaced prompts often stack multiple nearby genre labels rather than one isolated tag or many conflicting tags.

2. Vocal casting is one of the strongest recurring levers.
The better prompts often define who is singing and how they sound.

3. Instrument-role clarity matters.
The stronger prompts often give instruments jobs instead of only describing vibe.

4. Dynamic contrast is a frequent listen-worthiness factor.
Many surfaced prompts promise a before-and-after movement.

5. There are several recurring prompt families.
Most visible prompts tend to fall into one of these broad families:
- adjacent-tag stack
- arrangement brief
- full performance script

6. Overstuffed prompts can still work.
This does not mean bloat is the goal.
It means Suno can sometimes tolerate prompt sprawl when the lane, singer, groove, and payoff are still legible.

7. Simple prompts can still work.
Very basic prompts can still surface if the lane is easy for the model and the result sounds finished enough to replay.

8. Hybrid J-pop / anime-adjacent / electro-pop lanes appeared often.
This does not make them universal winners, but it does suggest that bright hybrid pop with strong hook logic is very compatible with public-facing Suno output.

Practical conclusion:
Most surfaced tracks do not appear to win because the prompt is clever.
They appear to win because the song is legible fast:
- clear lane
- clear singer
- clear groove engine
- clear payoff
- one memorable flourish

==================================================
14. POSITIVE REINFORCEMENT VS NEGATIVE FENCING
==================================================

Positive prompting generally works better than blacklist prompting.

Instead of:
- not grunge
- not pop
- not folk
- not EDM
- not this
- not that

prefer:
- dry, mechanical, wounded, claustrophobic
- retro dance brass with polished city sparkle
- collective choir mass with ritual severity
- bright arcade synth chaos with playful feminine lead

Use negatives sparingly when:
- a recurring parasite keeps appearing
- the model keeps snapping into the same wrong thing
- one surgical exclusion will actually help

Good surgical negatives:
- no soloist
- no rap cadence
- no lead strings
- no vocals here
- no heroic chorus lift

Bad negative overflow:
giant blacklist paragraphs that make the model orbit the ghosts you are trying to banish.

==================================================
15. PROMPT ARCHETYPES
==================================================

There are several stable archetypes that work well.

A. Adjacent-tag stack
Best when:
- the lane is already clear
- you want a compact Style box
- the genre neighborhood is doing most of the work

Example logic:
dream pop, indie pop, alt-pop, soft rock shimmer

B. Arrangement brief
Best when:
- instrument roles matter
- contrast matters
- you need a clearer body and payoff

Example logic:
slap bass drives, tight drums, guitar scratches, brass stabs, energetic tenor, fusion solo mid-track

C. Full performance script
Best when:
- multiple roles matter
- section identity matters
- the song is theatrical or high-concept

Example logic:
three distinct female voices, crowd noise, verse/chorus behavior changes, genre switching by section

D. Source-sheet mode
Best when:
- you are defining a reusable sonic doctrine
- you want a prompt constitution, not a one-off song
- future prompts will inherit the same internal rules

E. Movement-state scripting
Best when:
- the song transforms across states
- the opening identity must hold before the later rupture
- section names like "verse" are causing the model to rush into default structure

Example logic:
[Opening Omen] -> [Escalation] -> [Threshold] -> [Rupture] -> [Chant Movement]

==================================================
16. QUICK BUILD TEMPLATE
==================================================

Use this when you want a fast but disciplined build.

STEP 1 — FRONT PERSON
Who is on stage?
Examples:
- bright smiling female lead
- tense clean male lead
- no singer, instrumental
- low massed choir
- airy duet

Better question:
What kind of person is this singer, in only a few words?
Try to give the performer a narrow body and posture, not just a label.

Examples:
- polished flirt with a bright, dangerous smile
- tired baritone carrying private damage
- fragile close-mic tenor that sounds one breath away from collapse
- collective faceless choir with no room for individuality

STEP 2 — MOTION ENGINE
What moves the body?
Examples:
- slap bass and tight drums
- four-on-the-floor kick with brass bounce
- rolling trance bassline
- rigid guitar chug and punchy snare
- filtered sub pulse with metallic texture

STEP 3 — PAYOFF
Where is the reward?
Examples:
- explosive chorus
- delayed drop
- instrumental hook
- fusion solo
- giant chant refrain

STEP 4 — FLOURISH
What one thing makes it memorable?
Examples:
- glitch-chopped vocals
- diner-brass sparkle
- metallic throat chirps
- choir in Latin over metal
- arcade-sugar synth lead

STEP 5 — GENRE NEIGHBORHOOD
What house does it live in?
Choose adjacent descriptors only.

STEP 6 — FIELD SPLIT
Put global identity in Style.
Put local events in Lyrics.

==================================================
17. FAILURE PATTERNS
==================================================

1. Mush prompt
Too many descriptors, no front-person, no engine, no payoff.

Fix:
reduce to singer, engine, payoff, flourish.

2. Metadata prompt
Technically detailed, but no performability.

Fix:
make the singer and crowd picture clearer.

3. Costume pile
Many genre labels pulling in different directions.

Fix:
choose one neighborhood.

4. Wrong silhouette
The song sounds good but belongs to the wrong species.

Fix:
change the weight class, not the whole concept.

5. Default backbeat drift
The model normalizes into a generic 4/4 pulse.

Fix:
work with the 4/4 cage unless you are explicitly running a structure test.
Push surface identity and local event behavior instead of expecting radical meter obedience.

6. Lead singer takeover
Choir or ensemble prompt collapses into a featured soloist.

Fix:
reduce vocal sections, create more instrumental zones, specify collective-only sections, and avoid giving the model easy solo openings.

7. Sprawling Lyrics box
Too much staging, not enough clarity.

Fix:
use the bigger box for legibility, not sludge.

==================================================
18. TITLE DISCIPLINE
==================================================

The title matters more than people think.
It is:
- branding
- search memory
- mood cue
- part of the prompt package

Rules:
- keep it under 80 characters
- test the title like part of the song, not an afterthought
- long titles can work if they survive the cap and preserve a clear flavor
- overdramatic titles are acceptable if the flavor is intentional

A title can:
- reinforce the aesthetic
- sharpen the scene
- create irony
- turn a generic song into a more memorable artifact

But the title should not do the song's entire job for it.

==================================================
19. FINAL REMINDER
==================================================

A good Suno prompt is not a complete simulation of the song.
It is a clean staging system.

It should make the model's job easier at the points that matter most:
- who is performing
- what drives the motion
- where the payoff lands
- what one thing makes the song worth remembering

Everything else is support.

If the prompt starts swelling, return to:
front-person
motion engine
payoff
flourish
adjacent genre house
field split

That is the real spine.

==================================================
PART II — OPERATOR FIELD MANUAL
==================================================

Use Part II during live work.
It is ordered for action: route first, lint second, generate third, troubleshoot fourth.

Built from the research stack:
- normalized dataset
- findings memo
- troubleshooting matrix
- prompt lint checklist
- workflow routing sheet

Purpose:
This is the practical operator section.
It is meant to help decide:
1. what kind of Suno task is actually in front of you
2. which surface should solve it
3. whether the prompt is clean enough to justify a generation
4. how to diagnose a miss without spiraling into random prompt edits

Core law:
Do not use a fresh generation prompt to solve an edit, preservation, or remix problem when Suno already gives you a native workflow for that job.

==================================================
I. FAST OPERATING ORDER
==================================================

Use this order:

1. Route the job.
Ask:
- Is this a fresh song-generation task?
- Is this a local section-control task?
- Is this a source-preservation task?
- Is this a cover / style-transfer task?
- Is this an ending-fix or section-repair task?
- Is this a stems / cleanup task?

2. Lint the prompt.
Before generating, check:
- front-person
- motion engine
- payoff
- genre neighborhood
- one memorable flourish
- field split
- structure ambition
- instrumental purity risk
- negative-prompt discipline
- workflow routing
- revision hygiene
- species test

3. Generate or use the chosen workflow.

4. If it misses, classify the miss before changing anything.
Do not add more adjectives until you know what failed.

==================================================
II. FAST DECISION RULES
==================================================

Use a fresh text prompt when the real job is:
- create a new song body
- define lane, singer, groove, payoff, and flourish
- test broad genre or section ideas

Use a native workflow when the real job is:
- preserve uploaded audio
- preserve your voice
- change only the ending
- replace one broken section
- transfer style while keeping melody
- borrow from a playlist body
- reuse a voice/persona/model identity
- extract stems for later repair

If you cannot tell which it is:
- run the prompt lint checklist
- classify the miss with the troubleshooting matrix
- only then revise or reroute

==================================================
III. WORKFLOW ROUTING SHEET
==================================================

SUNO WORKFLOW ROUTING SHEET — REV 1

Purpose:
Use this sheet to decide which Suno surface should solve the job before you start spending generations.

Core rule:
Do not use a fresh generation prompt to solve an edit, preservation, or remix problem when Suno already gives you a native workflow for that job.

==================================================
ROUTING SHEET
==================================================

[01] Task / goal
Create a new song from scratch

Best starting path: Fresh text prompt
Use this when: You are defining a new lane, singer, groove, payoff, and overall identity without needing to preserve existing audio.
Primary Suno surfaces: Custom Mode: Title + Style + Lyrics
Prompt emphasis: Front-person, motion engine, payoff, flourish, adjacent genre house, field split
Common mistake: Trying to solve downstream editing problems before generating a clean song body
Escalate / switch when: The body is good but a specific section, ending, or source-preservation issue remains
Notes: This is the default creation path.

--------------------------------------------------

[02] Task / goal
Write or control local section behavior

Best starting path: Lyrics-box local control
Use this when: The global identity is mostly right, but verse/chorus/bridge behavior, local vocal routing, or instrumental breaks need help.
Primary Suno surfaces: Custom Mode Lyrics field
Prompt emphasis: Section tags, local cues, local vocal occupancy, event order, line anchors
Common mistake: Stuffing all local section logic into the Style box
Escalate / switch when: The model still skips or rewinds sections despite simplified staging
Notes: Best for local shaping, not for forcing exact execution.

--------------------------------------------------

[03] Task / goal
Create an instrumental-only piece

Best starting path: Fresh text prompt with instrumental-specific lint pass
Use this when: You want a new instrumental and do not need to preserve any uploaded source.
Primary Suno surfaces: Custom Mode with instrumental-only framing
Prompt emphasis: No vocals, instrumental function, non-vocal payoff, loop/body role, engine clarity
Common mistake: Leaving singer-like hook language or lyrical atmosphere cues in the prompt
Escalate / switch when: Stray vocals or hums persist across multiple clean generations
Notes: Instrumental purity remains unstable.

--------------------------------------------------

[04] Task / goal
Preserve an uploaded instrumental and add vocals

Best starting path: Add Vocals workflow
Use this when: You already have instrumental audio and want Suno to generate vocals over it.
Primary Suno surfaces: Audio Upload + Add Vocals
Prompt emphasis: Preserve this body; add only vocal identity and lyric behavior
Common mistake: Treating it like a full regeneration prompt instead of a source-preservation task
Escalate / switch when: The instrumental keeps changing materially or the vocal identity is too unstable
Notes: Plan for stems or external cleanup if preservation is critical.

--------------------------------------------------

[05] Task / goal
Preserve your uploaded vocals and add instrumental backing

Best starting path: Add Instrumental workflow
Use this when: You have a vocal recording and want Suno to build instrumental support around it.
Primary Suno surfaces: Audio Upload + Add Instrumental
Prompt emphasis: Protect the vocal body; add only the surrounding engine and arrangement
Common mistake: Assuming Suno will preserve your exact vocal identity with no reinterpretation
Escalate / switch when: The voice gets overprocessed or identity drift becomes the main issue
Notes: This is a source-preservation workflow, not a normal prompt-only task.

--------------------------------------------------

[06] Task / goal
Change the style of an existing song while keeping melody

Best starting path: Cover
Use this when: You like the melody or song body, but want it recast into a different style.
Primary Suno surfaces: Cover feature
Prompt emphasis: New style house, new production world, preserved melodic identity
Common mistake: Trying to recreate the whole thing from scratch with a new prompt
Escalate / switch when: The preserved body matters less than the general inspiration
Notes: Best when style transfer is the real task.

--------------------------------------------------

[07] Task / goal
Borrow inspiration from multiple songs rather than one exact source

Best starting path: Inspire
Use this when: You want Suno to synthesize style influence from a playlist rather than obey one text prompt alone.
Primary Suno surfaces: Inspire feature
Prompt emphasis: Reference vibe and broader musical body rather than literal imitation
Common mistake: Overloading the text prompt with many genre names when a source set would do the work better
Escalate / switch when: You need exact preservation, exact structure, or exact vocal identity
Notes: This is native style-borrowing, not ordinary prompt stacking.

--------------------------------------------------

[08] Task / goal
Reuse a known voice/persona/model identity

Best starting path: Voices / Personas / Custom Models
Use this when: The voice identity itself is the important continuity element.
Primary Suno surfaces: Voices, Personas, Custom Models, My Taste
Prompt emphasis: Song body and role, not rebuilding the singer from scratch every time
Common mistake: Trying to brute-force singer identity with repeated text alone
Escalate / switch when: The native identity tools still fail to preserve the target enough
Notes: This moves part of control outside pure text prompting.

--------------------------------------------------

[09] Task / goal
Fix only the ending or extend the song length

Best starting path: Extend
Use this when: The main body is right, but the ending, resolution, or duration is wrong.
Primary Suno surfaces: Extend / Remix/Edit
Prompt emphasis: What should happen from the cut point onward
Common mistake: Regenerating the entire song just to fix the ending
Escalate / switch when: You also need major earlier-structure changes
Notes: Ending control is often better handled here than by raw prompt pressure.

--------------------------------------------------

[10] Task / goal
Replace or repair one broken section

Best starting path: Replace Section / Remix/Edit
Use this when: A single section is the issue: wrong bridge, skipped verse, weak drop, bad transition.
Primary Suno surfaces: Replace Section / Remix/Edit family
Prompt emphasis: Only the local section goal and what it must now do
Common mistake: Throwing away a mostly good song because one section failed
Escalate / switch when: The entire song species is wrong, not just one section
Notes: This is the clean fix for local damage when the rest is fine.

--------------------------------------------------

[11] Task / goal
Keep the audio but change speed or timing feel later

Best starting path: Adjust Speed / post-generation editing
Use this when: The performance mostly works, but the pacing or timing feel is off.
Primary Suno surfaces: Remix/Edit family; external editing if needed
Prompt emphasis: Do not rely on exact BPM alone for first generation
Common mistake: Trying to bully exact tempo into existence through text only
Escalate / switch when: Meter itself is wrong, not just speed
Notes: Prompt for groove feel first; refine tempo later.

--------------------------------------------------

[12] Task / goal
Extract parts for cleanup, remixing, or DAW repair

Best starting path: Stem Extraction
Use this when: The generation is usable but needs cleanup, preservation, or recombination outside Suno.
Primary Suno surfaces: Stem Extraction / Studio
Prompt emphasis: Get the best generation you can, then separate it
Common mistake: Demanding perfect preservation or editability from the first generation itself
Escalate / switch when: The source material is fundamentally wrong, not just in need of cleanup
Notes: This is often the smartest path for source-preservation and instrumental-purity issues.

--------------------------------------------------

[13] Task / goal
Preserve melody or rhythm from a source clip but swap instruments

Best starting path: Stem Cover / Studio
Use this when: You want the skeleton of the source to remain, but the sound body to change.
Primary Suno surfaces: Stem Cover / Studio Cover or Recreate distinction
Prompt emphasis: Preserve melodic/rhythmic scaffold while changing timbral body
Common mistake: Trying to fake this with a fresh text prompt and hoping it lands close enough
Escalate / switch when: Exact preservation matters more than reinterpretation
Notes: This is style/body transformation with stronger source anchoring.

--------------------------------------------------

[14] Task / goal
Diagnose why a prompt failed before changing it again

Best starting path: Lint checklist + troubleshooting matrix
Use this when: You have a miss but do not yet know whether it is singer, engine, payoff, structure, or routing.
Primary Suno surfaces: Analysis step before generation
Prompt emphasis: Classify the miss first
Common mistake: Adding more adjectives without knowing what actually failed
Escalate / switch when: The same failure class repeats after a clean repair
Notes: This is the diagnostic entry point.

--------------------------------------------------

==================================================
FAST DECISION RULES
==================================================

Use a fresh text prompt when the real job is:
- create a new song body
- define lane, singer, engine, payoff, and flourish
- test broad genre or section ideas

Use a native workflow when the real job is:
- preserve uploaded audio
- preserve your voice
- change only the ending
- replace one broken section
- transfer style while keeping melody
- borrow from a playlist body
- reuse a voice/persona/model identity
- extract stems for later repair

If you cannot tell which it is:
- run the prompt lint checklist
- classify the miss with the troubleshooting matrix
- only then revise or reroute

==================================================
IV. PROMPT LINT CHECKLIST
==================================================

SUNO PROMPT LINT CHECKLIST — REV 1

Use note:
Run this before generation.
The goal is not to make prompts more ceremonial.
The goal is to catch the weak spots most likely to waste a generation.

Scoring suggestion:
- PASS = clear enough
- WATCH = partially clear, but drift risk remains
- FAIL = likely to waste credits or test the wrong layer

Quick rule:
A strong prompt should make the song legible fast at the snap-judgment points that matter most:
- who is performing
- what moves the body
- where the payoff lands
- what one thing makes it memorable

==================================================
CHECKLIST
==================================================

[01] Front-person clarity
Question: Can I instantly picture who is delivering this song, or is the singer/body still generic?
Why it matters: Success-side rows repeatedly made the front-person or non-vocal role legible early.
Pass looks like: Husky female lead; raw baritone; breathy male vocal; no vocals; full choir; chopped vocal samples only.
Fail looks like: Vocals. Male or female maybe. Emotional singer.
Repair move: Describe the voice physically and tonally, not only by gender label.

--------------------------------------------------

[02] Motion engine clarity
Question: Do I know what actually moves the track?
Why it matters: Successful rows usually name the groove engine, not just the mood.
Pass looks like: 2-step drums and rolling sub-bass; downtuned chug and punchy snare; upright bass and swing drums.
Fail looks like: Energetic. Groovy. Big production.
Repair move: Name the rhythm section, the pulse source, or the lead body-moving layer.

--------------------------------------------------

[03] Payoff design
Question: Is the reward moment visible?
Why it matters: Chorus, drop, hook, or breakdown clarity kept recurring in stronger outcomes.
Pass looks like: Explosive chorus; delayed drop; stripped breakdown before final return; instrumental hook.
Fail looks like: The song should be exciting all the way through.
Repair move: State where the listener gets paid and how.

--------------------------------------------------

[04] Genre neighborhood
Question: Do the genre words all live in the same house?
Why it matters: Adjacent clustering helped; costume piles drifted.
Pass looks like: Dream pop + indie pop + alt-pop. UK garage + house + jazz-pop fusion.
Fail looks like: Doom metal + city pop + bossa nova + witch house + gospel.
Repair move: Keep one primary genre house and one adjacent color unless fusion is the whole thesis.

--------------------------------------------------

[05] One memorable flourish
Question: What one thing makes the track worth remembering?
Why it matters: The strongest rows often had one flourish, not ten competing gimmicks.
Pass looks like: Glitch-chopped vocals; robotic doubles; Latin choir over metal; analog tape haze.
Fail looks like: Many cool details, none load-bearing.
Repair move: Choose one signature garnish and let it brand the track.

--------------------------------------------------

[06] Field split discipline
Question: Am I using Style for global identity and Lyrics for local behavior?
Why it matters: Official behavior and guide rows kept validating the field split.
Pass looks like: Style defines lane, singer, engine, palette; Lyrics handles sections, local cues, and events.
Fail looks like: The Style box is doing every section in detail, or the Lyrics box is just restating the Style box.
Repair move: Move global identity up; move local staging down.

--------------------------------------------------

[07] Structure ambition
Question: Am I asking for something Suno reliably resists?
Why it matters: Odd meter, mixed meter, strict timestamps, and section-perfect fidelity stayed weak in the dataset.
Pass looks like: One structural seam pushed at a time.
Fail looks like: Odd meter, alternating regimes, exact timestamp obedience, and section-perfect execution all demanded at once.
Repair move: Simplify the structure ask or shift to source-audio / edit workflows.

--------------------------------------------------

[08] Instrumental purity risk
Question: Am I asking for an instrumental while still leaving vocal affordances in the prompt?
Why it matters: Instrumental purity failures were common.
Pass looks like: No vocals, instrumental only, loop/function language, non-vocal payoff.
Fail looks like: Instrumental track with emotional singer-like hook language and lyrical atmosphere all over the prompt.
Repair move: Remove singer language and anchor the piece in instrumental function.

--------------------------------------------------

[09] Negative-prompt discipline
Question: Are negatives cleaning one parasite or replacing the whole prompt?
Why it matters: Negative cleanup helped sometimes, but it was not the main driver of strong results.
Pass looks like: One or two surgical exclusions.
Fail looks like: A long blacklist trying to control the whole song by negation.
Repair move: Reassert the positive identity first; only then exclude one recurring wrong turn.

--------------------------------------------------

[10] Workflow routing
Question: Is this actually a prompt problem, or is it an edit/remix/source-preservation problem?
Why it matters: A large share of modern Suno control lives in native workflows now.
Pass looks like: Fresh prompt for new song creation; native workflow for covers, endings, source preservation, stems, or voice reuse.
Fail looks like: Trying to solve an edit task with endless generation prompts.
Repair move: Route correctly: prompt, upload, cover, extend, add vocals, add instrumental, stems, or voices.

--------------------------------------------------

[11] Revision hygiene
Question: Am I changing one meaningful variable at a time?
Why it matters: Dirty tests make it impossible to tell whether the model failed or the prompt changed too much.
Pass looks like: One high-leverage revision per test round.
Fail looks like: Five simultaneous revisions followed by a single judgment.
Repair move: Change one variable and keep a clean record of what changed.

--------------------------------------------------

[12] Species test
Question: If this comes out good, will it still be the right species of song?
Why it matters: A common miss was 'good song, wrong target.'
Pass looks like: The spine clearly points to the intended song body.
Fail looks like: The prompt could produce several neighboring but wrong song species and still seem successful.
Repair move: Rebuild the front-person, engine, and payoff around the true target, not just the vibe.

--------------------------------------------------

==================================================
FAST LINT DECISION
==================================================

If 3 or more checks fail:
- do not generate yet
- rebuild the spine first

If the prompt passes most checks but one hard boundary remains:
- ask whether this is actually a workflow problem instead of a prompt problem

If the prompt is already clean and the model still misses:
- classify the miss
- use the troubleshooting matrix
- stop rewriting random adjectives

The clean repair order is:
1. front-person
2. motion engine
3. payoff
4. flourish
5. field split
6. routing

==================================================
IVA. NOT EVERY MISS IS A BAD PROMPT
==================================================

Keep this distinction explicit.

A miss can happen for at least four different reasons:

1. Prompt weakness
The prompt is too vague, too broad, too overloaded, or too internally conflicted.

2. Model-boundary miss
The prompt is reasonable, but the ask sits in a weak-control zone:
- odd meter
- strict BPM obedience
- section-perfect fidelity
- instrumental purity
- stable ensemble occupancy
- exact source preservation

3. Attractor miss
The model solves the easier neighboring version of the song.
This is the classic:
good song, wrong target.

4. Workflow-routing miss
The task was really an edit, preservation, or transformation problem, but it was approached like a fresh generation prob... (17 KB left)
