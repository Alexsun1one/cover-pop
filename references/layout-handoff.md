# Layout Handoff / 版式交接

Use this reference when planning platform ratio, crop safety, and what stays outside the cover.

Cover Pop creates the **cover image**. The platform may still crop for feed, search, share, or header slots. Plan for the crop, not only the full canvas.

## Handoff Fields

Return these fields when planning a generated cover:

```text
final container: xhs note / wechat OA / douyin-video / moments / search thumb / card well / other
asset role:
recommended ratio:
safe margin:
title inside image: yes (default) / no
caption outside image:
crop guidance:
background requirement:
handoff owner:
```

## Platform Ratios

| Platform / role | Default ratio | Notes |
| --- | --- | --- |
| 小红书笔记封面 | **3:4** vertical | skill default |
| 搜索结果缩略图 | match parent (usually 3:4) | title must survive ~120–200px width |
| 公众号头图 / 推送封面 | **2.35:1** or platform spec | ask if unknown; keep title out of extreme edges |
| 抖音 / 竖短视频封面 | **9:16** | face/subject + short title |
| 横视频封面 | **16:9** | title in safe center band |
| 朋友圈分享 | **1:1** or **3:4** | simpler; fewer words |
| 卡片中心图 | ask outer layout | often 16:9 or card well; **no large title** |

If the user does not name a platform, default to **小红书 3:4**.

## Safe Margins & Crop

- Keep the **title and focal subject** in the central ~70% — never flush to the extreme edge.
- Assume feed / grid / Moments may crop 5–10% from edges; do not put critical glyphs in corners.
- For OA wide headers, keep the title in a stable band that survives common center crops.
- For video thumbs, assume heavy compression — prefer solid title blocks over type on busy texture.
- Dense collages: regenerate simpler rather than asking the platform crop to "fix it."

## Caption Outside

Anything that is not the cover's one-second pitch stays outside:

- note body / article paragraphs
- hashtags
- "点击看全文" / CTA
- source citations
- long disclaimers

If a generated cover already contains a paragraph or hashtag pile, regenerate with title-only (plus optional sub) instead of relying on layout cropping.

## Handoff Notes

In final delivery, include:

- full image path
- platform & aspect ratio used
- exact title text rendered
- recommended caption outside the image (if any)
- crop warnings (edge pressure, OA wide crop, video compression)
- whether the cover is safe for small / search thumbnail display

## Anti-Patterns

- shipping 16:9 when the ask was 小红书封面
- title flush to the top edge that dies in grid crop
- putting the only promise in an outside caption while the image is mute
- delivering a center-well image stuffed with a full cover title when the card layout already owns the headline
