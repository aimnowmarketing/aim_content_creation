---
name: blog
description: Write a blog post in the user's voice. Use when the user asks to draft a blog post, article, or long-form written piece. Pulls voice, stories, beliefs, stats, humour, and vocabulary from the me/ context files.
---

# /blog — Blog post in your voice

Use this skill any time the user asks you to draft a blog post, article, or long-form written piece. Output is ready to publish or paste into a CMS.

## Step 1 — Load the user's voice

Always read these files first (they live in the `me/` folder at the root of this project). Do not guess the user's voice — pull from source:

1. `me/identity.md` — who they are, what they sell
2. `me/business-context.md` — AIM and ADVAN services, differentiators, proof points, and case studies
3. `me/tone.md` — how they write
4. `me/vocabulary.md` — words they use + words to avoid
5. `me/humour.md` — how they joke
6. `me/beliefs.md` — their hot takes / positions
7. `me/stories.md` — anecdotes they tell
8. `me/data.md` — numbers they name-drop
9. `me/analogies.md` — metaphors they use

Also read `examples/blog-example.md` for the canonical post structure (if it exists).

## Step 2 — Ask only what you can't infer

If the user gave you a topic, run with it. Only ask if it's genuinely ambiguous (e.g., "write a blog about AI" — clarify angle). Default to action over questioning.

## Step 3 — Post structure

Every post needs three things: a clear entry point, at least one real example, and a place where it lands. Everything between those three should vary by topic, tone, and length. Do not follow a fixed template.

- **Title** — specific, benefit-driven or curiosity-driven. No clickbait. Real numbers or bold claims where applicable.
- **Entry point** — can be a provocative statement, mid-story drop, a direct question to the reader, a surprising stat, or a blunt observation. No "In today's fast-paced world" openers. No two posts should open the same way.
- **Body** — the order of sections should feel driven by the argument, not a template. Mix short punchy paragraphs with the occasional longer one. Not every section needs a subheading. Not every post needs a checklist — use one only if the topic genuinely calls for it, not as a default format.
- **Real example** — at least one story or case study from `me/stories.md` embedded where it earns its place, not dropped in at a predictable "proof point" position.
- **Landing point** — can be a quiet confident close, a reframe, a direct CTA, or simply the post ending when the point has been made. Not every post needs a formal CTA. Sometimes ending on a strong thought is enough.

**Deliberately break the rhythm in at least one place per post.** Let a thought restart. Let a section feel slightly unresolved. Let one paragraph run longer than expected, or cut one shorter than feels complete. A post that flows perfectly from start to finish reads like a template, not a person.

## Step 4 — Voice rules (non-negotiable)

- Match the user's default voice from `me/tone.md`. Never sound generic.
- Use their sentence rhythm, not yours.
- Drop in their real numbers from `me/data.md` — never invent stats.
- Self-deprecation, humour, and profanity should match the levels defined in `me/humour.md` and `me/vocabulary.md`.
- Banned words from `me/vocabulary.md` are a hard filter. Scan the draft and remove every instance before delivering.
- End with a clear next step or a quietly confident line.

### Anti-AI-detection rules (apply to every post)

**1. Rough up the numbers.**
Use a maximum of 2–3 stats per post. Do not weave all available data points in cleanly. Drop at least one number mid-sentence without setup or fanfare — the way a founder would mention it in conversation, not the way an analyst would frame it in a presentation. Occasionally add a qualifier that introduces natural uncertainty: "somewhere around 40% in most cases", "closer to 5x depending on the category", "last time we checked, it was sitting at about 42%." This sounds human. Perfectly rounded, cleanly cited stats in every section do not.

**2. Break the structural predictability.**
Do not produce Hook → Problem → Why → Checklist → Pitch → Case Studies → CTA. That is a template AI detectors are trained to recognise. Vary the entry point, the order of ideas, and the close. Skip the checklist format unless it genuinely serves the post. Let the argument drive the structure, not the other way around.

**3. Vary the pacing deliberately.**
Not every paragraph should be 2–3 sentences. Not every section should land cleanly. Let one section run longer. Cut one shorter than expected. Let a sentence start one way and correct itself. A post with perfectly balanced pacing across every section signals assembly, not writing.

## Step 5 — Banned words (hard filter)

Before returning the draft, scan against `me/vocabulary.md` § "Banned words" section and remove every instance. Common AI-sounding offenders to watch for:

delve, tapestry, realm, testament, navigate (as verb), robust, leverage (as verb), synergy, holistic, ecosystem, bespoke, elevate, unlock, streamline, game-changer, moving forward, circle back, touch base, low-hanging fruit.

Also avoid emoji spam unless the user's style explicitly uses them. Match their emoji usage from `me/tone.md`.

## Step 6 — Length & format

- **Default:** ~1200 to 1500 words. Long enough to deliver real value, short enough to read in one sitting.
- **Short take / opinion piece:** ~200–400 words — hook + core argument + close.
- **Long-form / deep dive:** 1000 to 1100 words — full story arc with subheadings, examples, and numbered takeaways.

Default to long-form when the topic is a case study, how-to, or result reveal. Default to short when it's an opinion or quick take.

## Step 7 — Deliver

Output the post as a plain markdown code block (so the user can copy it cleanly). Below the post, in 1–2 lines, note:

- Which story / stat you anchored on
- One alternate opening the user can swap in

Do not write a preamble. Do not explain the post. Just deliver it.

## Topic-to-story mapping

<!-- After filling in me/stories.md and me/data.md, add shortcuts here so the AI knows which stories pair with which topics. Example format: -->

<!-- - **Websites / conversion** → [story name] + [stat from data.md] -->
<!-- - **Getting started / fear** → [origin story] + [lowest point numbers] -->
<!-- - **Your product / tools** → [product story] + [result stat] -->

## What success looks like

Reader can tell within the first paragraph who wrote this. The post lands a real number, tells one true story, and ends with a clear next step. Nothing in it sounds like it was written by an AI.
