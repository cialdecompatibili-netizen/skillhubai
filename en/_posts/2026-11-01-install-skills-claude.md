---
layout: single
title: "How to install a skill in Claude: three ways"
date: 2026-11-01
permalink: /en/blog/install-skills-claude/
excerpt: "Claude.ai, Claude Code and the skills CLI: the steps given in the official READMEs."
categories:
  - Guides
lang: en
locale: en
ref: installare-skill-claude
tr: tradotto
tr_hash: yisooh
---

The steps below are the ones given in the READMEs of [MotionSites](https://github.com/Motionsites-AI/claude-skill) and [/awwwards](https://github.com/juliobsz/skills). Menu names can change: if you cannot find them, check Claude's documentation.

## 1. Claude.ai and the desktop app
1. Download the skill's zip from the repository's releases page (MotionSites ships `motionsites-web-builder.zip`).
2. In Claude open **Customize → Skills → + → Create skill → Upload a skill**, choose the zip and switch the skill on.
3. Code execution must be enabled in Settings → Capabilities.

## 2. Claude Code, as a plugin
For MotionSites:
```
/plugin marketplace add Motionsites-AI/claude-skill
/plugin install motionsites-web-builder@motionsites
```
If you have no GitHub SSH key, use the full address: `/plugin marketplace add https://github.com/Motionsites-AI/claude-skill.git`.

## 3. With the skills CLI
```
npx skills add juliobsz/skills -g
```
The CLI detects your agents (Claude Code, Codex, Cursor, Gemini CLI and more) and lets you pick where to install. Then open a **new** session, because agents read skills at startup. Update: `npx skills update -g`. Remove: `npx skills remove awwwards jury -g`.

## Two warnings
- **Read the `SKILL.md`** before installing: a skill makes your agent run scripts.
- The /awwwards README notes that the CLI collects anonymous usage data; turn it off with `DISABLE_TELEMETRY=1`.

Do not install the same skill two ways (plugin and CLI) or it will show up twice. Guides to the individual skills: [MotionSites]({% include url-ref.html ref="motionsites-web-builder" %}) and [/awwwards]({% include url-ref.html ref="awwwards-skill" %}).
