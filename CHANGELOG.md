# Changelog

All notable changes to this project are documented here.
The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and the project uses [Semantic Versioning](https://semver.org/).

## [1.1.0] - 2026-11-11

Research-driven features before the Agensi listing (open-skills research, 2026-11-11).

### Added
- `references/growth-playbook.md`:
  - current limits and specs, each marked official or "check in app";
  - Instagram SEO;
  - **Trial Reels** hook tests;
  - **Story sequences**;
  - **daily outbound comment plan**;
  - **collab posts, collab pitch and brand-deal** templates;
  - **repurpose one idea into a week**;
  - **competitor outlier review**;
  - **human-voice check**.
- Audit: name field as Instagram SEO; **pinned posts** added to the highlights item.
- Weekly review leads with **sends per reach** and marks outliers at 2× the user's own median.
- `examples/nail-studio-week-plan.md`.
- Agensi frontmatter (`version`, `summary`, `tags`, `keywords`, `use_cases`), `scripts/build-agensi-zip.ps1`, `LISTING.md`, evals 4–6 and blind test results in `tests/`.

### Fixed (checked on official Instagram/Meta help pages, 2026-11-11)
- **Hashtags: Instagram allows at most 5 per post**; with more, the post or comment won't go through. Previously "Instagram now focuses on a few".
- AI label: the "Add AI label" toggle, which shows as "AI content". It is needed for photorealistic video or realistic-sounding audio. Previously the old name "AI info".
- Caption preview of about 125 characters is marked as observed, not official. Carousels up to 20 and Reels up to 3 minutes are marked "check in app".
- Giveaways: never offer money for engagement (Community Guidelines).

### Fixed (blind evals, 2026-11-11)
- Audit always scores all 10 rows with a total /20 (missing items scored 1 and marked `assumed`).
- 4-column phone calendar with Stories in both weeks; full-plan checklist.
- One CTA = one action (never "save and send"), also in formats.md.
- Length budget, no invented facts (`<placeholder>`), no guessed gender in RU/AZ.
- Weekly review always ends with the adjusted next 2 weeks; median rule for formats with few posts.
- Story plan: one 3–5 frame sequence first.
- Explanations always in the user's language; captions in the audience's language.
- No invented first-person claims ("I tested these"); `<your real detail>` instead. Full plan includes one carousel written slide by slide.
- Every audit row ends with an action (examples given); full plan always includes a Reel draft and a carousel; Trial Reel slots get a fallback post.

## [1.0.0] - 2026-11-10

### Added
- First release: audit /20, pillars, 2-week calendar, Reel and carousel drafts, captions with alt text and hashtag sets, reply templates in AZ/RU/EN, weekly review from pasted Insights, no bots or bought followers, labels for ads and AI content. MIT.
