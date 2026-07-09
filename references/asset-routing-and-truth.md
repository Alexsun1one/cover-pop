# Asset Routing And Truth / 资产路由与事实约束

Use this reference before Stop Test / archetype / prompt writing. Cover Pop is a **thumb-stopping cover system**, not a general illustration skill. The first question is not "what should it look like?" but "what cover job must this image do on which platform?"

## Core Rule

Keep Cover Pop only when the asset's one job is to **make the right reader stop scrolling and tap**.

If the final need is an article body figure, a quote save-card, a sticker, a logo, a dense infographic, or a multi-panel explainer, do not force Cover Pop to own the whole job. Say the better owner plainly and reroute.

## Asset Roles

Pick one role before choosing archetype or style.

### 小红书笔记封面 (XHS Note Cover)

Default role when the user says 封面 / 小红书封面 / 笔记首图.

- Visual job: earn the tap in a vertical feed / grid.
- Best form: one promise + one focal subject + native title typography.
- Ratio: **3:4 vertical** by default.
- Text ownership: **title MUST be in-image** (native pixels). Caption / note body stay outside.

### 公众号封面 / 头图 (WeChat OA Header)

Use for 公众号封面、推送头图、文章顶图.

- Visual job: stop the thumb in subscription list / timeline preview, then read as a header.
- Best form: strong title zone + calm subject; avoid edge-crammed type (OA crops vary).
- Ratio: often **2.35:1** wide header, or platform-specified crop; ask if unknown.
- Text ownership: main title in-image unless the OA template already owns the headline and the user wants a blank well.

### 抖音 / 视频封面 (Douyin / Video Thumb)

Use for 视频封面、短视频首帧、横/竖视频缩略图.

- Visual job: readable face/subject + short title at tiny preview size.
- Best form: one face or one result shot; title ≤ 10–12 字; high contrast block.
- Ratio: **9:16** vertical for short video; **16:9** for landscape video when specified.
- Text ownership: title in-image; do not rely on platform caption alone.

### 朋友圈分享图 (Moments Share)

Use for 朋友圈配图、分享卡片主图.

- Visual job: one clear beat that survives Moments compression and multi-image grids.
- Best form: simpler than XHS; fewer words; stronger single subject.
- Ratio: **1:1** or **3:4** depending on share layout.
- Text ownership: short title in-image if the share is title-led; otherwise subject-only with caption outside.

### 搜索结果缩略图 (Search-Result Thumb)

Use when the cover must win in search grids / 发现页 / 推荐 thrumbnails.

- Visual job: title still readable at ~120–200px width.
- Best form: fewer words, heavier type, solid title block, no busy texture under glyphs.
- Ratio: match the parent platform (usually XHS 3:4).
- Text ownership: title in-image; treat thumbnail readability as a hard gate.

### 卡片中心图 (Center Image For A Card)

Use when another system (quote-cards, social-card layout, slide, README card) will own headline, ratio, and caption.

- Visual job: be the image well only.
- Best form: **no large title inside**; leave safe margins; avoid dense edge type.
- Text ownership: outer layout owns title/subtitle; image may keep tiny object labels only if needed.
- When this is the real ask, prefer handing off to the card/layout owner rather than shipping a full Cover Pop title cover.

## Routing Questions

Answer these before Stop Test / prompt writing:

```text
asset role: xhs note cover / wechat OA header / douyin-video thumb / moments share / search-result thumb / center image for a card
platform:
ratio:
text ownership: title in-image (default) / outer layout / both
truth constraints: exact title text / exact numbers or claims in title / none
reroute?: yes/no → better owner
```

## Text Ownership (Cover Default)

For Cover Pop, **in-image title is the default**. A blank background for later overlay is allowed only when the user explicitly asks for editable / post-production text, or when the role is "center image for a card."

| Owns | What |
| --- | --- |
| Image (default) | main title ≤15 字, optional sub ≤10 字, any number/claim shown on the cover |
| Outer layout | note body, caption, hashtags, CTA copy, author bio, platform metadata |
| Refuse to invent | fake stats, fake "限时", fake social proof, unverified rankings |

## Truth Handling

### Must Be Exact

- the title string the user locked (or the title you proposed and they accepted)
- any number, percent, price, date, name, or ranking that appears on the cover
- product / book / place names when recognition matters
- before/after claims that the note actually delivers

Put exact requirements in the final prompt:

```text
Exact text: render EXACTLY these characters as the main title: "{title}".
Optional sub: "{sub}" or omit.
Do not invent extra numbers, badges, watermarks, or claims.
Do not alter, add, or drop characters.
```

### Can Be Symbolic

- mood lighting, texture, palette accent
- metaphor props that support the hook
- non-critical background objects
- archetype framing (contrast panels, list chips) as long as claims stay true

## What To Refuse Or Reroute

| Ask | Better owner |
| --- | --- |
| article / essay body illustration, concept figure, multi-beat explainer | **paper-operators** / **busy-town** / **lego-town** (by job) |
| quote save-card, 金句卡片, number poster for saving | **quote-cards** |
| sticker / emoji pack / expression set | **sticker-set** / gif-stickers |
| logo, icon system, brand mark | **refuse** — not a cover skill |
| dense infographic / full slide deck layout | PPT / chart / layout workflow |
| center illustration only, title owned by outer card | card/layout skill; Cover Pop only if they still need a cover-shaped well |

In these cases, say the better owner plainly. Do not "almost" make a cover that is really a body figure or a logo.

## QA Additions

Before delivery, check:

- The chosen asset role and platform ratio are visible in the result.
- Text ownership matches the role: title in-image for covers; no stuffed paragraphs.
- Exact title characters and any on-cover numbers/claims are not invented, misspelled, or swapped.
- The job is still "stop and tap" — not decoration, not a body explainer, not a logo.
- The cover remains readable at the intended thumbnail size.
