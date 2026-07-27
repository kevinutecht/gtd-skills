# GTD Skills

Generic [Codex](https://developers.openai.com/codex/) skills for a Markdown-based GTD system.

## Included skills

- `accountability-partner` reviews a weekly board and writes concrete feedback with `gtd partner write` when available.
- `gtd-brainstorm` creates 30 grounded, non-duplicative ideas in `brainstorm.md`.

## Install

Copy the desired skill directories into your Codex skills folder:

```bash
cp -R skills/accountability-partner skills/gtd-brainstorm ~/.codex/skills/
```

The skills read `GTD_DATA_DIR` when set and otherwise use `~/data/gtd`.

## Privacy

These skills contain no personal data or sample life history. Keep personal GTD data outside this repository.
