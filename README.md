# Instagram Manager

> Paste your bio, your last posts and your Insights numbers. Get an audit, content pillars, a 2-week calendar, Reel and carousel drafts, captions, hashtag sets, reply templates and a weekly review, in one honest loop.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Skill](https://img.shields.io/badge/Claude-Skill-D97757.svg)](SKILL.md)
[![Price: Free](https://img.shields.io/badge/price-free-brightgreen.svg)](#license)

A free, text-only skill by Codelady Abroad for students, beginners, small shops and personal brands. It runs anywhere a plain prompt runs: Claude Code, the Claude app, other agents or a website form. No scripts, no account access, no paid APIs.

## The loop

1. **Audit** of the profile from what you paste: score out of 20 and the top 3 fixes.
2. **Pillars:** 3–4 content themes tied to your goal.
3. **2-week calendar:** Reels, carousels, photos and stories you can really make.
4. **Drafts:** Reel hooks and shot lists, carousel slides, story ideas.
5. **Captions** with alt text and one CTA, plus **hashtags in rotating sets** of 3–5.
6. **Reply templates** for price questions, collabs, complaints, praise and scam DMs (AZ / RU / EN).
7. **Weekly review** from pasted numbers: save, share and follow rates against your own median, then repeat / fix / stop.

## What it never does

- Never asks for your password or login codes.
- Never automates likes, follows, comments or DMs, and never suggests bought followers or engagement pods.
- Never hides ads: paid, gifted and affiliate posts get the "Paid partnership" label and a clear word in the caption; realistic AI media gets the "AI info" label.
- Never invents your numbers or promises growth.

## Example request

> I teach beginner coding in Azerbaijani on Instagram (@example). Goal: 20 students for my online course in December. I can make 3 posts a week and I'm OK filming myself. Bio: "Proqramlaşdırma öyrədirəm 💻 | DM yazın". Last posts: 4 Reels with tips, 3 photos of my desk, 2 course ads. Make me a plan.

## Install

- **Claude Code:** copy this folder to `~/.claude/skills/instagram-manager/`.
- **Claude app:** zip the folder (with `SKILL.md` inside `instagram-manager/`) and upload it under *Customize → Skills*.
- **Any other agent or a web form:** use the body of `SKILL.md` as the system prompt. `references/` holds optional format guides and reply templates.

Test prompts and expected points: [`evals/evals.json`](evals/evals.json).

## Sources and credits

Written from scratch. Ideas and rules come from:
- Instagram's creators site (creators.instagram.com), Adam Mosseri's ranking explainers and Instagram Community Guidelines
- Meta Business Help Centre (Insights definitions, Paid partnership label, branded content rules)
- Ideas from MIT-licensed single-task skills found in Codelady Abroad's research, which this skill joins into one loop: `ig-audit`, `ig-dm` and `ig-reel` by Jakeschincariol, `ig-content-planner`, `ig-caption-writer` and `ig-hashtag-strategist` by sergebulaev, and `social` by coreyhaines31. No text was copied.

## License

[MIT](LICENSE) © 2026 Codelady Abroad
