---
name: first-version-article-outline
description: Create a Chinese-first blog article outline using mandatory live Google SERP research in Chrome with the installed Search Simulator extension, a dynamically structured reader-task path, a required search-backed non-duplicative FAQ, and mandatory context-adapted product or brand integration. Use when the user asks to make, summarize, reuse, or modify an article outline process; create SEO blog outlines; analyze search intent, top-ranking articles, FAQ/long-tail questions, or product insertion points; or invoke “第一版文章大纲skill”, “文章大纲skill”, or “first-version-article-outline”.
---

# 第一版文章大纲 Skill

## Overview

Use this skill to turn a keyword or topic into a blog outline that first satisfies reader search intent, then integrates the required product or brand messaging in a context-appropriate way. Always complete the mandatory live SERP research before analyzing search intent or creating any outline, even when the user provides existing research or asks for a one-shot result. Every outline must include a non-duplicative FAQ built from search-backed long-tail questions and a product or brand integration whose role, placement, depth, frequency, wording, and conversion intensity adapt to the article. Default to a step-by-step confirmation workflow: output one major stage, stop for user review, and continue only after the user confirms or revises it.

## Operating Mode

- Default to staged confirmation. Do not output the full outline in one pass unless the user explicitly asks for a one-shot result.
- After each checkpoint, ask whether the user wants to confirm, revise, or continue.
- If the user modifies a previous step, update that step and use the revised version as the basis for later steps.
- Keep the article reader-first. Do not add product promotion that interrupts the main search intent.
- Always integrate the designated product or brand, but dynamically adapt its role, placement, depth, frequency, wording, and conversion intensity to the article topic and reader journey.
- Always include an FAQ made of search-backed long-tail questions that are relevant to the topic, useful to the reader, unsuitable for full treatment in the main body, and not already answered there.
- Write in Chinese by default. Preserve English terms when they are keywords, product names, SERP titles, or common industry terms.
- Treat live SERP research as a mandatory prerequisite every time this skill is used. Never skip it, including when the user provides existing materials or asks for an outline based only on the current context.
- Use the Search Simulator extension already installed in Google Chrome to run the exact target keyword on Google and inspect the rendered results. This is required to reduce the influence of personalized search results as much as possible.
- Gather the first 10 visible organic results in their displayed order before proceeding to search-intent analysis, title design, or outline creation.
- Do not substitute a generic web-search tool, another search engine, direct Google browsing without Search Simulator, or an inferred ranking list for this workflow.
- Preserve Google's visible organic-result order and exclude ads, sponsored placements, AI Overviews, featured snippets, map packs, video packs, and other non-organic modules unless the user explicitly asks to analyze them.
- Record the query, Google locale/domain, simulated location, language, search date, visible region, whether Chrome is signed in when observable, and evidence that Search Simulator was used. Explain that geography, language, and other factors may still change the result order.
- Tell the user whenever a Top 10 result page cannot be opened or its body cannot be inspected. Never hide, silently skip, replace, or infer inaccessible content.
- If Chrome, the Search Simulator extension, or Google Search cannot be accessed, stop the workflow and ask the user to restore access or provide a Google results screenshot/export produced through this search process. Do not continue to later steps until valid SERP evidence is available.

## Workflow

### Step 1: Confirm the Input and Research Scope

Identify:

- Target keyword or article topic.
- Target reader and business context, if provided.
- Target market/language, if provided.
- The product, brand, and URL that must be integrated. If this information is missing, obtain it before finalizing the outline.

Always complete the following mandatory SERP research before proceeding:

- In Google Chrome, use the installed Search Simulator extension to search the exact target keyword on Google for the target market/location. Verify that the rendered results came from Search Simulator, then gather the first 10 visible organic results in their displayed order. Use additional query variants only after analyzing the exact keyword, and label each query separately.
- Open and inspect each Top 10 result when accessible. For every result, record its organic rank, page title, URL, site or brand, content type, title promise, main H2s, primary intent, content depth, distinctive information, apparent gaps, FAQ or long-tail questions, and whether the page body opened successfully.
- If a Top 10 page is blocked by a login wall, paywall, geographic restriction, robots restriction, broken page, or another access barrier, tell the user which ranked result is affected and why when observable. Preserve its original Google rank and record only information actually visible on the search results page or accessible page surface. Do not infer its H2s, depth, FAQ, or body content.
- Do not replace an inaccessible Top 10 result with result 11 or later. You may inspect later organic results as supplemental references, but label them clearly as supplemental and never mix them into the ranked Top 10 dataset.
- Report the research completeness, including how many of the Top 10 bodies were successfully inspected and which were inaccessible. If access failures materially weaken the comparison, state that limitation explicitly before drawing cross-result conclusions.
- High-value pages within roughly the top 20 when relevant: official docs, help centers, policies, product documentation, research reports, industry data, papers, standards, or authoritative references.
- Google “People also ask”, related searches, and autocomplete suggestions when available and high value.
- Synthesize cross-result patterns: dominant content formats, recurring H2 themes, repeated questions, common omissions, useful differentiation opportunities, and structures that should not be copied.

Do not call generic web search results "Google rankings." Do not use ordinary web search, another search engine, or direct Google results without Search Simulator as a fallback. If Chrome, Search Simulator, or Google Search cannot be accessed, pause the entire workflow, state the limitation, and ask the user to restore access or provide a Google results export/screenshot produced through the required search process. Do not analyze search intent or generate any title or outline until this requirement is satisfied.

Checkpoint output:

```text
Step 1 研究范围确认
- 目标关键词/主题：
- 目标读者：
- 业务背景：
- 目标市场：
- 目标语言：
- 搜索意图初判：
- 必须植入的产品/品牌/URL：
- 实际搜索查询：
- Google 域名/地区版本：
- Search Simulator 模拟地区/语言：
- 搜索日期：
- 搜索结果页可见地区：
- Chrome 登录状态（如可观察）：
- Search Simulator 使用证据：
- Google 前 10 个自然结果是否已采集：

Top 10 逐条记录：
- 自然排名：
- 页面标题：
- URL：
- 网站/品牌：
- 内容类型：
- 标题承诺：
- 主要 H2：
- 主要搜索意图：
- 内容深度：
- 特色信息：
- 明显缺口：
- FAQ/长尾问题：
- 是否成功打开正文：
- 无法访问的原因（如适用）：

横向结论：
- Top 10 的主流内容形式：
- 高频 H2 主题：
- 重复出现的问题：
- 普遍遗漏的内容：
- 可利用的差异点：
- 不值得跟随的结构：
- 正文成功访问数量：
- 无法访问的结果及原因：
- 研究完整度与限制：

请确认、修改，或告诉我继续进入 Step 2。
```

### Step 2: Summarize Search Intent and Reader Needs

Summarize what the reader wants to solve in order:

- Immediate answer they expect in the first screen.
- Information they must understand before completing the primary task.
- Steps, evidence, or evaluation criteria needed to complete that task.
- Limitations, risks, misconceptions, or obstacles that may prevent successful completion.
- Follow-up questions likely to remain after the primary task is completed.
- Needs that belong in the main body versus search-backed long-tail needs better reserved as preliminary FAQ candidates.

Checkpoint output:

```text
Step 2 搜索意图和读者需求
- 核心搜索意图：
- 读者最想快速得到的答案：
- 完成主要任务前必须理解的信息：
- 完成任务所需的步骤、证据或判断依据：
- 可能阻碍任务完成的限制、风险和误区：
- 文章必须覆盖的问题：
- 适合作为 FAQ 候选的长尾问题：
- 不建议写/不应展开的问题：

请确认、修改，或告诉我继续进入 Step 3。
```

### Step 3: Decide the Article Positioning and Title Direction

Decide the title direction dynamically from the primary search intent, the title and content-format patterns visible across the first 10 organic results, the target reader, and the article's actual scope. Do not default to including difference/comparison, use cases, limits, selection advice, FAQ, “complete guide”, or similar elements. Include an element only when it represents a major reader need and the article will answer it fully.

Use this process:

1. Identify the dominant search intent and expected content format. Distinguish among definition/explanation, tutorial, troubleshooting, comparison, selection/decision, recommendation list, review, trend/data analysis, case study, and resource/template intent. Treat these as categories for diagnosis, not title templates.
2. Analyze the first 10 organic results for the dominant title format, repeated promises and modifiers, keyword placement, content type, and unaddressed angles. Follow the result set's format expectations when they reflect reader intent, but do not copy competitor wording mechanically.
3. Define the article's actual coverage before writing the title. Use the SERP evidence and confirmed reader needs to decide the central question, scope, and one most valuable reading outcome.
4. Write a title that naturally includes the target keyword when feasible and emphasizes the primary reading outcome. Do not list every planned section or combine multiple secondary angles merely to make the title appear comprehensive.
5. Use a differentiating angle only when it is supported by a meaningful SERP content gap, a clearer audience or scenario, stronger evidence, or a more precise scope.
6. Verify every title promise against the planned article. Do not use “difference” without a substantive comparison, “how to choose” without decision criteria, “complete guide” for narrow coverage, “review/tested” without real testing or evidence, or “latest” without verifying current information. Do not mention FAQ in the title merely because the article contains an FAQ section.

Treat any example title as inspiration only. Never apply a fixed formula across unrelated topics.

Checkpoint output:

```text
Step 3 文章定位和标题方向
- 文章定位：
- 主要搜索意图：
- SERP 主流内容形式：
- SERP 标题共同模式：
- 可利用的标题差异点：
- 文章实际覆盖范围：
- 推荐标题：
- 备选标题：
- 推荐理由：
- 标题承诺是否都能由正文兑现：

请确认、修改，或告诉我继续进入 Step 4。
```

### Step 4: Build the H2 Outline Around the Reader Journey

Build the outline from search-intent clusters, the user's question chain, the primary reader task, and the semantic structure visible across the Search Simulator Google results. Do not assume every article follows a comparison or purchase-decision journey, and do not organize H2s as a flat inventory of everything that could be discussed.

Use this process:

1. Cluster the researched queries, recurring competitor sections, related searches, and reader questions by shared intent.
2. Identify the primary task the article must help the reader complete, such as understanding a concept, performing a task, solving a problem, comparing options, making a choice, finding resources, evaluating a product, interpreting a trend, or learning from a case. Treat these as diagnostic categories, not fixed outline templates.
3. Derive the answer path for this specific topic from the dominant search intent, the first 10 organic results, People Also Ask, related searches, the target reader, and the article's promised scope. Do not mechanically assign a standard path merely because the article belongs to a familiar category.
4. Run a Top 10 common-content coverage check. Identify the important questions, concepts, steps, criteria, or cautions repeatedly covered by strong results, then ensure the outline includes those that are necessary for the confirmed search intent. Do not copy competitor headings or reproduce a competitor's structure mechanically, and do not include repeated content merely because it is common.
5. Order H2s so the reader can complete the primary task in a continuous and natural sequence.
6. Assign one core question cluster to each H2. Every H2 must make a necessary contribution to completing the primary reader task.
7. Merge H2s when their search intent, expected answer, or subject substantially overlaps.
8. Demote secondary factors and narrow adjacent intents to an H3, paragraph, table field, callout, or FAQ when they do not justify an independent H2.
9. Decide the level of price, company size, deployment, geography, use case, risk, limitation, setup, and other factors from the actual search evidence. Do not preassign any factor to H2 or comparison-field status. Give it an H2 only when it represents an independent, important intent and requires substantial treatment.
10. Plan at least one and no more than three genuinely useful tables for every article. Use a table only when it makes comparisons, steps, criteria, evidence, risks, options, or other structured information easier to scan than prose. For each table, specify its location, purpose, and intended rows or columns. Do not repeat the same information at length in both the table and nearby prose.
11. Use bullet blocks only when the content benefits from scanning, such as findings, methods, evidence, checks, conditions, risks, or comparison criteria. Do not add bullets to every H2, do not split coherent reasoning mechanically, and do not repeat surrounding prose merely to create a list.
12. Select the closing function from what the reader most needs after the main body, such as a conclusion, action recommendation, selection guidance, verification method, risk reminder, escalation condition, observation criteria, reusable lesson, next resource, or product next step. These are options, not templates; combine them or choose another form when the topic requires it.
13. Reserve a mandatory FAQ module after the preliminary main-body close and build a search-backed candidate pool from People Also Ask, related searches, competitor omissions, SERP patterns, or clear reader follow-up needs.
14. At this stage, label candidates and their evidence without treating them as final. Flag likely overlap with the preliminary body for Step 6 review. Step 6 owns the final semantic de-duplication, replacement, product-integration reconciliation, and FAQ approval.

Before presenting the outline, run an H2 compression check:

- Can any two H2s be mistaken for covering the same content?
- Can any H2 be removed without preventing the reader from completing the primary task?
- Should any H2 become an H3, paragraph, table field, callout, or FAQ?
- Does the sequence read as a question-and-answer flow rather than a topic list?
- Does every H2 directly support the primary keyword's search intent?
- Does the outline cover the necessary common content found across the Top 10 without copying competitor wording or structure?
- Does the article plan contain one to three tables, and does every planned table improve understanding rather than repeat nearby prose?
- Is every bullet block justified by scannable content rather than added mechanically?
- Does the closing form match this topic instead of a generic article-type template?
- Does every preliminary FAQ candidate have a traceable search or reader-needs basis?
- Are likely overlaps with the preliminary body flagged for Step 6 instead of being presented as final?

Revise until these checks pass. Prefer the fewest H2s that fully satisfy the primary intent; do not add sections merely for comprehensiveness.

For each H2, include a short parenthetical note describing what the section should cover.

Checkpoint output:

```text
Step 4 初版文章大纲
- 文章需要帮助读者完成的主要任务：
- 大纲采用的回答逻辑：
- 结构依据：
- Top 10 必要共性内容覆盖：
- 未纳入的 Top 10 共性内容及原因：
- 表格规划（1–3 个，注明位置、目的和内容结构）：
- Bullet block 规划（如有，注明位置和作用）：
- 主体收尾方式及选择原因：
- FAQ 候选问题及来源：
- 与初版正文可能重叠的问题：

# 文章标题

## H2
（本节回答的核心问题及其在全文中的作用）

## H2
（本节回答的核心问题及其在全文中的作用）

## FAQ
（列出有搜索依据的候选问题及来源；Step 6 再完成最终去重、补位和定稿）

请确认、修改，或告诉我继续进入 Step 5。
```

### Step 5: Integrate Product or Brand Messaging Naturally

Integrate the designated product or brand in every outline. Do not decide whether to include it; decide how it should function and how strongly it should appear without disrupting the main search intent.

Use this process:

1. Define the product's role for this article: core solution, comparison subject, task-enabling tool, scenario-specific option, advanced alternative, implementation example, supporting resource, or next step. Treat these as candidate roles, not fixed placements.
2. Identify the exact reader problem the product solves and the first point in the reader journey where that need naturally appears.
3. Choose the placement dynamically. It may appear in the introduction, quick answer, relevant H2 paragraph, procedure, comparison table, scenario section, case, limitation-to-solution transition, closing, FAQ, or a standalone H2. Use a standalone H2 when the product itself is part of the primary search intent or needs substantial explanation; do not reject or prefer it by default.
4. Scale depth and frequency to relevance. Give a highly relevant product enough space to explain its function, fit, evidence, and limitations. For a weaker connection, use a concise but useful example, supporting option, or next step. Always include it, but never give it more prominence than its reader value supports.
5. Adapt wording and conversion intensity to intent. Use objective explanation or examples for information-led queries, clearer fit and selection guidance for comparison or decision queries, and stronger but accurate action guidance for product-led queries.
6. Make every mention informative by answering at least one concrete question: what it solves, who or which scenario it fits, why it belongs here, what it adds beyond basic methods, what constraints apply, or what the reader can do next.
7. Avoid repeated selling points, unsupported claims, artificial pain points, excessive brand repetition, abrupt sales copy, or turning an informational article into a landing page.
8. Explain why the selected role, placement, depth, frequency, wording, and conversion intensity fit the search intent and preserve the reader's answer path.

Checkpoint output:

```text
Step 5 产品或品牌植入方案
- 产品与主搜索意图的关系：
- 产品在文章中的角色：
- 产品解决的具体读者问题：
- 首次自然出现的位置：
- 其他必要出现位置：
- 是否需要独立 H2：
- 建议篇幅：
- 建议出现次数：
- 表述方式：
- 转化强度：
- 与前后内容的衔接方式：
- 如何避免破坏主要搜索意图：
- 需要避免的重复或宣传性表达：

请确认、修改，或告诉我继续进入 Step 6。
```

### Step 6: Finalize the Main-Body Close and FAQ

Finalize the main-body close and mandatory FAQ after combining the Step 4 outline with the Step 5 product-integration plan. Treat Step 4 as the preliminary structural design and use this step for final consistency, de-duplication, replacement, and placement decisions.

Use this process:

1. Confirm what the reader most needs after completing the article's primary task, then finalize a clear main-body close before the FAQ. The close may consolidate conclusions, recommend an action, support a choice, verify an outcome, clarify risk, define escalation or follow-up, extract a reusable lesson, or serve another topic-specific function. Treat these as candidate functions, not templates tied mechanically to article categories.
2. Ensure the close follows naturally from the body and adds synthesis, direction, validation, or a useful next step instead of merely repeating previous H2 content.
3. Reconcile the close with the confirmed Step 5 product plan. If the product appears there, make its role, wording, depth, and conversion intensity consistent with Step 5 and relevant to what the reader should do next.
4. Re-evaluate every preliminary FAQ candidate from Step 4 against the final H2s, H3s, tables, callouts, product integrations, and main-body close.
5. Keep an FAQ question only when it is directly relevant, has clear search or reader value, is supported by People Also Ask, related searches, SERP patterns, competitor omissions, or a clear follow-up need, is unsuitable for full expansion in the main body, and can be answered independently and concisely.
6. Detect semantic duplication, not just matching wording. Remove a candidate when its answer is already covered substantially anywhere in the final article plan.
7. Because the FAQ is mandatory, replace every removed duplicate or weak candidate with another qualified search-backed question. Continue researching or filtering until the final FAQ contains only relevant, useful, non-duplicative questions.
8. Use practical problems, limitations, pricing or fees, safety, compatibility, APIs, software or tools, missing features, account rules, and adjacent concepts only as research directions. Include one only when the evidence supports its relevance to the current topic; never fill a category mechanically.
9. Mention the product in an FAQ only when that FAQ has genuine tool, product, or solution intent and the product directly answers it. Follow the Step 5 role and conversion intensity; do not invent a question for exposure or repeat a selling point already covered elsewhere.
10. Place the finalized FAQ after the main-body close and verify that it does not stuff keywords, force product promotion, or duplicate itself.
11. Run a whole-article semantic duplication check across the introduction or quick answer, all H2s and H3s, tables, bullet blocks, callouts, product integrations, main-body close, and FAQ. Compare the expected answers and takeaways, not just heading wording. Merge, demote, relocate, or remove repeated material while preserving the reader's complete answer path.
12. Allow brief recaps only when they serve navigation, synthesis, or action. Mark them explicitly as concise recaps and do not repeat the same explanation, evidence, examples, product claims, or recommendations at length.

Checkpoint output:

```text
Step 6 主体收束与 FAQ 定稿

主体收束：
- 收束模块需要帮助读者完成什么：
- 采用的收束方式：
- 为什么适合当前主题和搜索意图：
- 是否只是重复正文：
- 产品是否在收束中出现：
- 与 Step 5 产品植入方案是否一致：

全篇内容去重：
- 检查范围（导语/H2/H3/表格/Bullet/提示框/产品植入/主体收束/FAQ）：
- 发现的语义重复：
- 合并、降级、移动或删除的内容：
- 保留简短回顾的位置及必要性：
- 去重后是否仍完整满足主要搜索意图：

FAQ：
- FAQ 候选问题及其来源：
- 每个问题对应的搜索或读者价值：
- 为什么不适合在正文中展开：
- 是否与最终正文、主体收束或其他 FAQ 重复：
- 删除或替换了哪些重复、薄弱问题：
- 产品是否需要在某个 FAQ 中出现及原因：
- 是否存在关键词堆砌或强行推广：
- 最终保留的 FAQ：

请确认、修改，或告诉我继续输出最终版大纲。
```

### Step 7: Output the Final Outline

Final output format:

```text
# 文章标题

## H2
（本节回答的问题、主要内容和必要写作提示）
（产品植入：如有，注明产品角色、位置和表达方式）

## 主体收束
（收束目的、主要结论和产品是否出现）

## FAQ

### 问题
（问题来源和回答方向）
```

If the user asks for only title and H2 outline, do not add ordinary H3s, full paragraphs, or a general source list. Keep each H2 note concise, but still mark the confirmed product integration briefly wherever it occurs and retain the mandatory FAQ with its finalized questions. If the user asks for a more detailed version, add H3s and bullet-level writing notes.
Always retain the topic-specific main-body close, qualified FAQ, and confirmed product or brand integration in the final outline, regardless of the requested level of detail.

Before delivering the final outline, verify that it covers the necessary Top 10 common content, contains one to three genuinely useful tables, uses bullet blocks only where the content benefits from scanning, and has no substantial semantic duplication across the entire article plan.
