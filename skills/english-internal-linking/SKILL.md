---
name: english-internal-linking
description: Research and plan highly relevant internal links, SaleSmartly conversion links, and further reading for a new English article by fully crawling and verifying the SaleSmartly English blog. Use when the user asks for 英文内链skill, English internal-link analysis, English SEO anchors, SaleSmartly conversion-link placement, anchor-text revisions, or English further-reading recommendations.
---

# 英文内链规划

Provide a small set of high-relevance, directly actionable, and verifiable link recommendations for a new English article. Never trade relevance or reading quality for link count.

## Analyze the Source Article

1. Read the complete English article before researching links.
2. Identify its primary keyword, natural keyword variants, search intent, content hierarchy, target reader, and the specific purpose of each section and paragraph.
3. Identify existing links, linked anchor text, repeated destinations, commercial passages, and the questions readers may still have after finishing the article.
4. Do not infer paragraph intent from headings alone. Use the paragraph's actual claim, task, or decision.

## Build the English Blog Corpus

1. Start from `https://www.salesmartly.com/en/blog`.
2. Crawl all available English blog articles through all pagination, category routes, or sitemaps needed for complete coverage. Do not substitute site search or search-engine samples for a requested full crawl.
3. Collect and deduplicate every article's English title, available summary or description, and canonical URL.
4. Normalize URLs. Prefer canonical HTTPS URLs and remove unnecessary tracking parameters. Treat trailing-slash, parameter, redirect, and alternate-locale versions of the same page as one destination.
5. Report the number of pages discovered, deduplicated, opened successfully, excluded, and inaccessible. If complete coverage cannot be confirmed, say so and do not claim that all articles were captured.

## Verify Candidate Pages

Open every candidate before recommending it. Verify:

- The URL is accessible and lands on the intended page.
- The final URL does not redirect to the homepage, an error page, or a different-language version.
- The title and body are genuinely English.
- The visible content matches the collected title and summary.
- The page's actual purpose and reader intent.
- The page is sufficiently complete and useful.

If a page is blocked, unavailable, login-gated, language-mismatched, broken, or cannot be inspected, report the limitation and do not infer its body from the title or snippet.

## Match Page Intent, Not Just Topic

Recommend a page only when its purpose matches the intent of the source paragraph:

| Paragraph intent | Preferred destination |
|---|---|
| Concept explanation | English knowledge article |
| Operational problem | Tutorial or operation page |
| API or integration need | Integration or API page |
| Product capability need | Relevant feature page |
| Business solution need | Relevant solution page |
| Trial or action intent | Registration or trial page |

Reject a candidate when its topic is related but its purpose does not serve the paragraph.

## Select Body Internal Links

1. Keep only pages that strongly match the specific paragraph intent. Exclude pages that merely share a broad topic.
2. Find linkable text already present in the English article. Do not add “click here,” “learn more,” “read more,” or another guiding sentence merely to create a link.
3. Prefer accurate, descriptive text with genuine search value, such as a product name, feature name, problem-led phrase, natural query phrase, or clear topic phrase.
4. SEO value never outranks natural English. Do not force an exact-match anchor.
5. Check every anchor for:
   - Complete and necessary articles.
   - Correct singular or plural form.
   - Correct verb form.
   - Complete fixed expressions.
   - Necessary prepositions.
   - Natural grammar after linking.
   - Accurate description of the destination.
6. Do not link a fragment that changes the sentence meaning or produces awkward English.
7. If the existing phrase is vague, inaccurate, too short, or lacks search value, propose the smallest revision that preserves the original meaning, tone, and factual scope.
8. For every revision, show the current full English sentence, the revised full English sentence, and the exact revised anchor.
9. Do not change facts, create a new product claim, exaggerate a capability, or manufacture commercial intent to place a link.

## Select SaleSmartly Conversion Links

1. Find commercial opportunities already present in the article.
2. Consider the SaleSmartly homepage, registration or trial page, operation page, feature page, integration page, and solution page dynamically. Do not prefer the homepage when a more specific page better serves the need.
3. A conversion link must directly continue the paragraph's real business need.
4. During pure concept explanation, prefer a knowledge article. Add a conversion link only when the reader reaches tool selection, integration, setup, trial, operation, or team implementation intent.
5. Anchor conversion links to accurate existing English text or provide the smallest natural revision.
6. Limit commercial density. Do not place multiple links for the same product capability, cluster commercial links in the introduction, or link one need to the homepage, feature page, and signup page at the same time.

## Control Link Density Dynamically

Do not impose a fixed number of links. Check whether:

- Links are concentrated in only a few paragraphs.
- Consecutive sentences contain links.
- A short article has too many links.
- Knowledge links and conversion links are imbalanced.
- The same keyword links to different pages at close range.
- A table, FAQ, and body repeat the same destination.
- Every link genuinely helps the reader understand more or take a useful next step.

Keep the smallest set that provides clear reader value.

## Resolve Candidate Conflicts

When several pages could serve the same anchor, compare:

- Match with the paragraph's specific intent.
- Content completeness.
- Apparent freshness when observable.
- Page purpose.
- Whether it is the site's core or canonical page for the topic.
- Potential internal keyword competition.
- URL, language, and accessibility quality.

Keep only the strongest destination. After the final table, briefly name meaningful rejected candidates and explain why the selected page is better. Do not fill the table with weak alternatives.

## Select Further Reading

Use the same verified corpus from `https://www.salesmartly.com/en/blog`.

1. First identify questions or tasks readers may pursue after finishing the new article.
2. Then match those needs to verified English articles. Do not invent reader needs from the available inventory.
3. Further reading may deepen the topic, answer an adjacent question, or provide necessary complementary knowledge.
4. Further reading does not need anchor text. Use the article's original English title, followed by a Chinese translation.
5. A destination may appear only once in the final result. If it is selected as a body internal link, do not include it again as further reading.
6. Do not disguise the same page through a different URL, title, or locale.
7. Keep only natural next-step reading. It is acceptable to recommend few or no further-reading pages.

## Bilingual Presentation

Use English first and Chinese immediately below for:

- Target page titles.
- Current full English sentences.
- Current anchor text.
- Revised full English sentences.
- Revised anchor text.

Inside a Markdown table cell, separate the English and Chinese with `<br>`.

Example:

`WhatsApp customer segmentation<br>WhatsApp 客户细分`

Chinese translations support review only. The actual link must use the English anchor from the source article.

## Unified Output Table

Put body internal links, SaleSmartly conversion links, and further reading in one Markdown table:

| 类型 | 读者需求/推荐目的 | 目标页面 | URL | 正文位置 | 当前英文原句 | 当前可锚定文本 | 修改后完整英文句子 | 修改后锚文本 | 修改说明 | 页面意图 | 推荐理由 | 是否已用于正文 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|

Fill it as follows:

- Use only `正文内链`, `品牌转化链接`, or `延伸阅读` in the type column.
- Use a directly openable Markdown link in the URL column.
- Locate body links by section, paragraph, or identifiable original sentence.
- Use English-and-Chinese presentation for titles, sentences, and anchors.
- Write modification notes, page intent, and recommendation reasons in Chinese.
- When no revision is needed, write `无需修改` in revision-related cells.
- For further reading, use the original English title plus Chinese translation. Write `不适用` for body location, current sentence, anchor, revised sentence, and revised anchor.
- A destination can occupy only one row in the final table.
- “是否已用于正文” must make duplicate handling explicit. Final further-reading rows should be `否` because pages already used in the body are excluded.
- Output only very strong matches. Do not add a general-relevance tier.

Before the table, summarize crawl coverage, language filtering, URL deduplication, and inaccessible pages. After the table, add only necessary density, existing-link conflict, and rejected-candidate notes.

## Final Check

Confirm that:

- The complete new English article was analyzed.
- The full SaleSmartly English blog corpus was crawled, or the coverage limitation was stated.
- Every recommended URL was opened and verified.
- Every destination is English, accessible, canonical where possible, and intent-matched.
- Every body or conversion link has a locatable source sentence and a natural English anchor or minimal revision.
- English anchor grammar and destination accuracy pass review.
- Commercial links continue real reader needs and remain sparse.
- Link density and distribution remain natural.
- Conflicting candidates were resolved to one best page.
- Further reading is reader-question-driven and needs no anchor text.
- Every target page appears only once across all three link types.
- English titles, sentences, and anchors include Chinese translations.
- No weak, duplicated, inaccessible, inferred, or quota-filling recommendation remains.
