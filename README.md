# Cover Pop

> A skill for high-conversion Chinese article covers, WeChat headers, thumbnails, and promo cards.

Cover Pop focuses on the first click: title architecture, cover archetypes, composition, and visual tension for Chinese social publishing. It helps create covers that are clear, shareable, and less generic.

## Examples

<p><img src="examples/images/cover-pop-open-source-skill.png" alt="Cover Pop open-source skill cover" width="100%"><br><sub>Cover Pop open-source skill cover</sub></p>
<p><img src="examples/images/paper-operators-wechat-cover.jpg" alt="Paper Operators WeChat cover" width="100%"><br><sub>Paper Operators WeChat cover</sub></p>

## What It Does

- Turn a topic into a strong cover headline and subline.
- Choose cover archetypes such as free-gift, contrarian, checklist, result promise, or field report.
- Generate WeChat/article/social cover prompts with readable native Chinese title text.
- QA the cover for contrast, cropping, title fit, and thumbnail survival.

## Install

Clone this repository into your local Codex skills folder:

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/Alexsun1one/cover-pop.git ~/.codex/skills/cover-pop
```

If your agent expects a nested skill directory instead of a direct clone, copy the folder that contains `SKILL.md` into its skills directory.

## Use

Example request:

```text
Use cover-pop to make a WeChat 900x383 cover. Topic: 免费送你一个开源 AI Skill. Make the headline large, native, and readable.
```

The skill entry point is [`SKILL.md`](SKILL.md). Supporting rules live in [`references/`](references/) when this repo includes them; helper scripts live in [`scripts/`](scripts/) when available.

## Quality Bar

- The image must explain a concrete idea, not merely decorate the page.
- Chinese text should be readable at the actual publishing size.
- The output should keep a stable style system across a set while letting each image fit its topic.
- Generated examples are prompts and visual references, not fixed templates.

## WeChat

More writeups, examples, and AI workflow notes are published on my WeChat official account. This is the real QR/search card used for the account, included as a normal bitmap asset rather than a stylized fake code.

<p align="center">
  <img src="assets/wechat-official-account.png" alt="微信搜一搜：正在逐渐AI化" width="720">
</p>

## License

MIT. See [`LICENSE`](LICENSE).

## Notice

This is an original open-source skill package by Sun Wuyuan / Alexsun1one. It is not affiliated with OpenAI, GitHub, WeChat, or any referenced platform. Avoid using it to imitate protected characters, living artists, or third-party brand assets without permission.
