# Failure Patterns / 失败模式库

Use this reference during QA and critique. A pretty cover can still fail. If one of these failures is present, do not describe the cover as "mostly fine." Name the failure and either regenerate or reroute.

## Common Failures

### Clickbait Empty Promise

Symptom: the title opens a gap ("你绝对想不到…") but the note has nothing concrete behind the tap; or the Forward Test blank is empty/generic.

Fix: reject. Rewrite title to a real payoff the content delivers, or refuse to generate until the promise is real.

### 微商风

Symptom: gold-on-red, glow bursts, sticker pile, fake "限时/爆款/马上抢" badges, QR cram, WordArt urgency.

Fix: regenerate clean — one base, one accent, one ink; solid title block; no fake urgency chrome.

### AI Plastic

Symptom: waxy skin, melted/gibberish glyphs, extra fingers, hallucinated logos, generic stock-photo-plus-bar look.

Fix: regenerate with harder negatives and quieter materials; repair title with exact-text block; never ship melted Chinese.

### Unreadable Thumb Title

Symptom: full-size looks fine, but at ~200px the main line cannot be transcribed character-by-character; type sits on busy texture; too many characters.

Fix: shorten (≤ 10–12 字), increase weight/contrast, move onto a solid plaque; re-run the real thumbnail squint test.

### Clutter

Symptom: collage of everything — three archetypes stacked, emoji rain, multiple focal subjects, title + paragraph + badges.

Fix: one promise, one focal subject, title budget only; cut the rest.

### Wrong Platform Ratio

Symptom: 16:9 delivered for 小红书; 3:4 delivered for OA wide header; video thumb letterboxed oddly.

Fix: regenerate at the platform ratio from `layout-handoff.md`; do not "stretch later."

### Wrong Owner

Symptom: Cover Pop is used for article body explainers, quote save-cards, stickers, logos, or dense infographics.

Fix: reroute — **paper-operators / busy-town / lego-town** for body figures; **quote-cards** for save-cards; **sticker-set** for stickers; **refuse** logos.

### Truth Drift

Symptom: title numbers, rankings, prices, or names were invented or altered from the locked string.

Fix: reject. Exact-text + exact-claim block; regenerate; do not "polish" locked copy.

### Center-Image Title Stuffing

Symptom: role is center illustration for a card, but the image still carries a full cover headline the outer layout will duplicate.

Fix: regenerate without large title; leave safe margins; let the card own the headline.

### Aesthetic Drift To Tacky

Symptom: 土味 bevel, neon-on-neon, PPT title-slide, rainbow gradient, plastic glow — even if the promise is real.

Fix: re-route aesthetic with `style-routing.md` / `style-dna.md`; one restraint; regenerate.

## QA Rule

Name the failure. Then either:

1. **Repair** (one wrong glyph, slight contrast bump) with a targeted re-render, or
2. **Regenerate** (empty promise, 微商风, unreadable thumb, wrong ratio, AI plastic), or
3. **Reroute** (wrong owner).

Do not ship a cover that would train the algorithm against the account.
