# Text Strategy / 文字策略

Use this reference whenever the cover title (and optional sub line) matters — which is almost always.

Cover Pop dies two ways with text: **too little** (pretty image, no readable promise) and **too much** (paragraph on a thumbnail). The model should generate only the text the **image itself** must own.

## Title Budget

| Line | Budget | Role |
| --- | --- | --- |
| Main title | **≤ 15 字** (prefer ≤ 12 for search thumbs) | the one promise / hook |
| Optional sub | **≤ 10 字** | qualifier, audience, or second beat |
| Everything else | **0** inside the image | body, hashtags, CTA → outside |

Do not stack three formulas. One main line earns the tap; a sub is optional, not a second essay.

## Native Text Is Mandatory

Default for all cover roles except "center image for a card":

- the generated cover **contains** the final Chinese/English title as designed typography in the pixels
- post-overlay / empty title block is **not** the default
- only use empty title block when the user explicitly asks for editable / post-production text

## Exact Text Block

For final prompts, state:

```text
Exact text: render EXACTLY these characters as the main title: "{title}".
Optional sub line: "{sub}" or omit entirely.
No other text, no fake paragraphs, no watermark, no "限时" badge, no invented numbers.
Heavy weight, high contrast, readable at ~200px thumbnail width.
```

If the user locked a title, do not "improve" the wording in the pixels. If you propose a better title, get acceptance (or state the proposed line in the plan) before generating.

## Good Title Shapes

Prefer titles that:

- name a reader or situation
- promise one concrete payoff
- open one curiosity gap
- survive squint / thumbnail transcription

Avoid:

- full sentences that wrap into three lines
- abstract vibe words with no payoff
- stacked formulas (数字 + 人群 + 反常识 + emoji)
- tiny captions on busy photo texture
- English stage jargon on a Chinese cover unless the audience is bilingual and the user asked

See also `title-formulas.md` for formula banks; this file owns budget, ownership, exactness, and repair.

## Text Ownership Split

### Image Owns (default)

- main title
- optional sub
- any number / claim / name that appears on the cover art

### Outer Layout Owns

- note / article body
- caption under the post
- hashtags
- CTA / follow copy
- author note
- platform metadata

### Center-Image Exception

When the role is "center image for a card," the outer card owns title/subtitle. Keep the image text-empty or label-only.

## Repair Policy (Garbled Chinese)

If the cover is good but title glyphs are wrong, melted, doubled, or gibberish:

1. One regeneration with a stricter exact-text block and a quieter title plaque / solid block.
2. Shorten the main line (≤ 10 字) and increase weight / contrast; move off busy texture.
3. If Chinese is still unstable **and** the user explicitly allows post-production text, regenerate with an empty title block of the right shape/size and overlay exact text in post — note this in the output contract.
4. Do **not** silently accept misspelled or invented title characters on public / showcase / client covers.

## Anti-Patterns

- blank cover "so text can be added later" without an explicit user request
- stuffing title + subtitle + three badges + a paragraph into one 3:4 frame
- changing locked title characters to "look better"
- inventing `100万粉同款` / `月入3万` / rankings the note does not support
- relying on platform caption to carry the only promise while the image is mute
