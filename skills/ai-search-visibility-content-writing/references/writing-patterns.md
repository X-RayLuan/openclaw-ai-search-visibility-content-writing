# Writing Patterns

Use these patterns when the brief already passed information-gain
qualification and the task is now to produce strong AI search visibility
content.

## Formula selector

Choose a narrative formula before drafting. Then pair it with one of the page
patterns below.

| Content job | Formula | Use when |
| --- | --- | --- |
| Teach a process | `QUEST` | The reader needs to complete a workflow or learn a method. |
| Solve a painful problem | `PAS` | The page should name a problem, show its cost, and give a concrete fix. |
| Recommend a product or feature | `AIDA` | The page needs attention, interest, desire, and action. |
| Share a real case or lesson | `SCAR` | The strongest value is lived experience, conflict, and outcome. |
| Compare options | `Decision + BAB` | The reader needs before/after contrast and a recommendation. |
| Make a strategic claim | `Contrarian hook + PAS` | The page challenges a common assumption and must prove why. |

Formula and page pattern are not the same thing:

- formula = narrative momentum
- page pattern = extraction and navigation

## Pattern 1: Answer-first explainer

Use when the user asks a definitional or operational question.

Recommended shape:

1. selected formula, usually `QUEST` or `PAS`
2. direct answer
3. short framing
4. how it works
5. why it matters
6. common mistakes
7. FAQ

Good for:

- "what is X"
- "how does X work"
- "when should I use X"

## Pattern 2: Decision page

Use when the query implies selection, comparison, or tradeoffs.

Recommended shape:

1. selected formula, usually `Decision + BAB`
2. direct recommendation
3. who each option is for
4. comparison table
5. tradeoffs
6. decision checklist
7. final recommendation

Good for:

- "X vs Y"
- "best tool for Z"
- "which approach should I choose"

## Pattern 3: Workflow guide

Use when the page should help a reader complete a process.

Recommended shape:

1. selected formula, usually `QUEST`
2. direct outcome statement
3. prerequisites
4. step-by-step workflow
5. failure points
6. verification checklist
7. next actions

Good for:

- operational playbooks
- onboarding guides
- implementation walkthroughs

## Pattern 4: FAQ cluster page

Use when the main value is answering a tight family of related questions.

Recommended shape:

1. selected formula, usually `PAS` for pain-led pages or `QUEST` for
   education-led pages
2. core answer
3. grouped FAQ sections
4. short answers first, elaboration second
5. related decisions or caveats

Good for:

- support content
- fast-answer pages
- query families with multiple follow-ups

## Skeleton template

Use this before writing the full draft:

```text
selected_formula:
hook:
core_answer:
formula_stage_map:
subquestion_map:
evidence_slots:
entity_slots:
quoteable_claims:
conversion_path:
```

Keep it short. If the skeleton needs more than 8 lines, the article probably
has too many search intents.

## Human voice audit

After drafting, scan for:

- over-positioned claims that talk down to the reader
- template phrases: "worth noting", "in conclusion", "unlock", "empower",
  "seamless", "robust", "leverage"
- repeated sentence shapes, especially balanced "not X but Y" patterns
- mechanical lists that should become prose
- paragraph rhythm that stays flat for too long
- claims with no example, constraint, evidence point, or boundary condition
- endings that summarize instead of helping the reader decide

Do not ask the model to rewrite the entire piece to sound human. Identify
specific problems, then revise only the lines that need it.

## Content moves that usually help

- Put the clearest sentence on the page near the top.
- Pick the formula before drafting.
- Build a 5-8 line skeleton before writing prose.
- Use tables only when comparison is the job.
- Use steps only when sequence matters.
- Use checklists only when evaluation matters.
- Use FAQ only when real follow-up questions exist.
- Prefer short, declarative claims over long soft paragraphs.
- Turn strong claims into standalone quotable sentences.

## Content moves that usually hurt

- Repeating the keyword in every heading
- Padding with history or background that does not help the query
- Using generic intros before answering the question
- Hiding the recommendation until the end
- Mixing multiple search intents into one page without a clear center
- Letting AI generate the whole structure from a topic alone
- Running a vague "make this more human" rewrite pass
