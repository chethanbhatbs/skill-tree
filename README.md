# Help — Claude Code Skill

List all available custom skills with descriptions, usage, and examples. Your skill directory assistant.

## Usage

```
/help              # List ALL custom skills in a table
/help skill-name   # Detailed info for a specific skill
```

## What it does

1. Scans `~/.claude/skills/` for all installed skills
2. Parses each `skill.md` for name, description, and arguments
3. Displays a formatted table or detailed view

## Output

**All skills:**
```
| Skill | Description | Usage |
|-------|-------------|-------|
| /investigate | Query databases... | /investigate <job_id> |
| /learnings | Capture learnings... | /learnings [topic] |
```

**Single skill:**
```
## /skill-name
Description: ...
Arguments: ...
Examples: ...
File: ~/.claude/skills/skill-name/skill.md
```

## Installation

```bash
cp -r help ~/.claude/skills/
```

## License

MIT
