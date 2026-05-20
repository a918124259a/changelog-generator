# Changelog Generator

A bash script that automatically generates a structured `CHANGELOG.md` from your project's git history.

## Quick Start

```bash
bash changelog.sh        # Generate CHANGELOG.md in current directory
bash changelog.sh /path  # Generate for a specific repo
```

## Features

- Auto-categorizes commits into: ✨ Added / 🐛 Fixed / 🔧 Changed / ❌ Removed
- Works from the last git tag (or entire history if no tags exist)
- Proper Markdown output with timestamps and commit references
- No dependencies beyond bash 4+ and git
- One command, zero config

## How It Works

The script parses your git log and categorizes commits based on conventional commit prefixes:

| Prefix | Category |
|--------|----------|
| feat: add: create: new: | Added |
| fix: patch: hotfix: | Fixed |
| remove: delete: deprecate: | Removed |
| (everything else) | Changed |

## Output

Writes `CHANGELOG.md` with sections, timestamps, and short commit hashes.

## License

MIT
