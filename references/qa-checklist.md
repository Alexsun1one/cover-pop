# QA Checklist

## Accept

For the image group below, every PASS must be justified by something visible in the rendered
file, not by what you intended. If your only evidence is the prompt you wrote, the item is
UNVERIFIED — regenerate or inspect, do not accept.

### Asset routing & ownership (plan + render)

- An **asset role** was chosen (xhs note cover / wechat OA header / douyin-video thumb / moments share / search-result thumb / center image for a card) per `asset-routing-and-truth.md`.
- This is still a **cover** job — if it should be quote-cards / sticker-set / paper-operators / busy-town / lego-town / a logo, **reroute** instead of accepting.
- **Text ownership** matches the role: title in-image by default; center-well images do not stuff a full headline the outer layout will duplicate.
- **Exact title truth**: every on-cover character matches the locked/accepted title; no invented numbers, rankings, prices, or claims (`text-strategy.md`).

### Layout / ratio

- **Platform ratio** matches the ask (default 小红书 **3:4**; OA / video / Moments per `layout-handoff.md`) — do not stretch later.
- Title and focal subject sit in the **central ~70%**; critical glyphs are not flush to edges that feed/search crops will cut.
- Any caption / body / hashtags / CTA stay **outside** the image.

### Failure pattern scan

Before accept, name-check `failure-patterns.md`. Fail (regenerate or reroute) if any is present:

- clickbait empty promise
- 微商风
- AI plastic / melted glyphs
- unreadable thumb title
- clutter / stacked archetypes
- wrong platform ratio
- wrong owner
- truth drift on title or claims

### Check the RENDERED IMAGE (look at the file)

- **Squint test (must view, not recall):** produce an actual 200px-wide downscaled copy of the
  rendered cover and look at THAT, not the full-size image or your prompt. From the thumbnail
  alone, transcribe the main line character-by-character and name the one promise. PASS only if
  (a) every Chinese character you transcribe matches the intended title exactly, and (b) you can
  name the promise without zooming. If you cannot generate or view a real thumbnail, you have not
  run this test — do not check it off; repair or regenerate the native title and retry.
- The Chinese characters are correct — no melted, doubled, or gibberish glyphs.
- There is exactly one focal subject — not a collage of everything.
- The palette is restrained: one base, one accent, one ink.
- The composition has breathing room; the title is not crammed edge to edge.
- The aspect ratio matches the platform (小红书 3:4 by default).
- If this is a README/gallery/showcase image, it looks like a real publishable cover for a real niche, not only a meta-ad for the tool.
- **Real-account test (name one, decide save-or-scroll):** name ONE specific real account in this
  exact niche (a real handle/博主名, e.g. a real 小红书/公众号 account you can point to — not "a
  typical 知识博主"). Imagine this cover sitting in that account's grid between two of their real
  posts. Give a one-word verdict: "belongs" or "amateur". It is "amateur" (regenerate) if ANY of
  these is true: the title font is lighter or busier than theirs, the palette has more colors than
  theirs, or a follower scrolling their grid would read this as an ad. If you cannot name a real
  account, you do not know the niche's bar — stop and find one before accepting.

### Re-confirm against the PLAN (must still hold post-render)

- There is exactly one promise.
- The promise is real: there is something behind the tap.
- The archetype matches the topic's job.
- A target reader scrolling past would plausibly stop and tap.

## Regenerate

- The title is unreadable at thumbnail size, mangled, or cut off.
- The characters are wrong, doubled, or partly gibberish — or diverge from the locked exact title.
- On-cover numbers/claims were invented or altered (truth drift).
- The promise is empty clickbait with nothing behind it.
- It reads as 微商: gold-red glow, sticker pile, fake urgency badge, QR cram.
- It reads as 土味: WordArt, bevel, neon-on-neon, double drop shadow.
- It reads as a PPT title slide or a stock photo with a color bar slapped on.
- It shows AI plastic: extra fingers, waxy skin, melted text, hallucinated logos.
- It is a cluttered collage with no focal point.
- Two or three archetypes are stacked onto one cover.
- The platform ratio is wrong for the asset role.
- The job belongs to another skill (wrong owner) — reroute instead of polishing.
- It is pretty but says nothing.

## Repair Moves

If the title text is wrong (most common):

```text
Re-render the title as EXACTLY "{correct text}" with clean correct Chinese characters,
heavy and readable at thumbnail size. Keep the composition. Remove any extra hallucinated
text or watermark. If clean text is still impossible, shorten the title and regenerate with
stronger type constraints; use an empty title block only when the user explicitly asks for
editable/post-production text.
```

If it looks 微商 or 土味:

```text
Regenerate clean and premium: one base color, one accent, one ink. Remove glow, stickers,
sparkles, urgency badges, WordArt, and double shadows. Put the title on a solid block or
clean photo area with breathing room.
```

If it is cluttered:

```text
Regenerate with one focal subject and one promise. Cut everything else. Give the title a
calm zone with generous margins.
```

If the promise is empty:

```text
Rewrite the title to name the specific reader and one concrete payoff, then regenerate.
The tap must lead to something real.
```

If the title is unreadable at thumbnail size:

```text
Shorten the main line to ≤ 10 字, increase weight and contrast, move it off busy texture
onto a solid block. Push secondary info to a smaller sub-line.
```

Only use an empty title block plus external overlay when the user explicitly requests an
editable/post-production route. For normal covers, native rendered title typography is part
of QA.
