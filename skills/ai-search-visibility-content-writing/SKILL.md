---
name: ai-search-visibility-content-writing
version: 0.2.0
description: Use when writing or rewriting articles, landing pages, or knowledge content that should perform well in both classic search and AI-powered search experiences, especially when the task needs answer-first structure, clear entities, non-commodity information gain, human-readable narrative, and content that is easy for AI systems to extract and cite.
triggers:
  - "ai search visibility content writing"
  - "write this for ai search"
  - "make this article ai-search ready"
  - "rewrite for seo and geo"
  - "answer-first article"
  - "make this page citeable"
mutating: false
---

# ai-search-visibility-content-writing

Write content for unified search visibility, not for SEO theater.

This skill is for the writing layer of the `OpenClaw AI SEO and GEO Workflow`.
It turns an approved brief into content that works for:

- classic search discovery
- human readers who want a fast, useful answer
- AI search systems that need clear, grounded, extractable information

This skill does **not** own topic discovery, information-gain approval,
publishing, or live QA. It assumes the topic already passed upstream
qualification.

## When to use

Invoke this skill when the task is to write, rewrite, or substantially improve:

- blog posts
- landing pages
- product explainers
- operational guides
- comparison pages
- FAQ-heavy pages

Use it when the content should satisfy both classic SEO expectations and AI
search visibility expectations.

Do **not** use it for:

- keyword discovery
- topic qualification
- technical SEO audits
- schema-only tasks
- publish or deployment work

## Required inputs

Before writing, confirm the brief includes:

- `target_reader`
- `core_query`
- `primary_answer`
- `must_cover_subquestions`
- `required_entities`
- `evidence_points` or source constraints
- `conversion_path` when the page has a business goal

If one of these is missing, make the narrowest reasonable assumption and state
it in the output. Do not stop unless the gap would make the page misleading.

## Writing contract

The page must do all of the following:

1. Answer the main question early.
2. Give the reader a better result than generic AI summary sludge.
3. Make important claims easy to quote, verify, and extract.
4. Use a deliberate narrative formula before drafting, so the page has a
   shape instead of becoming an information dump.
5. Use clear structure so humans and AI systems can navigate the page fast.
6. Preserve entity clarity: products, tools, terms, and actors should never
   blur together.
7. Remove obvious AI-writing artifacts through audit and human judgment, not
   blind AI rewriting.

## Workflow

### 1. Lock the answer

Write the shortest honest answer to the core query first.

This answer should usually appear:

- in the intro
- in a direct definition block
- or in the first substantive section

If the page cannot answer the query directly, the page is probably poorly
scoped.

### 2. Choose the narrative formula

Pick one writing formula before drafting. The formula is the narrative frame;
the SEO/GEO pattern is the extraction frame. Use both.

Default choices:

- `QUEST`: tutorial, method, or workflow content
- `PAS`: pain-point and solution content
- `AIDA`: product, tool, or feature recommendation content
- `SCAR`: case study, lived experience, or postmortem content
- `Decision + BAB`: comparison and before/after decision pages
- `Contrarian hook + PAS`: AI search, GEO, or strategic opinion content

If none fits, state the chosen structure in plain language before drafting.

### 3. Build the skeleton before the draft

Do not jump from brief to full article. First create a compact skeleton with
5-8 lines:

- `hook`
- `core_answer`
- `formula_stage_map`
- `subquestion_map`
- `evidence_slots`
- `entity_slots`
- `quoteable_claims`
- `conversion_path`, when relevant

The skeleton is the real article plan. The draft should fill the skeleton, not
invent a new shape.

### 4. Build the page around subquestions

Turn the brief into a visible question hierarchy:

- main question
- decision questions
- comparison questions
- operational follow-ups

Each major section should resolve one subquestion cleanly. Avoid sections that
exist only to pad length or sprinkle keywords.

### 5. Write for information gain

The page must contain value beyond common-knowledge explanation.

Prefer:

- original framing
- operational detail
- real constraints
- specific examples
- explicit tradeoffs
- decision criteria
- process steps

Avoid:

- generic definitions with no applied value
- broad overviews that say nothing concrete
- summary paragraphs that could fit any tool or any company

### 6. Make the page extractable

AI systems are more likely to use content that is easy to segment and ground.
Use structure that helps extraction without becoming artificial:

- direct answer near the top
- clear `H2` / `H3` hierarchy
- short declarative sentences for key claims
- comparison tables when evaluating options
- step lists when explaining procedures
- checklists when helping decisions
- FAQ or follow-up questions when natural

Do not force all formats into every page. Use only the structures that improve
clarity.

### 7. Protect entity clarity

Be precise with names:

- product names
- feature names
- frameworks
- roles
- metrics
- workflows

If a term could mean multiple things, define it once and use it consistently.

### 8. Audit for human voice

Use AI to identify likely writing problems, not to blindly rewrite the whole
piece. Mark issues, then revise with judgment.

Check for:

- over-positioned claims that speak down to the reader
- template phrases such as "worth noting", "in conclusion", "unlock", or
  "empower" unless they are genuinely needed
- repeated symmetric sentence patterns
- mechanical numbered lists where prose would be clearer
- paragraph rhythm that stays the same for too long
- claims without a specific example, constraint, or evidence point
- generic endings that summarize instead of giving a decision or next step

The final page should still sound like a person with a point of view.

### 9. Write for readers first, extraction second

The page should feel useful to a serious reader, not optimized for a robot at
the reader's expense.

Prioritize:

- clarity
- specificity
- honesty about limits
- concrete examples
- clean navigation

## Default page shape

Use this structure unless the brief clearly calls for another pattern:

1. `Title`
2. `Direct answer intro`
3. `Why this matters` or immediate framing
4. `Core sections` mapped to subquestions
5. `Comparison / checklist / steps` when useful
6. `FAQ or follow-up questions` when useful
7. `Conclusion / decision guidance`
8. `CTA or next step` when relevant

See `references/writing-patterns.md` for page patterns.

## Output requirements

When delivering a draft, include:

- proposed `title`
- proposed `meta_description`
- `selected_formula`
- `content_skeleton`
- the full article body
- `schema_hints` if relevant
- `internal_link_suggestions`
- `platform_variants` when useful:
  - `clawlite_ready_markdown`
  - `x_thread`
  - `linkedin_post`
  - `faq_schema_hints`
  - `ai_answer_summary`
- `self_audit`

The `self_audit` must explicitly answer:

- Did the page answer the core query directly?
- Where is the strongest information gain?
- Which sections are most citeable or extractable?
- Is there any remaining commodity filler to cut?
- What AI-writing artifacts were found and fixed?
- What should a human review before publishing?

## Quality bar

The content passes only if it has:

- a direct answer near the top
- a visible section hierarchy
- consistent entity naming
- a selected narrative formula
- a compact skeleton before the draft
- at least one form of structured clarity where useful
  (`table`, `checklist`, `steps`, or `faq`)
- concrete claims instead of vague filler
- non-commodity value
- a human-voice audit that catches obvious AI artifacts

## Anti-patterns

- ❌ Keyword stuffing
- ❌ Generic AI filler paragraphs
- ❌ Letting AI choose the entire structure after receiving only a topic
- ❌ Asking AI to "make it sound human" without a specific audit checklist
- ❌ Fake certainty without evidence
- ❌ Definitions that never become actionable
- ❌ Section headings that repeat the same idea in different words
- ❌ Decorative references to AEO/GEO hacks with no user value
- ❌ Forcing FAQ, tables, or checklists where they do not help

## Boundary with other workflow stages

This skill assumes:

- topic qualification already happened
- information gain was already approved
- publishing happens elsewhere
- technical eligibility happens elsewhere

If the brief is weak, improve the writing angle locally, but do not silently
invent an entirely different topic.

## Related skills

- `skills/strategic-reading/SKILL.md` — map source material onto a specific problem
- `skills/article-enrichment/SKILL.md` — transform raw article dumps into structured pages
- `skills/gr-seo-patrol/SKILL.md` — technical and monitoring SEO/GEO patrol work
