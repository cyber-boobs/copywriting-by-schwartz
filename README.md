# copywriting-by-schwartz

**English** · [Русский](README.ru.md)

A Claude skill that writes ads using Eugene Schwartz's method from *Breakthrough Advertising* (1966).

Schwartz believed the analysis comes first and the copy comes second. So before writing a word, the skill works out:

- which mass desire already exists in the market;
- which of the five levels of awareness the buyer is at, from "unaware of the problem" to "knows the product and wants it";
- what the market has already heard from competitors: its stage of sophistication, and whether a new mechanism is needed;
- and so where the headline has to start.

Only then does it write headlines, using the 38 verbalization techniques, and body copy, using the 7 techniques: Intensification, Identification, Gradualization, Redefinition, Mechanization, Concentration and Camouflage.

The skill's instructions are written in Russian, but it writes copy in whatever language you ask for.

## What it does

- Headlines and Google Ads RSA sets (15 × 30 and 4 × 90 characters)
- Ad creatives and short-form video scripts
- Above-the-fold landing page copy, long-form landing pages, sales letters, VSLs
- Emails
- Diagnosing why an ad stopped working, and how to stand out when every competitor promises the same thing

## Installation

### Claude Code

```bash
git clone https://github.com/cyber-boobs/copywriting-by-schwartz.git ~/.claude/skills/copywriting-by-schwartz
```

To update:

```bash
git -C ~/.claude/skills/copywriting-by-schwartz pull
```

### Claude.ai and Claude Desktop

Download `copywriting-by-schwartz.zip` from [Releases](https://github.com/cyber-boobs/copywriting-by-schwartz/releases) and upload it under Skills in settings.

## Usage

Run `/copywriting-by-schwartz`, or just mention Schwartz, levels of awareness or market sophistication. For example:

- "Using Schwartz, write 15 RSA headlines for an eSIM service, in English, 30-character limit"
- "Why did this creative burn out? Break it down by awareness level"
- "Every competitor promises the same thing. How do we stand out?"

The skill starts by showing an analysis map (desire, awareness level, sophistication stage, headline entry point) and only then writes the copy.

## Contents

| File | What's inside |
|---|---|
| `SKILL.md` | the method step by step, workflow, checklist, what not to do |
| `references/awareness-sophistication.md` | mass desire, 5 levels of awareness, 5 stages of sophistication, how they combine, how they map to channels |
| `references/headline-verbalization.md` | 38 ways to strengthen a headline, which to use at each stage, rules for RSA |
| `references/seven-techniques.md` | the 7 body copy techniques |
| `references/final-touches.md` | Verification, Reinforcement, Interweaving, Sensitivity, Momentum, Mood, short video, final checklist |

## Notes

- This is a retelling and adaptation of the method in my own words, not the text of the book. The book is worth reading in full.
- The examples in the reference files are illustrative only: numbers are replaced with `[N]` and mechanisms are marked `[если правда]` ("if true"). The skill never carries them into your copy as facts. It takes facts only from your brief, your website or your answers.
- The skill refers to other skills (`copywriting`, `ad-creative`, `copy-editing`, `copywriting-by-shugerman` and others). It works fine without them; it just won't suggest switching.
