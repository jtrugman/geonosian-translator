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
git clone https://github.com/jtrugman/geonosian-translator.git ~/.claude/skills/geonosian-translator
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

## Examples

### Command

> **Input:** "Everyone retreat immediately!"

**LAVA OH SH SH SH VOTE TITO HOLE' '**

*Literally:* command — immediately — everyone — retreat (with terminal gravity).

*Translator's notes:* `LAVA` opens as the imperative expletive; the high-low click closes with command-weight. No trill needed — the command itself is the attention call.

---

### Prophetic / formal

> **Input:** "Behold, the day of reckoning has come, and our enemies shall fall."

**RRRRR... OD' ' GUI KURKA-A ABOOT' ' INYURKA**

*Literally:* listen — behold (gravity) — now death-comes (to) enemies (gravity) — god help us.

*Translator's notes:* Full theatrical register. Opening trill for prophecy-framing. `KURKA-A` ("death-go") stretches canonical roots into "the reckoning comes." `INYURKA` closes the dire prophecy.

---

### Unilateral command

> **Input:** "I forbid you to speak of this."

**UNALUI AIE-NOA''**

*Literally:* I (commanding) speak-cannot (extreme).

*Translator's notes:* Pure unilateral command — exactly the case `UNALUI` is reserved for. Double-click `''` closes with the extreme-importance marker, signaling decree, not request.

---

### Casual sentiment with a vocabulary gap

> **Input:** "I love my parents."

**OD K'TITO**

*Literally:* behold the makers.

*Translator's notes:* Geonosian nobility has no canonical word for "love" or "parents" — the culture doesn't foreground tender sentiment. `OD` (witness/behold/revere) stretches toward reverence; `K'TITO` is invented as a compound for "progenitors / makers" and flagged.

---

### Cultural substitution

> **Input:** "Begin the executions."

**GUI BARA HYUNDAI''**

*Literally:* now (let begin) the sacred-ritual-combat (extreme).

*Translator's notes:* "Executions" is never translated literally — `BARA HYUNDAI` is the cultural equivalent, the sacred festival of ritual combat and sacrifice.

For more worked examples (questions, heavy-gap fictions, register edge cases), see [references/examples.md](references/examples.md).

## Files

- [SKILL.md](SKILL.md) — the skill instructions Claude follows
- [references/lexicon.md](references/lexicon.md) — canonical Geonosian vocabulary and morphology
- [references/examples.md](references/examples.md) — worked translations across registers

## Credits

The lexicon and grammar rules encoded in this skill are based on the YouTube breakdown ["Learn to Speak Geonosian!"](https://youtu.be/2vqsJC4sYig), which reverse-engineers Geonosian from Episode II. All credit for the underlying rule set goes to the creator of that video. This repo just packages those rules as a Claude Agent Skill so Claude can apply them consistently to new English input.

## License

See [LICENSE](LICENSE).
