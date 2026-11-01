---
layout: single
title: "MotionSites Web Builder: the free skill for cinematic landing pages"
date: 2026-11-01
permalink: /en/blog/motionsites-web-builder/
excerpt: "What the MotionSites skill contains, how it works and where the free part ends and the paid part begins."
categories:
  - Guides
lang: en
locale: en
ref: motionsites-web-builder
tr: tradotto
tr_hash: 66qrjm
---

[MotionSites Web Builder](https://github.com/Motionsites-AI/claude-skill) is a free skill for Claude. The stated idea in its README: make the AI build "award-level" landing pages instead of the usual average layouts. This post summarises that README; we have not yet tried it on a real project and we will say so when we do.

## Why AI-built pages look alike
According to the authors, for three reasons: a vague plan, no real media, and nobody looking at the result. The skill addresses all three: it studies the most-liked MotionSites designs, picks real media, writes a precise spec, builds the page and then **screenshots its own work and fixes it**.

## What is inside
- 40 example prompts, the most-liked free ones on MotionSites
- a media shelf: more than 50 hero videos, 30 transparent 3D cut-outs and 29 images
- more than 55 technique recipes with working code (video loops, liquid glass, word-by-word blur headlines, 3D scenes with Three.js and more)
- taste rules with real numbers: type scale, spacing, colour, motion timing
- a spec template and a QA script (broken assets, mobile overflow, fonts, video playback)
- "prompt mode": instead of code you get a prompt for Lovable, Bolt, v0, Cursor, Manus, Google AI Studio or Kimi

## Free part and paid part
The included examples and media are a **free sample**. The full library is called MotionSites Unlimited and is paid: according to the README it includes more than 500 premium prompts, animated backgrounds, Lovable templates and an MCP. We are not affiliated with MotionSites.

## License
The skill's instructions and code are MIT. The example prompts and media remain MotionSites' property, but the README says you may use them in sites built with the skill.

## How to use it
Once installed, just ask Claude for a site, for example a landing page for a sleep-tracking ring or a homepage for an architecture photographer. For installation see our [guide]({% include url-ref.html ref="installare-skill-claude" %}). For a comparison with another skill: [MotionSites vs /awwwards]({% include url-ref.html ref="motionsites-vs-awwwards" %}).
