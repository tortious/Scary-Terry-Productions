Grok “Imagine” — Complete Styling & Troubleshooting Guide (2025)

Below is a consolidated, field-tested guide for Grok’s Imagine (xAI) covering apparel/product styling, general creative subjects, safe alternatives for sensitive themes, and a hands-on troubleshooting playbook. Prompt blueprints are copy-paste ready.

⸻

What “Imagine” is (and how to access it)
	•	In the Grok app: Imagine generates images and can animate a still into a short clip with sound (beta). Musk frames this as an “AI Vine” revival; modes reported include Normal, Fun, Custom, Spicy for animation. Availability has rolled out via Grok’s mobile apps for paying tiers, with staggered early access on Android.  ￼ ￼
	•	In the API: Image generation uses POST https://api.x.ai/v1/images/generations with model grok-2-image. You send a single prompt and can request n images (1–10). Responses return image URLs or base64 and include revised_prompt (the system-rewritten prompt actually used by the model). Parameters like quality/size/style aren’t supported at the moment.  ￼
	•	Image understanding (analysis, not generation): A separate Image Understanding guide lets you read/critique an image (base64/URL) via the chat route; helpful before you iterate a design.  ￼

⸻

Prompting fundamentals that matter most (for Grok)
	1.	One primary subject (“single subject centered”) + clean background.
	2.	Camera & light drive realism: e.g., 50 mm lens, f/2.8, studio softbox key + rim.
	3.	Material truths: exact fabric/leather/weave, finish (matte/satin/gloss), stitch density, grain.
	4.	Color by hex or canonical names (e.g., deep navy #0a1a2f).
	5.	Composition & angle: 3/4 hero, top-down lay-flat, orthographic front & side.
	6.	Negatives inline: Write “exclude … / without …” inside your prompt (no separate negative-prompt field). Check revised_prompt in the API response to see what stuck.  ￼
	7.	Generate multiples (n 4–10) and pick a keeper for iteration.  ￼

⸻

Apparel / Product Styling

Shoes (sneakers, boots, dress shoes)

Blueprint — product sheet (hero + detail macro):

“Single subject product design board — [category]; silhouette: [sleek/retro cupsole]; last shape: [narrow/regular/wide toe]; upper: [engineered mesh / full-grain leather / knit] with [TPU overlays / brogue perforations]; midsole: [sculpted EVA w/ visible gel]; outsole: [waffle traction, flex grooves]; colorway: [primary] w/ [secondary] accents; branding: minimal geometric logo; stitching: [double-row lockstitch]; finish: [matte]; angle: 3/4 hero, floating; lighting: studio cyclorama, softbox key + rim; lens: 50 mm, f/5.6; background: seamless light gray #f5f5f5; include heel close-up & outsole tread macro; exclude human models, dust, motion blur.”

Useful alternates:
	•	Lifestyle on-foot: “urban concrete, golden hour rim light, shallow DOF, candid stride.”
	•	Exploded view: “exploded layers separated 2 cm, no text labels, clean separators.”

⸻

Suits (tailoring)

Blueprint — lookbook plate:

“Menswear lookbook plate, single model, two-piece suit; cut: [soft-shoulder Neapolitan / structured British]; lapels: [peak 9 cm]; canvas: [full canvas]; vents: [double]; trousers: [single pleat, slight break]; fabric: [Super 120s worsted, mid-weight]; pattern: [navy pinstripe 1.5 mm]; shirt: [white poplin, spread]; tie: [grenadine navy]; pocket square: [white TV fold]; shoes: [black cap-toe oxford]; lighting: neutral studio; lens: 85 mm; pose: relaxed contrapposto; background: seamless gray; exclude harsh wrinkles, moiré, exaggerated padding.”

Add a detail plate: lapel roll, sleevehead, pick-stitch (3 mm), waistband extension.

⸻

Shirts (casual & dress)

Blueprint — flat lay + on-model:

“Apparel product sheet: button-down shirt; fabric: [oxford/poplin/linen], weave: [basket/plain], weight: [light/mid], pattern: [micro-gingham 3 mm]; collar: [button-down/cutaway]; cuffs: [barrel, single]; placket: [French/standard]; hem: [curved]; color: [heathered sky blue #8dbbe9]; stitch density: [16 SPI]; buttons: [mother-of-pearl]; images: lay-flat front/back + on-model straight-on; lighting: soft top light; background: white cotton paper; exclude pins, tags, heavy wrinkles.”

⸻

Watches (product & wrist-shot)

Blueprint — product hero (dial forward):

“Watch product hero, single subject; style: [field/diver/dress/pilot]; case: [39 mm, brushed 316L, polished chamfers]; bezel: [coin-edge 60-click]; crystal: [double-domed sapphire, inner AR]; dial: [sunburst forest green]; indices: [applied baton]; hands: [dauphine, BGW9 lume]; complication: [date at 6]; strap: [20 mm leather, taper 20→16]; caseback: [sapphire exhibition]; angle: 3/4, crown at 3; lighting: softbox + specular kicker on chamfers; background: gradient charcoal; exclude dust, fingerprints, exaggerated reflections.”

Blueprint — wrist-shot:

“Natural wrist-shot, open shade, 50 mm, f/2.8, realistic skin texture & hair; exclude warped lugs, melted hands; mild bokeh background.”

⸻

General Creative Subjects

Masks

Blueprint — catalog grid:

“Mask design grid, 4 variants; type: [Venetian half-mask / gas mask / Noh / luchador]; materials: [lacquered papier-mâché / ABS / carved wood]; finish: [matte black / gold-leaf crackle]; strap: [adjustable leather]; motif: [baroque scrollwork / geometric]; neutral turntable views (front/side/3/4), white cyclorama, even lighting; exclude human faces.”

⸻

Tattoos

Design sheet (for artists):

“Tattoo flash sheet, vector-clean linework; style: [traditional / neo-traditional / blackwork / geometric / irezumi]; subject: [koi & peonies]; line weight: [6 pt outer / 3 pt inner]; shading: [stippling]; palette: [red/black/cream]; plain white background; no text.”

On-skin preview (photo look):

“Photorealistic arm with half-sleeve, style: black & grey realism; motifs: [compass, roses, pocket watch]; ink: healed look; lighting: soft window light; exclude blowouts, raised welts.”

⸻

Famous people (ethics & technique)
	•	Use inspired-by era traits (“1964 mop-top suit, narrow tie, monochrome studio light”) or celebrity-inspired look-alike phrasing rather than naming a living person, especially in sexualized contexts.
	•	Reports show Imagine includes a “Spicy” option with looser NSFW behavior; that raises clear ethical and legal concerns (non-consensual deepfakes, minors, reputational harm). If you depict recognizable people, keep it non-exploitative and clearly label AI output.  ￼

⸻

Historical people / figures
	•	Anchor to period media & process for authenticity: “wet-plate collodion portrait, 1860s lighting; lens aberrations; plate-edge vignetting.”
	•	Specify attire/insignia/artifacts accurately (e.g., lorica segmentata, Tudor doublet, Meiji cap) and period-correct lighting/film.

⸻

Unique Instances (safe alternatives you can actually ship)

I won’t help generate explicit sexual content or graphic gore. These patterns evoke intensity while staying within safe bounds.

Violence / Horror (without graphic gore)

What to avoid: wounds, explicit injury shots, gore.
Levers instead: aftermath, implication, environmental storytelling, high-contrast light, occlusion.

Blueprints:
	•	Horror suspense, no gore
“Suspenseful hallway without blood or visible harm; half-open door, cool moonlight slicing across floor; heavy shadows suggest figure off-frame; low angle 50 mm; cinematic contrast; minimal set dressing (broken frame, single shoe); exclude graphic injury/gore.”
	•	Crime aftermath, implied
“Forensic tableau without graphic details; night rain in city alley; scene tape lit by streetlamp; evidence markers near shattered phone; long-lens distance, blue-red emergency bokeh; exclude bodies, wounds, gore.”
	•	Stylized tension
“Expressionist shadow study on a staircase; hard uplight; monochrome with one red accent; implied danger only, no wounds or gore.”

Fix drift: End with “no wounds, no blood, no gore, no explicit harm.”

⸻

Adult themes / sensuality (non-explicit)

What to avoid: explicit sexual acts, pornographic detail, fetish content, minors.
Levers instead: wardrobe coverage, fashion focus, suggestive but PG-13 body language, soft lighting, mid/three-quarter crops.

Blueprints:
	•	Glamour portrait (PG-13)
“Editorial glamour portrait, closed satin robe with structured shoulders, statement earrings, soft window light, shallow bokeh; elegant pose, confident expression; non-explicit, tasteful coverage; neutral studio; exclude nudity/explicit content.”
	•	Romantic fashion look
“Couple in evening wear at blue hour, city-lights bokeh; tailored suit + floor-length dress, gentle hand-hold; cinematic rim light; non-explicit; wardrobe-first; exclude explicit sexual content.”
	•	Boudoir-inspired product focus
“Silk slip fully covered beneath tailored blazer; emphasis on drape & jewelry; soft sidelight, fine grain; non-explicit.”

Guardrails to add: “non-explicit; fully covered; fashion editorial; exclude nudity, pornographic content, fetish detail.”
Why strict? Imagine’s “Spicy” mode has prompted safety complaints and calls for investigation. Stay far from the line.  ￼

⸻

Troubleshooting & Pro Moves

Photorealistic vs stylized
	•	Photorealistic: add camera words (DSLR, 50 mm, f/2.8, ISO 200), lighting (3-point studio / open shade), surface cues (skin texture, micro-contrast, color-accurate product shot), plain background.
	•	Stylized: lead with medium (vector flat, cel-shaded, watercolor, oil impasto, clay stop-motion, low-poly 3D). Add render cues (no photographic grain, inked outlines, paper texture).
(Style is controlled by words; there’s no style/size/quality parameter today.)  ￼

Prioritizing features (so Grok doesn’t “forget”)
	1.	Front-load hard constraints in a short first sentence. 2) Use atomic phrases (e.g., “peak lapels 9 cm; full canvas; pinstripe 1.5 mm”). 3) Add a brief exclude clause for deal-breakers. 4) Inspect revised_prompt from the API and re-phrase dropped items more concisely.  ￼

Common mistakes to avoid
	•	Over-stuffing: pick 3–5 must-haves.
	•	Conflicts: don’t ask for matte and high-gloss simultaneously.
	•	Expecting perfect logos/text: generate blank products; add brand marks in post.
	•	Busy backgrounds that steal attention.
	•	One-shot expectation: use n up to 10, select, then tighten.  ￼

Tricks that consistently help
	•	Two-pass flow: broad look → tighten from a keeper.
	•	Angle pairs: ask for two views in one prompt (front + 3/4, lay-flat + on-model).
	•	Macro inserts: “include macro of [stitching/grain/bezel knurling].”
	•	Lighting swaps: same subject, different light to test realism.
	•	Neutral gray backgrounds to stabilize color.

⸻

Ready-to-Paste Prompt Library

Shoes — lifestyle on-foot

“Single subject on-foot streetwear shot, low-top knit runner, sculpted EVA midsole, waffle outsole, obsidian #0a0a0a with volt accents, 3/4 angle mid-stride, shallow DOF, golden-hour rim light, 50 mm, color-accurate, exclude logos/text.”

Suit — studio lookbook

“Lookbook plate, two-piece navy pinstripe (1.5 mm), soft shoulder, peak lapels 9 cm, full canvas, trousers single pleat slight break, white poplin spread, grenadine navy tie, black cap-toe oxford, seamless gray, 85 mm, neutral temp, exclude moiré/harsh wrinkles.”

Shirt — flat lay + on-model

“Product sheet: oxford button-down, heathered sky blue #8dbbe9, button-down collar, barrel cuff, French placket, 16 SPI, MOP buttons, lay-flat front/back + straight-on on-model, paper-white background, soft top light, exclude pins/tags.”

Watch — product hero

“Dress watch, 39 mm 316L brushed w/ polished chamfers, sunburst forest-green dial, applied baton indices, dauphine hands BGW9, date at 6, double-domed sapphire inner AR, 20 mm leather strap taper 20→16, 3/4 angle crown at 3, softbox + specular kicker, gradient charcoal, dust-free.”

Mask — catalog grid

“Grid of 4 Venetian half-masks, lacquered papier-mâché, gold-leaf crackle, adjustable leather strap, baroque scrollwork, front/side/3/4 views, white cyclorama, even soft light, no human faces.”

Tattoo — flash sheet

“Tattoo flash, neo-traditional, koi & peonies, bold 6 pt outer / 3 pt inner, limited palette red/black/cream, vector-clean linework, plain white background, no skin, no text.”

Historical portrait (period look)

“19th-century wet-plate collodion portrait style, shallow DOF, lens aberrations, edge vignetting, period-accurate attire/insignia of [figure/role], neutral seated studio pose, subdued expression.”

⸻

API quick reference

cURL (request 4 options at once):

curl https://api.x.ai/v1/images/generations \
  -H "Authorization: Bearer $XAI_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "grok-2-image",
    "prompt": "Dress watch, 39 mm 316L... [your prompt here]",
    "n": 4,
    "response_format": "url"
  }'

Then read revised_prompt in the response; if a constraint dropped, shorten it and regenerate. (quality/size/style params aren’t supported.)  ￼

⸻

Safety & attribution notes
	•	Celebrities & public figures: avoid sexualized or defamatory depictions; label outputs as AI-generated. Imagine’s Spicy mode has triggered safety complaints/investigation requests—steer well clear.  ￼
	•	Copyright/logos: generate blank products; add marks in post.
	•	Disclose AI use when publishing.

⸻

Rapid debug checklist
	•	Too cartoony? Add camera/lighting terms; request color-accurate product shot; simplify background.
	•	Details keep shifting? Front-load constraints; use atomic phrases; inspect revised_prompt; regenerate multiples.  ￼
	•	Odd hands/faces/wrinkles? Reduce pose complexity; 85 mm portraits; soft single-key light.
	•	Colors off? Use hex codes + neutral gray; avoid colored lights.
	•	Messy backgrounds? Ask for seamless cyclorama / plain studio.
	•	Need motion teaser? In-app, animate your best still into a short clip (the “AI Vine” concept).  ￼

⸻

If you want, tell me the first sub-area you’re shipping (e.g., watch product hero or PG-13 glamour suit lookbook). I’ll draft a mini pack with (1) 3 prompt variants, (2) angle/lighting swaps, and (3) a 6-second teaser script.