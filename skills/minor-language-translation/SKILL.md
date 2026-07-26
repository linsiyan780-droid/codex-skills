---
name: minor-language-translation
description: Translate English words, phrases, titles, SEO keywords, product feature names, or short text into six fixed languages: Portuguese (PT), Thai (TH), Korean (KO), Malay (MS), Arabic (AR), and Spanish (ES). Use when the user asks for “小语种翻译skill”, minor-language translation, multilingual keyword translation, or asks to translate English into the six language tags shown as PT, TH, KO, MS, AR, and ES.
---

# 小语种翻译skill

## Overview

Use this skill when the user gives English text and wants it translated into six fixed languages: Portuguese, Thai, Korean, Malay, Arabic, and Spanish. Keep output concise and practical for blog titles, SEO keywords, product functions, navigation labels, and marketing terms.

## Languages

Always output these six language tags in this order:

- PT: Portuguese
- TH: Thai
- KO: Korean
- MS: Malay
- AR: Arabic
- ES: Spanish

## Translation Rules

- Preserve brand names, product names, app names, and platform names unless the official local name is known.
- For SEO keywords or article titles, prefer natural local search wording over stiff literal translation.
- For product features, prefer terminology users would recognize in that language.
- Keep translations short when the source is a keyword or UI label.
- If a term has two common translations, provide the primary translation first and add a short note only when useful.
- Do not add unrelated explanation unless the user asks.
- If the English source is ambiguous, translate the most likely marketing/SEO meaning and mention the ambiguity briefly.

## Output Format

Use this format by default:

```text
英文原文：<source>

PT：<Portuguese>
TH：<Thai>
KO：<Korean>
MS：<Malay>
AR：<Arabic>
ES：<Spanish>
```

If the user provides multiple English terms, output one block per term.

## Examples

Input:

```text
WhatsApp broadcast
```

Output:

```text
英文原文：WhatsApp broadcast

PT：Transmissão do WhatsApp
TH：การบรอดแคสต์ WhatsApp
KO：WhatsApp 브로드캐스트
MS：Siaran WhatsApp
AR：بث واتساب
ES：Difusión de WhatsApp
```

For Spanish WhatsApp feature wording, `Lista de difusión de WhatsApp` can be suggested when the context specifically means WhatsApp’s broadcast list feature.

## Quality Check

- Check that all six language tags are present.
- Check that right-to-left Arabic text is not reversed.
- Check that app or brand names like WhatsApp remain recognizable.
- Check that the output stays in the requested fixed order.
