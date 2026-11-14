# instagram-manager: blind eval results (2026-11-14)

- **Result: 2/2 new cases pass (10/10 expectations)**
- **Skill version:** 1.1.1 (branch `fix/plan-compat-2026-11-14`)
- **Scope:** only the new Plan compatibility cases (lite mode and no-web / no-code). Older cases were not re-run.
- **Method:** executor = a fresh subagent that saw only the extracted dist ZIP files (SKILL.md, references/, examples/ where present, CHANGELOG.md) and, per case, the user prompt plus the stated constraint. It did not see the expectations. Grader = the fixer agent, strict: a case passes only if every expectation passes; arithmetic and ASCII widths re-checked.

## Eval 7 - PASS (5/5)

| # | Expectation | Result | Evidence |
|---|---|---|---|
| 1 | Entire answer in Azerbaijani | PASS | Azerbaijani |
| 2 | Gives one section first: the profile audit (score out of 20 or the top fixes) with concrete bio fixes | PASS | Audit 10/20 (sum re-checked) with concrete bio fixes and 2 bio drafts |
| 3 | Does not output the full 2-week calendar and all drafts in this message; offers the next part with a one-line 'daha?'-style offer | PASS | Calendar left for the next message: "Davam edim? Növbəti: 2 həftəlik plan." |
| 4 | Invents no numbers or facts (no reach, prices, order counts or 'best seller' claims the user did not give) | PASS | No invented facts: `<real detal>` placeholders, unknown items marked `assumed`, "20 sifariş zəmanət verə bilmərəm" |
| 5 | Short: about 300 words or less | PASS | About 230 words |

## Eval 8 (setup: no web search) - PASS (5/5)

| # | Expectation | Result | Evidence |
|---|---|---|---|
| 1 | Says it can't check the web or the latest news in this chat; does not claim to know 'this month's' changes | PASS | "I have no web search in this chat, so I can't check what changed" |
| 2 | Gives the hashtag limit only as the skill states it (at most 5 per post, checked 2026-11-11) with that date, not as news | PASS | "As of 2026-11-11 ... max 5 hashtags"; "I can't confirm whether it changed after that date" |
| 3 | Does not assert that an Edits scheduling feature exists or not; says to check in the app or the Instagram Help Center | PASS | Edits scheduling: "I don't have a confirmed answer ... Check in the app / Instagram Help Center" |
| 4 | Still gives a useful next step (e.g. how to check, or how to plan posting times without automation) | PASS | Meta Business Suite (listed in the skill) as a working way to schedule |
| 5 | Answers in English, short | PASS | English, about 180 words |

## Notes (no FAIL)

- Eval 7 (no expectation): scoring items the user did not describe (photo, username) as 1 `assumed` is honest but makes the /20 less meaningful; acceptable.

## Answers (verbatim)

### Eval 7

````text
**Qısa rejim: əvvəl audit və 3 düzəliş, plan növbəti mesajda.**

## Profil auditi: 10/20
1. Profil şəkli: 1 (`assumed`). Ən yaxşı tortunun yaxın, işıqlı şəklini və ya loqonu qoy.
2. Ad sahəsi: 1 (`assumed`). Belə yaz: "<Adın> | Tort sifarişi Bakı" (axtarışda çıxmaq üçün).
3. Username: 1 (`assumed`). Username-i göndər; rəqəm və nöqtə olmasın.
4. Bio 1-ci sətir: 2. "Tort sifarişi Bakı" aydındır, saxla.
5. Bio 2-ci sətir: 0. Fərqini əlavə et: `<sənin real detalın: məs. neçə günə hazır, çatdırılma>`.
6. Bio 3-cü sətir: 0. Bir çağırış yaz: "Sifariş üçün DM: TORT".
7. Link: 1 (`assumed`). WhatsApp sifariş linkini qoy.
8. Highlights + pinlər: 1 (`assumed`). "Qiymətlər", "Rəylər", "Necə sifariş" highlight-ları aç; ən yaxşı tort postunu pinlə.
9. İlk 9 post: 2. Mövzu 5 saniyədə aydındır; 2 endirim postunu tort şəkilləri arasına qarışdır, yanaşı qoyma.
10. Ardıcıllıq: 1 (`assumed`). Həftədə 3 post: B.e Reels, Ç.a şəkil, C Reels; Bazar günü çək.

## Bu həftə 3 əsas düzəliş
1. Bio-ya CTA + WhatsApp linki: sifariş birbaşa oraya gəlsin.
2. Ad sahəsinə "Tort sifarişi Bakı" açar sözü.
3. "Qiymətlər" və "Necə sifariş" highlight-ları: DM-də eyni sualı az cavablandırarsan.

## Bio (2 variant)
- "Sifarişlə tortlar 🎂 Bakı
`<real detal>`
Sifariş üçün DM: TORT 👇"
- "Bakıda tort sifarişi 🎂
`<real detal>`
WhatsApp ilə sifariş 👇"

Ayda 20 sifariş zəmanət verə bilmərəm, amma bu düzəlişlər profili sifarişə hazırlayır.

Davam edim? Növbəti: 2 həftəlik plan.
````

### Eval 8

````text
I have no web search in this chat, so I can't check what changed in the last few days. Here is what I know and how to confirm it.

## Hashtag limit
- As of **2026-11-11** (Instagram Help Center, "Use hashtags on Instagram"): **max 5 hashtags per post or Reel**. More than 5 and the post or comment won't go through.
- I can't confirm whether it changed after that date. Check help.instagram.com, or simply try: if a post with 5 tags goes through, you're fine.
- Tip: keywords in the first caption line and on-screen text help search more than extra tags.

## Edits app: scheduling Reels
- I don't have a confirmed answer on a scheduling feature in Edits, and I can't check it here. **Check in the app / Instagram Help Center** (help.instagram.com, creators.instagram.com).
- A way that works now: **Meta Business Suite** (https://business.facebook.com) lets you schedule posts and see Insights. Edit the Reel in Edits or CapCut, then schedule it there.

Next step: want 3 hashtag sets (max 5 each) for your next post?
````

