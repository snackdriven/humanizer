# Humanizer

For when a perfectly ordinary paragraph starts talking about the evolving landscape.

A writing-editor skill for **Claude Code and OpenCode**. It looks for puffed-up phrasing, repetitive structure, and the little chatbot habits that survive a first rewrite. Give it a sample of your own writing so it has someone to sound like.

This fork adds Kayla's patterns for leaked citation tokens, forced slang, and other less obvious leftovers.

## Install

Use Git. Choose the directory for your tool. If it already contains a humanizer installation, back it up first.

### Claude Code

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/snackdriven/humanizer.git ~/.claude/skills/humanizer
```

### OpenCode

```bash
mkdir -p ~/.config/opencode/skills
git clone https://github.com/snackdriven/humanizer.git ~/.config/opencode/skills/humanizer
```

The installed skill is [SKILL.md](SKILL.md). There is no build step or package install.

## Give it something to edit

Invoke the skill and paste the draft:

```text
/humanizer

[paste your draft here]
```

For voice matching, include two or three paragraphs you've written and identify them as the sample. Put the draft after them.

The skill produces a rewrite, audits what still sounds generated, and revises again. Read the result before using it; the point still needs to be yours.

## 45 patterns detected

| Family | What it looks for |
| --- | --- |
| Content | Inflated importance and claims with nobody behind them |
| Language | Stock vocabulary and elaborate ways of saying “is” |
| Style | Manufactured punchlines, decorative formatting, and overworked punctuation |
| Chatbot habits | Flattery, canned closers, and cutoff disclaimers |
| Filler | Long ways of saying very little |
| Structural leftovers | Citation debris, bullet avalanches, forced slang, and uniform rhythm |

[The full catalog and worked example](docs/reference.md) keep the details off the front page. [SKILL.md](SKILL.md) defines the editing rules.

## Version history

**2.8.0+kayla** adds patterns 34–45 and guidance on older signals that have become less useful. [Full history](docs/reference.md#version-history).

[Upstream](https://github.com/blader/humanizer) · [MIT license](LICENSE)
