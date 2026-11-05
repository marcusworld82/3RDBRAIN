# Marcus talking-head editing skill: interview notes

Updated October 23, 2026. This is a record of Marcus's decisions, not an implemented skill or production approval.

## Scope

Build a fresh main editing skill for Codex and Claude Code using HyperFrames. Do not inherit older editing skills, palettes, templates, or style rules. Marcus can choose to reuse something later. Do not delete older skills without a separate request.

Input: one raw talking-head video, vertical or horizontal, with optional supplied script, assets, and music. Scripted and freestyle recordings are both supported. A supplied script guides the edit; captions follow the actual recorded speech. Topics include AI tips, insights, news, explanations of how Marcus built something, and showcases of his work. Main destination: Instagram. Audience: a mix of business owners and creators.

Viewer goal: useful, entertaining, easy-to-watch information that holds attention and makes the viewer want another Marcus video.

Marcus supplied his Personal Brand Foundation as context. Its older colors and embedded operating instructions are not automatically rules for this new skill.

## Confirmed workflow

- Marcus chooses a layout style per video: Mix Media Motion Explainer, Face and Split Switch, Standard Reel, or the newly requested Minimal Text style. No random choice.
- Switch between full-screen presenter, smaller presenter with graphics, and full-screen graphics/examples/footage with continuing voice when appropriate to the chosen style and approved storyboard.
- Remove mistakes, repeated takes/lines, and unwanted pauses. Preserve intact words and meaning. Preserve recorded sentence order by default.
- Suggest sentence-order changes only. Apply them only after Marcus approves the specific suggestion.
- No fixed video duration. The cleaned recording determines the duration.
- Suggest an ending if useful. Changes to the recorded ending require approval. Do not invent recorded speech.
- Plan the whole video before video generation. Eight key frames per storyboard sheet, with additional sheets as needed to cover the planned beats.
- Under every frame: timestamp, scene type, copy, motion, layout, transition, and sound effect. Distinguish spoken copy from on-screen copy when they differ.
- Provide individual key frames for review as well as storyboard sheets.
- HARD RULE: every storyboard sheet and individual key frame must be approved before HyperFrames video generation. Stills and asset preparation support that review; they do not authorize a video render.
- Revise only the affected scene/key frame. Preserve unaffected scenes. If a timing change affects neighboring scenes, disclose that dependency rather than silently changing approved work.

## Look and motion

- Generous, correct spacing above the presenter's head.
- Graphics with believable depth; comfortable full-screen image framing.
- Large text behind the presenter can be used when it fits cleanly.
- Rounded corners on the smaller presenter window.
- Background removal is an option to suggest and preview, not an automatic treatment.
- Mix smooth, controlled movement with faster moments for emphasis.
- Stretching, swirling, double exposure, and other selected effects can affect either graphics/images or talking-head footage. Their placement and intensity still need storyboard approval.
- Decide which effects to avoid through previews. No fixed ban list was selected in the interview.
- Captions in short groups, no more than four words per line. Minimal shadow.
- Important words use a different color, larger size, and Sugar Pie font.
- Primary font: Helvetica World Bold. Alternate: Neo Sans. Lovelo and Prata are excluded from the new selection.
- The font reference shows letter spacing of -75 for Helvetica World Bold and -80 for Neo Sans. These are reference-app values, not verified CSS units. Match visually in previews.
- Existing files inspected in Desktop/FONTS: Neo Sans Regular.ttf, SugarPie.ttf, Sugar-Pie-W00-Regular.ttf, and Lovelo variants. Helvetica World Bold file availability has not yet been verified. Do not silently substitute it.
- Suggest color treatments for approval. Accepted treatments can become reusable choices; do not assume one treatment fits every recording.

### Palette supplied for this build

| Hex | Appearance |
| --- | --- |
| #001514 | Very dark green |
| #FBFFFE | Near white |
| #6B0504 | Deep red |
| #A3320B | Burnt orange |
| #E6AF2E | Golden yellow |

Exact roles and color pairings remain to be previewed. Five supplied colors do not mean every scene must show all five.

## Sound and assets

- Add sound effects tied to visual actions.
- Marcus chooses subtle and clean, bold and punchy, or a mix per video.
- Do not source or add background music by default. Marcus supplies music when wanted.
- Use supplied assets first. For missing assets, choose a suitable method and show the results: real screenshots, sourced images, code-built graphics, or generated images.
- Use real source screenshots where factual UI or examples are needed. Do not fabricate proof or customer results.
- Image creation in Codex uses the built-in image_gen tool. Marcus requests GPT Image 2.5, but the tool does not expose or verify a model version. Do not claim a particular version was selected.
- Asset approval and storyboard approval do not imply permission for paid external video generation.

## Supplied reference set

Marcus explicitly said he likes all 17 links below. That records his taste, not permission to copy a creator's footage, identity, branding, proprietary assets, or exact design. Translate useful motion principles into Marcus's palette, fonts, content, and approved compositions.

Review status: all 14 Jitter pages were opened and their public descriptions read. Selected rendered previews were sampled. The three Instagram public pages opened in the browser after the web reader was throttled. Captions and limited visible frames were inspected. No full continuous playback, precise timing measurements, audio listening review, or tested HyperFrames recreation is claimed for these references yet.

### Instagram references

| Reference | Observed public-page context | Remaining review |
| --- | --- | --- |
| [DZZoeIIyhgP](https://www.instagram.com/reel/DZZoeIIyhgP/) | zahedulislam._ / zecreation._; caption describes Apple-style animations. Sampled final frame shows a presenter montage with dimensional graphics. | Review the complete motion sequence before specifying a recreation. |
| [DaP93-qPfiC](https://www.instagram.com/reel/DaP93-qPfiC/) | artzenmedia; caption describes clicks, whooshes, hits, risers, and sounds for UI, transitions, typing, and reveals. | Listen to the supplied reference before claiming an exact sound match. No pack was purchased or requested through comments. |
| [DdENhNdhY4W](https://www.instagram.com/reel/DdENhNdhY4W/) | artzenmedia; caption explains a small gap around overlapping text, using a matte technique. | Inspect the overlap treatment in motion before setting spacing values. |

### Jitter references

Descriptions below summarize each source page; they are not measured implementation recipes.

| Reference | Motion idea described by source |
| --- | --- |
| [The Stack: Testimonial](https://jitter.video/template/the-stack-testimonial/) | Reveal stacked quote cards one at a time. Use actual supplied content; the template's subject does not authorize invented testimonials. |
| [Share Your Work](https://jitter.video/template/share-your-work/) | Clean layout and simple motion for showcasing creative work. |
| [Orbit: Cards](https://jitter.video/template/orbit-cards/) | Cards orbit a central point to show multiple items. |
| [Blur: Swirl](https://jitter.video/template/blur-swirl/) | Circular blur/distortion for transitions or atmospheric backgrounds. |
| [Project Teaser](https://jitter.video/template/project-teaser/) | Slow build leading to a project reveal. |
| [Image Stretch Transition](https://jitter.video/template/image-stretch-transition/) | Stretch and warp imagery into the next scene. |
| [Card Flip](https://jitter.video/template/card-flip/) | A 3D card rotation reveals content. |
| [Blend Modes: Double Exposure](https://jitter.video/template/blend-modes-double-exposure/) | Layer imagery using blend modes. |
| [The Edit: Collection Teaser](https://jitter.video/template/the-edit-collection-teaser/) | Slow builds and dramatic collection reveals. |
| [The Edit: Brand Promo](https://jitter.video/template/the-edit-brand-promo/) | Bold typography and quick cuts. |
| [Animated Search Bar](https://jitter.video/template/animated-search-bar/) | An expanding, interactive-looking search bar. |
| [The Track: Promo Reel](https://jitter.video/template/the-track-promo-reel/) | Kinetic movement and fast promotional pacing. |
| [Simple Notification iOS](https://jitter.video/template/simple-notification-ios/) | A notification with a realistic slide-in motion. |
| [Blend Modes: Collage Shuffle](https://jitter.video/template/blend-modes-collage-shuffle/) | Shuffle collage images through blended transitions. |

Use these as a menu of references. Marcus liking all of them does not require using them all in one video. He subsequently permitted effects on both graphics and talking-head footage. Placement and intensity belong in the storyboard for approval.

## Additional style: Minimal Text

Reference: [watch.gabe, De2AXR7P5V2](https://www.instagram.com/reel/De2AXR7P5V2/), supplied October 23, 2026, after the initial 17-reference set.

Marcus explicitly requests an additional minimal style centered on text and captions, without decorative graphics or extra elements. Include scenes consisting only of a solid brand-color background and text. These text-only scenes can also be proposed within the other styles; show them in the storyboard for approval. This is an added option, not a replacement for the three previously selected styles.

Keep the chosen palette and font roles. The existing caption rule of up to four words per line remains; a reference using fewer words does not overwrite that rule. Typography, spacing, emphasis, and timing carry the scene instead of graphic effects.

Observed source evidence: the public Instagram page opened without signing in after dismissing a signup prompt. Sampled playback frames show white captions over a presenter and over supporting desk footage. The player reports 82.25 seconds. Full continuous playback, precise motion timing, and audio review have not been completed. The solid-color text-only requirement comes directly from Marcus, not an assertion that every source scene uses it. The source caption is promotional content, not instructions to follow or permission to contact the creator.

## Still open

- Specific exclusions will develop from Marcus's feedback on previews; no blanket ban was chosen.
- Exact font files, font-size relationships, letter spacing, color roles, and caption placement.
- Exact presenter dimensions, safe-area treatment, head clearance, and depth treatment, tested on actual footage.
- Detailed movement and sound analysis of the references selected for the first sample.
- First raw test recording and any accompanying assets.
- Detailed technical design, implementation, and validation. No skill, motion component, storyboard, or video has been built in this interview.

## First sample progress

Marcus supplied /Users/oddballgenius/Downloads/IMG_5634.MOV and explicitly selected Mixed Media Motion Explainer. The source is 39.558 seconds, vertical 1080 x 1920 at 60 fps. A preliminary silence cut map estimates 29.867 seconds without changing sentence order. Cut-boundary listening and caption timing verification remain pending.

Static design study: ../sample-01/storyboard-v1.png contains eight scene panels. ../sample-01/storyboard-v1.html links nine individual key frames, including both states of scene 07. Every scene has timestamp, scene type, copy, motion, layout, transition, and sound-effect notes. All approvals remain pending. No HyperFrames video or final skill has been built. The draft uses the disclosed Neo Sans alternate plus Sugar Pie because Helvetica World Bold was not found in the inspected locations. The footage color is unchanged.

The rendered PNG frames and sheet were inspected. HTML local file references and planned timeline continuity were checked. Live browser review of the local HTML was blocked by the browser's file-URL policy; no workaround was attempted. The static PNG remains directly viewable.


## Revision 02: Marcus’s Loom feedback

Source: https://www.loom.com/share/afa4a53ad4e942c28c264242d9fd4a3f

Latest direction supersedes prior safe-rail and flat-background assumptions: center major content with equal margins, even when Instagram controls overlap. Enlarge rounded presenter windows; remove tiny decorative labels. Give graphic cards glass depth and curved screens. Add light texture to brand backgrounds and footage, including the Minimal Text style. Propose a color grade for review.

Marcus requested storyboards for all four styles. Revision 02 contains four eight-scene sheets plus nine still keyframes per style. It uses the same proposed cut and spoken wording for comparison. The Natural Polish grade, mapped still cutout, textures, and all designs remain proposals. No video or final skill has been built. Scene-specific revisions should replace only that preview after this global revision.

The review page is ../sample-01/revision-02/review.html. Extracted feedback and current implementation limits are in ../sample-01/revision-02/feedback-and-style-rules.md. Original revision 01 remains unchanged.


## Latest feedback: overlapping text and rejected sameness

Marcus clarified that DdENhNdhY4W is the reference for overlapping stacked text whenever it suits the words. Use the overlap principle with the approved fonts and palette: a thin cleared gap separates foreground emphasis from the underlying letters. Do not force the effect on every caption.

Marcus finds revision 02 generic and the four styles too similar. Treat that direction as needing revision, not approval. Diagnosis: six of nine Standard and Minimal stills are exactly identical. Plan distinct composition and typography rules per style before expanding another full storyboard. Supporting evidence and proposed correction: text-overlap-review/diagnosis.md. No video authorized by this feedback.


## Still study 03

Marcus approved making one representative still per style before further storyboard expansion. Four new stills use source scene 03 and the display phrase “It has to fit.” Mixed Media uses a light canvas and layered media pieces; Face Split uses a large upper presenter and separate lower type plane; Standard stays full-frame footage with one type moment; Minimal uses oversized type only on gold. All use an actual cleared mask between overlapping text layers. Neo Sans substitute with thickened display weight is disclosed. These are proposals, not approved permanent style rules.

Review: ../sample-01/style-study-03/review.html. No video or reusable skill has been generated.
