# Help — Claude Code Skill

List all installed custom skills with descriptions, usage examples, and file paths. Your skill directory assistant.

## Prerequisites

- [Claude Code](https://claude.ai/claude-code) CLI installed
- GitHub CLI (`gh`) for one-line install

## Installation

**One-line install:**

```bash
gh repo clone chethanbhatbs/skill-tree ~/.claude/skills/skill-tree
```

**Manual install:**

```bash
git clone https://github.com/chethanbhatbs/skill-tree.git
cp -r help-skill/ ~/.claude/skills/skill-tree/
```

**Verify it's installed:**

```bash
ls ~/.claude/skills/skill-tree/
```

You should see `SKILL.md` (and any other skill files).

## Usage

```
/help                   # List ALL custom skills in a table
/help skill-name        # Detailed info for a specific skill
```

### What it does

1. Scans `~/.claude/skills/` for all installed skills
2. Parses each `SKILL.md` for name, description, and arguments
3. Shows a formatted table (all skills) or detailed view (single skill)

### Output example

```
| Skill         | Description                    | Usage              |
|---------------|--------------------------------|--------------------|
| /investigate  | Query emergent.sh databases... | /investigate <id>  |
| /learnings    | Capture what you learned...    | /learnings [topic] |
| /organize     | Sort Downloads, screenshots... | /organize [mode]   |
```



## How Claude Code Skills Work

Skills are markdown files in `~/.claude/skills/` that give Claude Code specialized instructions for specific tasks. When you invoke a skill (e.g., `/Help`), Claude reads the `SKILL.md` and follows its instructions.

## Uninstall

```bash
rm -rf ~/.claude/skills/skill-tree
```

## License

MIT
