---
name: urlskill
description: Generate article SEO packaging fields after a draft or outline is ready, including URL slug, SEO keywords, SEO meta description, short summary under 20 Chinese characters, and summary under 100 Chinese characters. Use when the user asks for URL, SEO keywords, SEO description, meta description, article summaries, publishing metadata, or Chinese blog SEO packaging.
---

# URLskill

Use this skill to package a finished or near-finished article for publishing.

## Output Fields

Always provide these five fields unless the user asks otherwise:

1. URL
2. SEO keywords
3. SEO description
4. Short summary, within 20 Chinese characters
5. Summary, within 100 Chinese characters

When responding in Chinese, label the fields as:

1. URL
2. SEO关键词
3. SEO描述
4. 20字以内摘要
5. 100字以内摘要

## Workflow

1. Identify the article title, core keyword, target reader, and main business value.
2. Create a concise URL slug:
   - Use lowercase English words.
   - Prefer `/blog/<core-keyword-in-english>`.
   - Keep it readable and avoid dates, filler words, or unnecessary categories.
3. Generate SEO keywords:
   - Put the core keyword first.
   - Include close variants, Chinese terms, English equivalents, and high-value long-tail terms.
   - Separate SEO keywords with English commas `,` only. Do not use Chinese commas `，`, enumeration commas `、`, semicolons, or line breaks as separators.
   - Do not stuff irrelevant keywords.
4. Generate the SEO description:
   - Keep it within 88 Chinese characters unless the user sets another limit.
   - Put the core keyword near the front.
   - Make the value clear for the target reader.
   - Avoid bland summaries equivalent to "This article introduces...".
   - Show what problem the article helps solve or what decision it helps readers make.
5. Generate summaries:
   - The 20-character summary should be compact, clear, and usually action-oriented.
   - The 100-character summary should explain what the article covers and who it helps.

## Style Rules

- Prioritize click-worthy clarity over clever wording.
- For B2B or business articles, emphasize decision-making value, efficiency, risk reduction, customer acquisition, operations, or conversion when relevant.
- Keep SEO descriptions natural; do not overuse punctuation or stack keywords mechanically.
- If a suggested SEO description feels generic, rewrite it around the reader's decision or pain point.
- Do not invent unsupported product claims. If product benefits appear in the article, phrase them as concrete use cases.

## Example Pattern

For an article about "WhatsApp broadcast vs group":

- URL: `/blog/whatsapp-broadcast-vs-group`
- SEO keywords: include the core Chinese keyword first, then variants such as WhatsApp broadcast, WhatsApp group, WhatsApp mass messaging, WhatsApp Business API.
- SEO description: start with the core keyword, then state the decision value for merchants.
- 20-character summary: a short phrase that tells readers the article helps them choose.
- 100-character summary: summarize the comparison, limits, scenarios, and business decision value.
