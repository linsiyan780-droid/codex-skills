---
name: wechat-official-account-cover
description: Create polished WeChat official account top-article covers from article titles, outlines, or full drafts. Use when the user asks for a 微信公众号封面, 公众号头图, 微信头条封面, article cover, or wants an image-generation prompt/visual direction for a Chinese WeChat article cover, especially with requirements like light background, no text, article-related elements, minimal premium style, and 2D vector illustration.
---

# 微信公众号封面

## Overview

Turn a Chinese article draft into a clear cover-image direction for a WeChat official account top article. Prioritize a clean editorial banner that communicates the article topic through symbols and composition instead of text.

## Workflow

1. Read the title and article body carefully.
2. Identify the article's core contrast, question, or decision framework.
3. Extract 3-6 visual elements that can represent the topic without words.
4. Choose a light, refined visual system suitable for a WeChat top cover.
5. Generate the image directly with `imagegen` when the user asks for the cover image; otherwise provide a ready-to-use prompt.

## Visual Rules

- Use a wide horizontal composition suitable for a WeChat official account top image.
- Use a light background by default: off-white, pale gray, very light blue, pale mint, or soft neutral tones.
- Do not include text unless the user explicitly asks for visible copy.
- Do not include readable letters, numbers, UI copy, QR codes, watermarks, or brand wordmarks.
- Prefer 2D vector illustration, flat editorial style, crisp linework, restrained shadows, and simple geometric accents.
- Avoid overly 3D, photorealistic, cluttered, dark, loud, or cartoonish results.
- Make the image clearly related to the article by showing abstract but recognizable domain elements.
- For business or SaaS topics, aim for a premium, clean, organized, modern editorial look.

## Article-To-Image Mapping

When reading the article, translate ideas into simple visual metaphors:

- Comparison articles: split or balanced left-right composition, two workflows, two clusters, or two symbolic systems.
- Tool selection guides: central decision hub, branching paths, cards, toggles, or connected nodes.
- Messaging or customer communication: phone, chat bubbles, sender nodes, customer avatars, inbox, notification symbols, flow arrows.
- Automation or API topics: connected nodes, tags, gear, routing lines, shared inbox, simple workflow blocks.
- Marketing or business growth: customer segments, outreach paths, conversion funnel, CRM-like abstract panels.

Keep metaphors abstract enough to avoid relying on exact brand logos, but concrete enough that the article topic is obvious.

## Prompt Pattern

Use this structure for image generation:

```text
Use case: ads-marketing
Asset type: WeChat official account top article cover, wide horizontal banner, no text
Primary request: Create a polished 2D vector illustration cover for a Chinese article about <article topic>.
Scene/backdrop: clean light background, airy negative space, subtle geometric accents, premium editorial business-tech feeling.
Subject: <central visual metaphor from the article>. Include <3-6 article-related elements>. Use abstract icons and symbols only, with no readable words.
Style/medium: flat 2D vector illustration, minimalist, refined, modern editorial cover, crisp edges, gentle linework, slight soft shadows only, not 3D, not photorealistic.
Composition/framing: wide horizontal composition suitable for WeChat cover, balanced layout, clear focal point, enough breathing room.
Color palette: light background; restrained accent colors appropriate to the topic; avoid a one-note palette.
Text (verbatim): none.
Constraints: absolutely no text, no letters, no numbers, no logos or brand wordmarks, no QR codes, no watermark. Keep it simple, high-end, clean, and clearly related to the article.
Avoid: realistic 3D objects, busy UI, dark background, dominant gradients, cartoonish characters, excessive detail, clutter, readable UI text, brand logos.
```

## Example: WhatsApp Broadcast vs Group Article

For an article comparing WhatsApp broadcast, group chat, and Business API:

- Show a central smartphone with abstract chat bubbles.
- Show one-to-many private outreach on one side: a sender node pointing to separate customer avatar circles.
- Show many-to-many group interaction on the other side: avatar circles around shared chat bubbles.
- Add subtle business/API automation hints: connected nodes, tags, an inbox tray, a gear, or routing arrows.
- Use generic messaging symbols only; do not use the official WhatsApp logo or readable app UI.

Example prompt:

```text
Create a polished 2D vector illustration cover for a Chinese WeChat article comparing WhatsApp Broadcast vs WhatsApp Groups and explaining when merchants should choose Broadcast, Groups, or WhatsApp Business API. Use a clean light background with airy negative space and subtle geometric accents. In the center, place a simplified smartphone with abstract chat bubbles and no readable UI text. On the left, show one sender node sending private message bubbles to separate customer avatar circles, implying broadcast. On the right, show several avatar circles connected around shared chat bubbles, implying group discussion. Add subtle business automation elements near the bottom: connected nodes, tag shapes, an inbox tray, a gear, and simple flow arrows. Use a flat 2D vector style, minimalist premium business-tech editorial look, crisp edges, gentle linework, and very slight soft shadows. No text, no letters, no numbers, no logos, no QR codes, no watermark. Do not use the official WhatsApp logo; use generic messaging symbols only. Avoid 3D, photorealism, dark background, clutter, and readable UI text.
```
