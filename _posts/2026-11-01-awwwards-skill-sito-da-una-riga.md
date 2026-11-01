---
layout: single
title: "/awwwards: la skill che costruisce un sito partendo da una riga"
date: 2026-11-01
permalink: /blog/awwwards-skill-sito-da-una-riga/
excerpt: "Come lavora /awwwards di juliobsz, cosa serve per usarla e perché i suoi autori avvertono che richiede tempo e token."
categories:
  - Guide
ref: awwwards-skill
---

[/awwwards](https://github.com/juliobsz/skills) è una skill per agenti AI (Claude Code, Codex, Antigravity e altri) con licenza MIT. La promessa del README è un sito di livello "Awwwards" da un brief di una sola riga, per esempio "fammi un portfolio, mi chiamo Ana". Questo articolo riassume il README; non l'abbiamo ancora provata su un progetto reale.

## Le fasi del lavoro
| Fase | Cosa succede |
|---|---|
| Brief | Deduce pubblico e scopo; i dati mancanti diventano ipotesi scritte |
| Concept | Tre idee da territori diversi, valutate per originalità e coerenza |
| Direzione artistica | Palette, font gratuiti, griglia e movimento, scritti in `DESIGN.md` |
| Costruzione | HTML semantico, poi animazioni e un momento "firma" |
| Controllo qualità | Build di produzione, audit SEO e accessibilità, screenshot in browser reale su desktop e mobile |
| Consegna | Immagine social, favicon, sitemap e, solo dopo la tua conferma, il deploy |

## Tecnologie
Di default Next.js; Astro per siti di soli contenuti dove conta il movimento. Il movimento usa GSAP, Lenis e OGL per il WebGL.

## Cosa non fa
Secondo il README: niente finti premi, loghi o numeri inventati, niente lorem ipsum. Ciò che è inventato viene segnato come segnaposto e listato a fine lavoro.

## Cosa serve
Node 22.20 o superiore per la CLI, Playwright per gli screenshot e un modello capace di leggere immagini. Il deploy richiede un account Vercel, Netlify o Cloudflare, solo se lo vuoi.

## I limiti dichiarati
- **Richiede tempo**: una sessione completa è lunga e usa molti token, non è uno snippet veloce.
- **Dipende dal modello**: concept e controllo visivo valgono quanto il modello che li esegue.
- **I contenuti veri sono tuoi**: senza progetti, foto e testi reali restano segnaposto da sostituire.

## /jury
Nello stesso repo c'è /jury, che valuta qualsiasi sito come una giuria: misura LCP, CLS, accessibilità e SEO e produce una scheda con le correzioni in ordine di importanza. Il README precisa che non è affiliata ad Awwwards e che la stima si basa su due soli siti vincitori.

Installazione: [guida]({% include url-ref.html ref="installare-skill-claude" %}). Confronto con un'altra skill: [MotionSites contro /awwwards]({% include url-ref.html ref="motionsites-vs-awwwards" %}).
