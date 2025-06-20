Below is a consolidated reference sheet you can keep on-hand while prompting AI Music Lab.
It is split into Country and Hip Hop sections and shows every practical knob you can turn with [square-bracket tags] (global or sectional instructions) and (parenthetical inserts) (ad-libs, spoken asides, background parts).
Examples use neutral wording; swap in your own lyrics after the tags.

⸻

1  General Tagging Rules

Convention	What the engine does	Notes
[ … ]	Sets style, instrumentation, mix, or performance for the section that follows until the next tag	Works at song level if placed before the first line
( … )	Generates simultaneous or “layer-behind” vocals, ad-libs, crowd shouts, FX, or spoken lines	Good for call-and-response, hype tracks, or harmony pads
[Verse] / [Chorus] / [Bridge] / [Solo]	Explicitly marks structure; engine respects the label when arranging	Optional but helps keep long prompts organized
Multiple tags	Stackable; engine applies all (e.g., [BPM:95][Key:G][Twang Male Vocal])	Order does not matter
Capitalization	Tag names are case-insensitive	

(Parentheses as backing vocal markers are confirmed behaviour in tools like Suno; brackets override tone and mix settings.)  ￼ ￼

⸻

2  Country – Exhaustive Capability Menu

a) Core Style / Tempo / Key

[Genre: Country]        # forces Nashville / modern country palette  
[BPM: 72]               # slow ballad range (65-80)  
[BPM: 96]               # mid-upbeat radio feel (85-100)  
[Key: G Major]          # specify tonality; works with minor keys too  
[TimeSig: 3/4]          # for a waltz - optional  

b) Instrumentation Tags

[Instruments: AcousticGtr, ElectricGtr-Clean, PedalSteel, Fiddle, Banjo-Lite, UprightBass, BrushedDrums, HandClaps, Whistle]  

You can list any mix; leave out Banjo to avoid bluegrass.

c) Lead & Harmony Vocal Controls

[Twang Male Vocal]               # warm, lightly nasal delivery  
[Female Harmony Bright]          # high third-above harmony on choruses  
[Dual Lead: Male+Female]         # trades lines  
[Choir: Small Crowd]             # gang-style singalong refrains  
[Accent: Midwestern US]          # adjusts phonetics  

d) Lyrical / Thematic Modifiers

[Americana Imagery High]         # engine peppers porch, highway, small-town lines  
[Storytelling Verse]             # narrative phrasing, vivid detail  
[CallAndResponse: “Yee-haw!”]    # auto-injects shout before each chorus  

e) Mix & FX

[Reverb: Plate-Medium]  
[Delay: Slapback-75ms]           # classic Sun Records slap  
[Panning: AcousticGtr-L30, Fiddle-R25]  
[MasterEQ: WarmLowMid]  

f) Background / Ad-Lib Syntax

(whistle hook)                  # a melodic whistle layer  
(spoken: “Let’s ride!”)         # one-shot voice-over  
(Yee-haw!)                      # crowd shout on beat  

g) Full Prompt Template (swap in your own lyrics)

[Genre: Country][BPM:92][Key:D Major][Twang Male Vocal][Female Harmony Bright]
[Verse]
I left my boots by the back door, sunrise paintin’ gold across the corn
(Mm-hmm)
[Pre-Chorus][HandClaps][CallAndResponse:"Hey!"]
[Chorus]
(Choir: Small Crowd)  
This red, white, and restless heart keeps rollin’ on  
...
[Bridge][PedalSteel Solo]
...


⸻

3  Hip Hop – Exhaustive Capability Menu

a) Core Style / Tempo / Key

[Genre: HipHop]                # default modern kit  
[SubStyle: BoomBap]            # or JazzRap / Trap / WestCoast / Drill  
[BPM: 88]                      # radio mid-tempo (80-95)  
[BPM: 74]                      # slow head-nod pocket  
[Key: D Minor]  
[Shuffle: 55%]                 # swing feel for drums  

b) Instrumentation & Beat Elements

[Instruments: 808Kick, Snare-Crack, HiHat-Trap-Triplet, UprightBass-Sampled, RhodesPiano, JazzSax, VinylScratch, HornStabs, StringPad]  
[BeatBreak: 4bar-DJcut]        # inserts drumless break for rap focus  

c) Vocal & Flow Controls

[Lead Rap: Deep Male]              # baritone flow  
[Lead Rap Alt: Aggressive Female]  # swap or double verses  
[Hook Vocal: Sultry Female]        # R&B style sung chorus  
[Bridge Vocal: High Male Falsetto] # radio yet soulful  
[Stacked Adlibs: Stereo]           # panned hype echoes  
[FlowStyle: TripletTrap]           # vs BoomBapLinear / Mumble / FastDoubleTime  
[AutoTune: Light]                  # subtle pitch correction on sung parts  

d) Lyrical / Thematic Modifiers

[Mood: Swagger+Dark]               # tonal vocabulary shift  
[JazzyChords High]                 # extended 7ths & 9ths in keys  
[GangVocals: “Yeah!”]              # crowd stabs every 2 bars  
[WordplayDense]                    # multisyllabic, internal rhyme focus  

e) Mix & FX

[Sidechain: Kick-Bass-3dB]  
[Reverb: Room-Tight on Vox]  
[Delay: Quarter-Note Throw on last word]  
[VinylCrackle: Low]  
[MasterBus: TapeSaturation-Soft]  

f) Background / Ad-Lib Syntax

(yeah, uh-huh)                 # hype ad-lib  
(whisper: “count it up…”)      # panned whisper  
(crowd chant: “Chi-Town!”)     # one-shot chant sample  
(SaxSolo 8 bars)               # inserts improvised sax riff  

g) Full Prompt Template

[Genre: HipHop][SubStyle: JazzRap][BPM:90][Key:F Minor]
[Lead Rap: Deep Male][Hook Vocal: Sultry Female][JazzyChords High][VinylCrackle:Low]
[Verse 1]
Strollin’ State Street, dusk on my chain—
(yeah)
Rhodes keys drippin’ under vinyl rain…
[Hook]
(gospel choir pad)
She said “time ain’t nothin’ when ya own the clock,”
Sax moans while the 808 knocks…
[Bridge][High Male Falsetto][AutoTune:Light]
...


⸻

4  Quick Reference – All Tag Categories at a Glance
	•	Global/Section Tags: [Genre:] [SubStyle:] [BPM:] [Key:] [TimeSig:] [Mood:] [Storytelling:] [WordplayDense]
	•	Instrumentation: [Instruments: …] [SaxSolo] [BeatBreak] [GuitarSolo] [PedalSteel Solo]
	•	Voices: [Lead Rap: …] [Twang Male Vocal] [Female Harmony Bright] [Hook Vocal: …] [Choir: Small Crowd]
	•	Flow/Tone: [FlowStyle:] [AutoTune:] [Accent:] [CallAndResponse:]
	•	Mix/FX: [Reverb:] [Delay:] [Sidechain:] [Panning:] [MasterEQ:] [VinylCrackle:] [TapeSaturation:]
	•	Parenthetical Inserts: (spoken: …) (whisper: …) (crowd chant: …) (Yee-haw!) (yeah!)

Use these menus to build prompts that hit precisely the pace, instrumentation, vocal texture, and Americana or jazzy swagger you outlined. Drop me the sections you want expanded or any new style mash-ups, and I can draft full prompts or troubleshoot further.