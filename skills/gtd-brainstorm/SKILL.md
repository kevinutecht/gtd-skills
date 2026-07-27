---
name: gtd-brainstorm
description: Generate grounded, non-duplicative ideas from a Markdown-based GTD system. Use when a user asks for fresh GTD ideas, next projects, life-area ideas, or to refresh brainstorm.md during a weekly review.
---

# GTD Brainstorm

Generate 30 useful ideas from the user's actual GTD data. Favor ideas that fit the user's goals, available resources, and current commitments over generic aspiration lists.

## Data Root

Use `GTD_DATA_DIR` when it is set. Otherwise use `~/data/gtd`.

Read the files that exist, prioritizing:

- `purpose.md`, `vision.md`, `areas.md`, and `goals.md`
- `projects.md` and `someday-maybe.md`
- recent files in `weekly/`
- `brainstorm.md` to avoid duplicates

Use `calendar.md`, `waiting-for.md`, `agendas.md`, or `inbox.md` only when they add relevant context.

## Generate Ideas

Find gaps between horizons and active work, momentum worth extending, stalled commitments, useful cross-pollination, and realistic stretch opportunities.

Generate 30 ideas across these categories:

1. Projects and active work
2. Creative and personal interests
3. Learning and growth
4. Community and relationships
5. Wild cards

Keep ideas specific enough to start. Include a mix of quick wins, medium-term projects, and longer-term possibilities. Respect constraints visible in the data, including time, energy, and budget.

## Write `brainstorm.md`

Preserve prior ideas that are still relevant and not duplicated. Write the result to `$GTD_DATA_DIR/brainstorm.md` using this shape:

```markdown
# Brainstorm

*Generated: YYYY-MM-DD*

## Projects and Active Work

- [ ] Specific idea with brief context

## Creative and Personal Interests

- [ ] Specific idea with brief context

## Learning and Growth

- [ ] Specific idea with brief context

## Community and Relationships

- [ ] Specific idea with brief context

## Wild Cards

- [ ] Specific idea with brief context

## Existing Ideas (Kept)

- [ ] A non-duplicated prior idea
```

If the file is shown in a terminal viewer, wrap lines near 110 characters. Use `- [ ]` so ideas remain actionable.

## Quality Bar

- Ground each idea in a goal, area, project, weekly pattern, or stated interest.
- Do not duplicate existing ideas or disguise a duplicate with new wording.
- Prefer practical, low-friction starts over vague advice.
- Include some stretch ideas, but avoid unrealistic or expensive suggestions unless the data supports them.
- Do not infer personal facts that are absent from the GTD files.
