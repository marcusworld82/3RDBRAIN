# Motion vocabulary and tools

## 1. The Motion Cheat Sheet (Notion, by Shaan Johari)

Source: https://app.notion.com/p/oddballgenius/The-Motion-Cheat-Sheet-9b98226e3aa5823082938155f1d57832
Read in full on October 24, 2026. Credit: Shaan Johari (@viashaan). Kept here as a vocabulary reference.

Why it matters: this is the missing "premium" ingredient. Premium motion eases out and settles. Cheap motion is linear or snaps.

### Core eight

| Motion | Looks like | Use for | Note to send |
| --- | --- | --- | --- |
| Linear | Constant speed | Spinners, loops, color shifts | linear timing, constant speed |
| Ease in | Slow start, fast exit | Things leaving | ease in on exit |
| Ease out | Fast start, soft stop | Things arriving | ease out on entry |
| Ease in-out | Slow, fast, slow | Moving between two spots | ease in-out between positions |
| Overshoot | Passes its mark, settles back | Titles with attitude | slight overshoot on the title, about 10% |
| Spring | Soft natural settle | Anything physical | spring settle, low bounce |
| Bounce | Hits, rebounds, lands | Things that drop | bounce on landing, two small bounces |
| Steps | Jumps in ticks | Counters, stop-motion | stepped timing, 12 steps |

### Extras

Stagger (each item starts a beat later), Morph (shape turns into the next), Elastic (wobbles, use sparingly), Hold (nothing moves so people can read), Anticipation (small wind-up first), Follow-through (parts keep moving after the main thing stops), Motion blur (fast moves smear a little).

### Timing starting points

- Small UI moves: 0.15 to 0.3 s.
- Titles and graphics in a video: 0.3 to 0.6 s in, then hold long enough to read.
- Big full-screen moves: 0.6 to 1 s.
- Exits are a little faster than entrances.

### How to write a motion note

1. Name the thing ("the title", not "it").
2. Name the motion from the tables.
3. Give one number (duration, distance, percent, or count).
4. Say what to avoid ("no fade").

Example: "ease out on entry, 0.4s, slight overshoot on the title, no fade".

### Prompt to paste at the start of any animation chat

When we work on motion, describe every move with these words: linear, ease in, ease out, ease in-out, overshoot, spring, bounce, steps, stagger, morph, hold. For each animation you make, list the moves you used with their timing (for example "title: ease out, 0.4s, slight overshoot"), so I can give notes in the same words.

## 2. Prompt Motion

Source: https://prompt-motion.com/
A gallery of motion videos made with Claude, each with the prompt (a few with a skill) behind it. Categories and counts on the page: Product UI 103, Kinetic type 96, Music 49, Particles 43, Shapes 42, Charts 34, Diagrams 31, Characters 27, Photos 23, Phone 22, Code 21.
The prompts sit behind each card and were not in the page text I could read. Use it as a menu to browse, then open the cards that fit.
Most relevant to Marcus: Kinetic type (96) and Particles (43).

## 3. MCP setup (run these on your Mac, not in a cloud session)

These were NOT installed by Claude. They were not run in the cloud session because that would only install them in a temporary container.

```
claude mcp add motionsites --scope user --transport http https://xgdzyqfalbibzelpdpvr.supabase.co/functions/v1/mcp
```

```
npx shadcn@latest mcp init --client claude
```

Run the second one inside your project folder. It sets up the shadcn MCP for that project.
Not verified: whether it also covers React Bits. That depends on registry settings I have not checked.
After installing, restart Claude Code and run /mcp to see which tools each server exposes. Both are third-party, so read what they offer before relying on them.

## 4. Standing rules from Marcus

1. When Marcus says "be creative," pull options from the motionsites MCP, React Bits and Prompt Motion, then show a few strong ones. Never a long list.
2. Use the Motion Cheat Sheet words for every motion note, with a number for each.
3. These libraries feed the build at Style Lab round one and the component library. They are not a reason to add more elements to a scene. Fewer, better.
