---
layout: single
title: "MotionSites Web Builder: la skill gratuita per landing page cinematografiche"
date: 2026-11-01
permalink: /blog/motionsites-web-builder/
excerpt: "Cosa contiene la skill di MotionSites, come lavora e dove sta il confine tra parte gratuita e parte a pagamento."
categories:
  - Guide
ref: motionsites-web-builder
---

[MotionSites Web Builder](https://github.com/Motionsites-AI/claude-skill) è una skill gratuita per Claude. L'idea dichiarata nel README: far costruire all'AI landing page "da premio" invece dei soliti layout medi. Questo articolo riassume quel README; non l'abbiamo ancora provata su un progetto reale e ve lo diremo quando lo faremo.

## Perché le pagine fatte dall'AI si assomigliano
Secondo gli autori per tre motivi: un piano vago, nessun contenuto multimediale vero e nessuno che guardi il risultato. La skill interviene su tutti e tre: studia i design più apprezzati di MotionSites, sceglie media reali, scrive una specifica precisa, costruisce la pagina e poi **si fa uno screenshot del proprio lavoro e lo corregge**.

## Cosa c'è dentro
- 40 prompt di esempio, i più apprezzati tra quelli gratuiti di MotionSites
- uno scaffale di media: più di 50 video hero, 30 ritagli 3D trasparenti e 29 immagini
- più di 55 ricette di tecniche con codice funzionante (loop video, liquid glass, titoli con blur parola per parola, scene 3D con Three.js e altre)
- regole di gusto con numeri reali: scala dei caratteri, spaziature, colori, tempi di animazione
- un modello di specifica e uno script di controllo (asset rotti, overflow su mobile, font, riproduzione video)
- la modalità "prompt": invece del codice ottieni un prompt per Lovable, Bolt, v0, Cursor, Manus, Google AI Studio o Kimi

## Parte gratuita e parte a pagamento
Esempi e media inclusi sono un **campione gratuito**. La libreria completa si chiama MotionSites Unlimited ed è a pagamento: secondo il README comprende più di 500 prompt premium, sfondi animati, template Lovable e un MCP. Noi non siamo affiliati a MotionSites.

## Licenza
Le istruzioni e il codice della skill sono MIT. I prompt di esempio e i media restano di MotionSites, ma il README dice che puoi usarli nei siti costruiti con la skill.

## Come si usa
Dopo l'installazione basta chiedere un sito a Claude, per esempio una landing per un anello di monitoraggio del sonno o una home per un fotografo di architettura. Per l'installazione vedi la nostra [guida]({% include url-ref.html ref="installare-skill-claude" %}). Per un confronto con un'altra skill: [MotionSites contro /awwwards]({% include url-ref.html ref="motionsites-vs-awwwards" %}).
