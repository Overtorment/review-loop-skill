# review-loop

One command for a review → validate → fix loop on your current changes.

Type `/review-loop` and your agent will:

1. Review the changes (correctness, performance, robustness), using the [superpowers](https://github.com/obra/superpowers) code-review skill when available.
2. Check that the code is elegant, readable and not overengineered.
3. Validate every finding and fix the valid ones worth fixing.
4. Repeat until a review round finds no major issues (nitpicks and minor issues don't count).

## Install

Copy `SKILL.md` into your agent's skills folder, for example:

```sh
mkdir -p ~/.cursor/skills/review-loop && curl -fsSL https://raw.githubusercontent.com/Overtorment/review-loop-skill/main/SKILL.md -o ~/.cursor/skills/review-loop/SKILL.md
```

Use `~/.claude/skills/review-loop/` for Claude Code or `~/.codex/skills/review-loop/` for Codex.

## License

MIT
