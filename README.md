# geonosian-translator

A Claude Code Agent Skill that translates English into **Geonosian** — the noble hive-tongue of Poggle the Lesser and the Geonosian aristocracy from Star Wars.

The skill renders English with the martial-theatrical character of the Geonosian court: click consonants, capitalized stress, attention trills, ritual gravity, and intelligent gap-handling for concepts the hive's nobility doesn't have native vocabulary for.

## What it does

Given an English phrase, the skill produces:

- The Geonosian translation
- A literal word-for-word gloss
- Translator's notes explaining register, invented words, omitted bulk, and cultural substitutions (e.g., `BARA HYUNDAI` for "executions")

It matches register: casual sentences stay plain, while formal, commanding, or prophetic input earns the full theatrical treatment — opening trills, terminal click patterns, and `INYURKA` where warranted.

## Installation

### Option A — Clone into your skills directory

```bash
git clone https://github.com/<your-username>/geonosian-translator.git ~/.claude/skills/geonosian-translator
```

### Option B — Download and copy

1. Download this repo (Code → Download ZIP, or `git clone`).
2. Copy the folder into `~/.claude/skills/` and rename it to `geonosian-translator` if needed.

The final layout should look like:

```
~/.claude/skills/geonosian-translator/
├── SKILL.md
└── references/
    ├── lexicon.md
    └── examples.md
```

Restart Claude Code (or start a new session) and the skill will be available.

## Usage

Once installed, just ask Claude for a Geonosian translation. The skill triggers automatically on prompts like:

- "Translate this to Geonosian: *Everyone retreat immediately!*"
- "How would Poggle the Lesser say *Behold, the day of reckoning has come*?"
- "Render *I forbid you to speak of this* in the hive tongue."

## Files

- [SKILL.md](SKILL.md) — the skill instructions Claude follows
- [references/lexicon.md](references/lexicon.md) — canonical Geonosian vocabulary and morphology
- [references/examples.md](references/examples.md) — worked translations across registers

## License

See [LICENSE](LICENSE).
