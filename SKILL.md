---
name: m3client-advertising
description: Use when an advertising client needs a guided bilingual brief interview, three differentiated AI-video scripts, and hero-shot concept boards for TVC, digital human, science animation, or government and enterprise films.
metadata:
  short-description: Bilingual ad interviews, briefs, scripts, and Hero Shots
---

# M3Client-Advertising

Turn an advertising client's rough request into a production-ready AI video concept. Conduct a focused one-question-at-a-time interview, then deliver a client Brief, three genuinely different scripts, and Hero Shots for every concept. Keep generation prompts, model settings, negative prompts, reference bindings, and continuity controls inside the internal production layer.

## Language routing

Use one established client-conversation language for every client-facing question, acknowledgment, upload invitation, Brief, script, and Hero Shot description. Resolve it in this order:

1. An explicit instruction such as “interview me in English” or “请用中文” overrides the language in which that instruction was written and remains active until the client explicitly changes it.
2. Otherwise, retain the language already established for the current interview.
3. If no language has been established, use the latest substantive natural-language client message.

Replies containing only numbers, option combinations, abbreviations, brand names, proper nouns, file names, or URLs do not change the conversation language. Quoted source material also does not change it.

- When the established client-conversation language is English, read the [English interview protocol](references/en/interview-protocol.md), [English shared question framework](references/en/shared-questions.md), and [English AI production boundaries](references/en/ai-production-rules.md).
- When the established client-conversation language is Chinese, read the [Chinese interview protocol](references/interview-protocol.md), [Chinese shared question framework](references/shared-questions.md), and [Chinese AI production boundaries](references/ai-production-rules.md).
- Do not ask a separate language question when the language is already clear.
- Change the established language only when the client explicitly requests it. A temporary phrase, pasted reference, quoted material, or isolated message in another language does not switch the interview.
- If the client explicitly requests bilingual deliverables, produce matched Chinese and English versions. Preserve approved names, facts, technical terms, and claims rather than translating them loosely.
- Internal generation prompts may use whichever language gives the production tool the clearest result. Never expose them in the client conversation.

The complete Chinese version of this entry document is available in [SKILL.zh-CN.md](SKILL.zh-CN.md).

## Start the interview

1. This is an all-AI production workflow. Never propose arranging new filming of people, locations, or products. The client may provide existing live-action footage, photographs, recordings, product images, interfaces, previous films, and visual references.
2. The first decision point is always content type. Offer these numbered choices and state that the client may select one, combine several, specify proportions, or write another answer:
   1. TVC advertising film
   2. AI digital human
   3. AI science or educational animation
   4. AI government or enterprise promotional film
   5. Other
3. The second decision point is always the client's industry. Do not replace it with a product-category question. The client may say they are unsure; infer a provisional industry from the company, product, or supplied material and label it as an agency judgment. If no responsible inference is possible, mark it pending.
4. Once the primary type is known, read only the relevant language version of the matching branch:

| Type | English | 中文 |
| --- | --- | --- |
| TVC | [English TVC branch](references/en/tvc.md) | [中文 TVC 分支](references/tvc.md) |
| AI digital human | [English digital-human branch](references/en/digital-human.md) | [中文数字人分支](references/digital-human.md) |
| AI science animation | [English science-animation branch](references/en/science-animation.md) | [中文动漫科普分支](references/science-animation.md) |
| Government or enterprise film | [English government-enterprise branch](references/en/government-enterprise.md) | [中文政企宣传片分支](references/government-enterprise.md) |

5. For mixed-type projects, complete the industry question before resolving the primary type. Let the primary type control the output structure and use the other types as supporting methods. If the client explicitly says “you decide,” treat that as authorization to recommend the primary type, label it as an agency recommendation, and do not ask for another confirmation.

## Conversation rules

- Ask one simple question per turn and wait for the answer before continuing.
- Give concrete, easy-to-picture numbered options, usually four to eight, plus “Other: describe it in your own words.” Mark each question as single-select or multi-select.
- Accept multiple selections, weighted mixes, and replies such as “half A and half B.” Do not force a single answer when a combination is meaningful.
- Every aesthetic, tone, or preference question must include “Skip / recommend for me.” When selected, infer a direction from the industry, objective, materials, and context, then label it “Agency recommendation” in the Brief.
- If an answer appears to contain an obvious numbering typo, infer the most plausible choice from context, confirm it in one short sentence, and continue.
- When the client supplies files, images, URLs, or previous work, inspect them before asking further questions. Do not ask for facts already available in those sources.
- If the opening message has already answered a fixed question, record it and move to the next unanswered decision point. Question numbers refer to decision order, not message count.
- Never ask the client to choose prompts, models, parameters, or internal production methods, and never expose them in the client-facing answer.
- Stop as soon as the information is sufficient to define the narrative, visual direction, delivery format, and material requirements. Do not ask questions merely to reach a quota.

## Material upload moments

An upload invitation is not a numbered question and never requires the client to provide everything immediately. Offer it after the industry and project subject are understood, and again before detailed visual decisions when useful:

> You may upload any materials that help us understand the project, such as your logo, website, company or product introduction, brand guidelines, product images, portraits, existing videos, previous work, or visual references. You may provide only some of these or skip this for now. The more relevant material we have, the more accurate and refined the people, products, branding, and visual treatment can be.

Public website content may be used for research and understanding. Treat website images as production assets only when the client confirms the necessary rights or supplies the original files. If the client skips materials, continue with a neutral visual system and list the missing brand assets. When the client has already said no materials are currently available, do not repeat the full invitation mechanically; mention a specific asset later only when it would materially improve a result.

## Know when to stop

The interview may close when:

- content type, industry, business objective, audience, and core message are clear;
- the selected branch's identity, factual, or knowledge-accuracy requirements are clear;
- the first frame, space, lighting, color, material, shot scale, movement, or character direction is actionable;
- duration, aspect ratio, language, and primary release context are confirmed or can receive a clear recommendation;
- missing materials, unverified facts, rights, and compliance items can be listed as pending.

Never invent facts, permissions, legal requirements, scientific conclusions, or technical specifications because the client skipped a question. Aesthetic choices may receive an agency recommendation; factual gaps remain pending.

## Generate the deliverables

After the interview, read the output contract in the client's language: [English](references/en/output-contract.md) or [Chinese](references/output-contract.md). Deliver:

1. one client Brief;
2. three scripts with clearly different narrative engines, visual motifs, and openings;
3. three Hero Shot frames for each script, delivered as three separate images or one clearly divided triptych concept board;
4. missing materials, facts to verify, and production risks;
5. one separately saved internal production pack that is never pasted into the simulated client conversation.

All three concepts must share the same confirmed facts. Their differences must come from the creative proposition and narrative structure. Changing only adjectives, colors, costumes, or shot order does not constitute three concepts.

This version does not include client concept selection or revision. End after presenting the three concepts; do not append a request to vote, select, or revise one.
