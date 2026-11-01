---
layout: single
title: "Come installare una skill in Claude: tre strade"
date: 2026-11-01
permalink: /blog/installare-skill-claude/
excerpt: "Claude.ai, Claude Code e la CLI skills: i passaggi indicati dai README ufficiali."
categories:
  - Guide
ref: installare-skill-claude
---

I passaggi qui sotto sono quelli indicati dai README di [MotionSites](https://github.com/Motionsites-AI/claude-skill) e [/awwwards](https://github.com/juliobsz/skills). I nomi dei menu possono cambiare: se non li trovi, guarda la documentazione di Claude.

## 1. Claude.ai e app desktop
1. Scarica lo zip della skill dalla pagina delle release del repository (MotionSites distribuisce `motionsites-web-builder.zip`).
2. In Claude apri **Customize → Skills → + → Create skill → Upload a skill**, scegli lo zip e attiva la skill.
3. Serve l'esecuzione di codice attiva in Impostazioni → Capabilities.

## 2. Claude Code, come plugin
Per MotionSites:
```
/plugin marketplace add Motionsites-AI/claude-skill
/plugin install motionsites-web-builder@motionsites
```
Se non hai una chiave SSH per GitHub, usa l'indirizzo completo: `/plugin marketplace add https://github.com/Motionsites-AI/claude-skill.git`.

## 3. Con la CLI skills
```
npx skills add juliobsz/skills -g
```
La CLI riconosce i tuoi agenti (Claude Code, Codex, Cursor, Gemini CLI e altri) e ti fa scegliere dove installare. Poi apri una **nuova** sessione, perché gli agenti leggono le skill all'avvio. Aggiornamento: `npx skills update -g`. Rimozione: `npx skills remove awwwards jury -g`.

## Due avvertenze
- **Leggi il `SKILL.md`** prima di installare: la skill fa eseguire script al tuo agente.
- Il README di /awwwards segnala che la CLI raccoglie dati d'uso anonimi; si disattivano con `DISABLE_TELEMETRY=1`.

Non installare la stessa skill in due modi (plugin e CLI), o ti comparirà due volte. Guide alle singole skill: [MotionSites]({% include url-ref.html ref="motionsites-web-builder" %}) e [/awwwards]({% include url-ref.html ref="awwwards-skill" %}).
