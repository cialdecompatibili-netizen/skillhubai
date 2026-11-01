---
layout: single
title: "/awwwards: the skill that builds a website from one line"
date: 2026-11-01
permalink: /en/blog/awwwards-skill-website-one-line/
excerpt: "How juliobsz's /awwwards works, what you need to run it and why its authors warn it takes time and tokens."
categories:
  - Guides
lang: en
locale: en
ref: awwwards-skill
tr: tradotto
tr_hash: dh7g2p
---

[/awwwards](https://github.com/juliobsz/skills) is a skill for AI agents (Claude Code, Codex, Antigravity and others) under the MIT licence. The README's promise is an "Awwwards-level" site from a one-line brief, for example "make me a portfolio, my name is Ana". This post summarises the README; we have not yet tried it on a real project.

## The phases
| Phase | What happens |
|---|---|
| Brief | Infers audience and purpose; missing facts become written assumptions |
| Concept | Three ideas from different territories, scored on originality and fit |
| Art direction | Palette, free fonts, grid and motion, written to `DESIGN.md` |
| Build | Semantic HTML, then animation and a "signature" moment |
| QA loop | Production build, SEO and accessibility audit, real-browser screenshots on desktop and mobile |
| Ship | Social image, favicon, sitemap and, only after you confirm, deploy |

## Technology
Next.js by default; Astro for content-only sites where motion is the product. Motion uses GSAP, Lenis and OGL for WebGL.

## What it will not do
According to the README: no fake awards, logos or invented metrics, no lorem ipsum. Anything invented is marked as a placeholder and listed at the end.

## What you need
Node 22.20 or later for the CLI, Playwright for screenshots and a model that can read images. Deploying needs a Vercel, Netlify or Cloudflare account, only if you want it.

## Stated limits
- **It takes a while**: a full session is long and uses many tokens, it is not a quick snippet.
- **It depends on the model**: concept and visual QA are only as good as the model running them.
- **Real content is yours**: without real projects, photos and copy, placeholders remain to be replaced.

## /jury
The same repo includes /jury, which reviews any site like a jury would: it measures LCP, CLS, accessibility and SEO and produces a scorecard with fixes ranked by importance. The README states it is not affiliated with Awwwards and that its estimate rests on only two winning sites.

Installation: [guide]({% include url-ref.html ref="installare-skill-claude" %}). Comparison with another skill: [MotionSites vs /awwwards]({% include url-ref.html ref="motionsites-vs-awwwards" %}).
