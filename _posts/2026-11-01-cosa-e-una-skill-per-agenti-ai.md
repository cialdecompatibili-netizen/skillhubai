---
layout: single
title: "Che cos'è una skill per agenti AI"
date: 2026-11-01
permalink: /blog/cosa-e-una-skill-per-agenti-ai/
excerpt: "Una skill è una cartella di istruzioni che l'agente segue: ecco cosa contiene, dove si installa e cosa controllare prima."
categories:
  - Guide
ref: cosa-e-una-skill
---

Una **skill** è, in pratica, una cartella con dentro un file `SKILL.md`: le istruzioni che l'agente AI legge e segue quando gli chiedi un certo tipo di lavoro. Può contenere anche esempi, script e materiali di riferimento.

È il modo in cui gli agenti stanno imparando a fare bene cose specifiche, per esempio costruire un sito o valutarne la qualità, invece di dare ogni volta risposte generiche.

## Dove funzionano
Secondo la documentazione dei progetti che seguiamo, lo stesso formato è letto da più agenti: Claude Code, Codex, Cursor, Gemini CLI, OpenCode, Copilot e altri. Cambia solo la cartella in cui si installano.

## Cosa controllare prima di installarne una
Una skill è un insieme di istruzioni che il tuo agente esegue, e alcune fanno lanciare build e script sul tuo computer. Il consiglio che dà il progetto [/awwwards]({% include url-ref.html ref="awwwards-skill" %}) è semplice: **leggi il `SKILL.md` prima di installarla**, come faresti con qualsiasi codice che esegui.

## Cosa trovi in questo blog
Riassumiamo in italiano le skill che stanno crescendo, partendo da ciò che dichiarano i loro README ufficiali, con limiti e costi. Per ora:

- [MotionSites Web Builder]({% include url-ref.html ref="motionsites-web-builder" %}), per landing page cinematografiche
- [/awwwards]({% include url-ref.html ref="awwwards-skill" %}), per costruire un sito da una riga di descrizione
- [Come installare una skill in Claude]({% include url-ref.html ref="installare-skill-claude" %})
