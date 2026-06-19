# Bullet Background Paper (BBP) Report Writing Skill

Create concise, evidence-backed Bullet Background Paper (BBP) reports with AI assistants. This repo includes a Codex skill and Claude-ready instructions for decision memos, research summaries, incident recaps, provider comparisons, and review-ready Markdown or HTML artifacts.

## What Is BBP?

A Bullet Background Paper is a short, structured write-up that helps a busy reviewer understand the question, facts, caveats, and next decision quickly.

The BBP style is useful when dense notes, research, or investigation findings need to become precise, scoped, and easy to review.

## What This Includes

- `codex/bbp-report-writing/`: a Codex skill folder with `SKILL.md` and `openai.yaml`.
- `claude/bbp-report-writing.md`: a Claude-ready instruction file for Claude Projects, `CLAUDE.md`, or direct chat use.

## Best Use Cases

Use these instructions when turning dense notes into:

- decision memos
- research summaries
- incident recaps
- provider or vendor comparisons
- technical investigation summaries
- project status artifacts
- Markdown or HTML reports for team review

## Install

Set the raw file URL once:

```bash
BBP_SKILLS_URL="https://raw.githubusercontent.com/bowang-solutionstream/bullet-background-paper-report-writing-skill/main"
```

### Option A: Codex Skill

Install globally for Codex:

```bash
mkdir -p ~/.codex/skills/bbp-report-writing/agents

curl -fsSL "$BBP_SKILLS_URL/codex/bbp-report-writing/SKILL.md" \
  -o ~/.codex/skills/bbp-report-writing/SKILL.md

curl -fsSL "$BBP_SKILLS_URL/codex/bbp-report-writing/agents/openai.yaml" \
  -o ~/.codex/skills/bbp-report-writing/agents/openai.yaml
```

Then start a new Codex session and use:

```text
Use $bbp-report-writing to turn this evidence into a concise BBP-style report.
```

### Option B: Claude Project Instructions

Create a new `CLAUDE.md` file:

```bash
curl -fsSL "$BBP_SKILLS_URL/claude/bbp-report-writing.md" \
  -o CLAUDE.md
```

Append to an existing `CLAUDE.md` file:

```bash
printf "\n\n" >> CLAUDE.md

curl -fsSL "$BBP_SKILLS_URL/claude/bbp-report-writing.md" \
  >> CLAUDE.md
```

In Claude App, you can also open `claude/bbp-report-writing.md` and paste it into project instructions or project knowledge.

### Option C: Preview Before Installing

```bash
curl -fsSL "$BBP_SKILLS_URL/claude/bbp-report-writing.md"
```

## Public-Safe Content Rule

This repo is intended for reusable process guidance only. Do not add credentials, private evidence, private messages, provider payloads, or sensitive project data.
