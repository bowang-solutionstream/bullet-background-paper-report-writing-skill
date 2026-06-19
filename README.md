# Bullet Background Paper (BBP) Report Writing Skill

Portable skills for AI assistants that help teams produce concise, evidence-backed Bullet Background Paper (BBP) reports and review artifacts.

## What Is BBP?

BBP means Bullet Background Paper: a short write-up that helps a busy reviewer understand the question, facts, caveats, and next decision quickly.

The BBP style is useful when dense notes need to become precise, scoped, and review-ready.

## Included Skills

- `bbp-report-writing`: creates or revises BBP-style reports, decision memos, research summaries, incident recaps, provider comparisons, technical investigation summaries, project status artifacts, and HTML/Markdown reports.

## Best Use Cases

Use this skill when turning dense notes into:

- decision memos
- research summaries
- incident recaps
- provider or vendor comparisons
- technical investigation summaries
- project status artifacts
- HTML or Markdown reports for team review

## Install

Set the repo raw URL once:

```bash
BBP_SKILLS_URL="https://raw.githubusercontent.com/<owner>/bullet-background-paper-report-writing-skill/main"
```

Replace `<owner>` with the GitHub owner or organization that hosts this repo.

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

New Claude project or repo:

```bash
curl -fsSL "$BBP_SKILLS_URL/claude/bbp-report-writing.md" \
  -o CLAUDE.md
```

Existing `CLAUDE.md`:

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

This repo is intended for reusable process guidance only. Do not add credentials, raw client evidence, private messages, provider payloads, or sensitive project data.
