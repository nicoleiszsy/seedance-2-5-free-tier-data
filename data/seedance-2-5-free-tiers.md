# AI video model free-tier observations

Maintained by VideoFreeTier — https://videofreetier.com/

Coverage: Seedance 2.5, PixVerse, Runway and Wan 2.5 (more models added as they are verified).
Each row records what a channel granted or stated (or, for a documented absence, what the official pages do not state), on the date observed.
`source_type`: `vendor` = stated by the vendor, including officially published absences; `report` = reported by a user; `single-source` = one uncorroborated account.

| model | channel | metric | value | observed | source_type | note |
|---|---|---|---|---|---|---|
| Seedance 2.5 | Jimeng | daily free credits | 60-100 | 2026-07-04 | report | not a published figure; range as reported |
| Seedance 2.5 | Jimeng | daily free credits | 88 | 2026-08-11 | report | conflicts with the July figure above; no official statement |
| Seedance 2.5 | Doubao | daily generations (free tier) | 5 | 2026-08-11 | report | per account per day |
| Seedance 2.5 | Mina Labs | sign-up bonus | 20 credits | 2026-08-11 | report | one-off, new users |
| Seedance 2.5 | Lovart | annual plan bonus | up to 20 generations | 2026-08-11 | report | tied to an annual subscription |
| Seedance 2.5 | Doubao Work | launch giveaway | 30 days Standard membership (list CNY 68) | 2026-08-25 | report | desktop client + phone-number login required; inner quota unverified |
| Seedance 2.5 | ByteDance (official) | max clip length | 30 seconds, single pass | 2026-07-31 | vendor | up from 15 s in Seedance 2.0 |
| Seedance 2.5 | ByteDance (official) | extension ceiling | multi-minute, no round limit stated | 2026-07-31 | vendor | official wording is 'several minutes' |
| Seedance 2.5 | Jimeng (reported) | extension ceiling | 3 minutes, Jimeng-only | 2026-07-08 | report | official material confirms neither the number nor exclusivity |
| Seedance 2.5 | ByteDance (official) | output resolution | not stated | 2026-07-31 | vendor | the official post omits resolution entirely |
| Seedance 2.5 | most hosting platforms | output resolution | 1080p | 2026-07 to 2026-08 | vendor | as advertised on model landing pages |
| Seedance 2.5 | one hosting platform | output resolution claim | 4K | 2026 | vendor | single platform; contradicted by its own plan table |
| Seedance 2.5 | one pre-launch tester | output resolution | 4K + 10-bit | 2026-07-04 | single-source | source was under NDA; nothing else corroborates it |
| Seedance 2.5 | Doubao | watermark, free tier | watermarked | 2026-08-27 | report |  |
| Seedance 2.5 | Doubao | watermark, paid tier | removal off by default, manual toggle | 2026-08-27 | report | toggle path: generate, open full size, top-right menu, auto-remove watermark |
| Seedance 2.5 | Doubao | watermark, after the fact | not retroactive | 2026-08-27 | report | subscribing later does not strip watermarks already saved |
| Seedance 2.5 | BytePlus ModelArk | API availability | coming soon | 2026-07-31 | vendor | as stated in the official launch post |
| Seedance 2.5 | developer report | API availability | opened 2026-07-16 | 2026-07-15 | report | conflicts with the vendor statement; unresolved |
| Seedance 2.5 | API (in practice) | error codes seen | 429, 400, 402 | 2026-08-04 | report | 429 rate cap; 400 param limits; 402 insufficient balance |
| Seedance 2.5 | API (in practice) | error strings seen | api error: 529 overloaded; connection lost mid-response | 2026-08-25 | report |  |
| Seedance 2.5 | API (in practice) | billing on failure | moderation/platform failures not charged; dissatisfaction charged | 2026-08-04 | report |  |
| Seedance 2.5 | one host, 5 test groups | first-attempt usable rate | ~30% to >60% | 2026-08-12 | report | with structured prompts assigning one job per reference; one tester, not a benchmark |
| PixVerse | pixverse.ai (official site) | free-tier allowance figures | not published | 2026-10-02 | vendor | homepage and /zh/pricing checked 2026-10-02; /pricing returns 404; the official marketing site carries no free-tier credit figure; third-party guides claim 60 credits/day and a 90-credit sign-up bonus but no official page verifies it |
| PixVerse | app.pixverse.ai (official app) | plan and credit details | published only behind a human-verification wall | 2026-10-02 | vendor | automated access on 2026-10-02 met a Cloudflare human-check interstitial; plan figures exist but could not be read without an interactive session; third-party claims unverified |
| PixVerse | app.pixverse.ai (official app, pricing page) | free plan initial credits | 60 (one-time) | 2026-10-02 | vendor | pricing table: initial credits 60; read via an interactive browser session that passed the human check |
| PixVerse | app.pixverse.ai (official app, pricing page) | free plan daily credits | 30 per day | 2026-10-02 | vendor | pricing table: daily refresh 30 for the free plan; paid tiers get 60/day; contradicts third-party guides that claim 60/day for free (60 is the free tier's initial grant, and the paid tiers' daily figure) |
| PixVerse | app.pixverse.ai (official app, pricing page) | free plan video resolution ceiling | up to 540P | 2026-10-02 | vendor | paid tiers: up to 720P (Standard) and up to 4K |
| PixVerse | app.pixverse.ai (official app, pricing page) | watermark removal | paid plans only; no watermark-free row in the free tier column | 2026-10-02 | vendor | pricing table lists watermark-free output from the Standard tier upward |
| PixVerse | app.pixverse.ai (official app, pricing page) | free plan monthly membership credits | none (paid tiers: 1200-25000 per 30 days) | 2026-10-02 | vendor | credit packs sold separately: 500 credits $5, 2000 $20, 5000 $50, 10000 $100 |
| PixVerse | app.pixverse.ai (logged-in session) | credit deduction, one 5-second video generation | 50 credits | 2026-10-02 | report | site-measured: logged-in session, one 5-second generation on default app settings; credit record screenshot on file; not independently re-verified by a second party. Against the free grant: the 30/day refresh cannot fund one 5s generation (50 > 30); the one-time 60 covers exactly one, leaving 10 |
| Runway | runwayml.com (official pricing page) | free plan credits | 125 one-time credits | 2026-10-02 | vendor | plan table wording: 'Free forever... 125 one-time credits to explore Runway's AI tools' |
| Runway | runwayml.com (official pricing page) | free plan credit expiry | one-time deposit, does not expire | 2026-10-02 | vendor | FAQ wording: 'the Free plan includes a one-time deposit of 125 credits that doesn't expire' |
| Runway | runwayml.com (official pricing page) | credit consumption, Gen-4.5 | 12 credits per second of generated video | 2026-10-02 | vendor | from the pricing FAQ; the page states credit cost per generation depends on model, duration and resolution |
| Runway | runwayml.com (official pricing page) | free plan storage | 5GB asset storage | 2026-10-02 | vendor | free plan also includes 'a selection of generative creative models to test concepts' |
| Wan 2.5 | create.wan.video (official app, pricing page) | free plan credits per month | not published | 2026-10-03 | vendor | the Free column is the only one of the three plan columns without a credits-per-month figure; the same page states 300 for Pro and 1,200 for Premium |
| Wan 2.5 | create.wan.video (official app, pricing page) | free plan credit source | daily check-in; the amount is not stated | 2026-10-03 | vendor | page wording: 'Daily check-in to earn free credits'; no figure for it appears in any of the three tabs (Membership Plans, Credits, Gift Cards) |
| Wan 2.5 | create.wan.video (official app, pricing page) | free plan concurrent video submissions | 1 | 2026-10-03 | vendor | wording: 'Submit up to 1 video concurrently'; Pro 3, Premium 8 |
| Wan 2.5 | create.wan.video (official app, pricing page) | free plan concurrent image submissions | 1 | 2026-10-03 | vendor | wording: 'Submit up to 1 image concurrently'; Pro 3, Premium 5 |
| Wan 2.5 | create.wan.video (official app, pricing page) | free plan image styles | 6 | 2026-10-03 | vendor | wording: 'Access to 6 image styles'; the paid tiers get all image styles |
| Wan 2.5 | create.wan.video (official app, pricing page) | free plan watermark-free download | not listed | 2026-10-03 | vendor | 'Download watermark-free images & videos' appears in the Pro and Premium columns only |
| Wan 2.5 | create.wan.video (official app, pricing page) | free plan maximum video resolution | not listed | 2026-10-03 | vendor | 'Create High-Res Videos (1080p)' appears from Pro upward; the free column carries no resolution figure |
| Wan 2.5 | create.wan.video (official app, pricing page) | free plan video duration | not listed | 2026-10-03 | vendor | 'Create longer videos (10-30s)' appears from Pro upward; the free column states no duration |
| Wan 2.5 | create.wan.video (official app, pricing page) | paid tier credits per month | Pro 300; Premium 1,200 | 2026-10-03 | vendor | Pro US$5/month billed yearly (US$10 monthly); Premium US$20/month billed yearly (US$40 monthly); both auto-renew; the page notes the purchase covers model creation on create.wan.video only and that the API is a separate purchase |
| Wan 2.5 | create.wan.video (official app, pricing page) | one-time credit packs | 30 credits US$1.50 to 3,900 credits US$100 | 2026-10-03 | vendor | seven packs; the page's own 'Accelerate: up to N images or M videos' lines work out to 5 credits per video and 0.25 per image at every pack size and at both membership tiers (our arithmetic on the page's wording, not a unit price the page states); credits are non-refundable, non-transferable, 2-year validity on redemption |
| Wan 2.5 | create.wan.video (anonymous session) | login requirement for generation | account required; no anonymous generation path | 2026-10-03 | report | site-measured: headed browser session on 2026-10-03 opened /generate and was met immediately by a login modal ('Welcome to Wan / Log in / Don't have an account? Sign up'); screenshot on file; no prompt could be submitted without an account |
| Wan 2.5 | create.wan.video (logged-in session) | daily check-in grant | 6 credits | 2026-10-03 | report | site-measured: read from the logged-in free account on 2026-10-03; the pricing page states only that 'Daily check-in to earn free credits' and never gives the amount, so this figure exists nowhere on the vendor's pages; credit record screenshot on file; not independently re-verified by a second party |
| Wan 2.5 | create.wan.video (logged-in session) | credit deduction, one 2-second video generation | 6 credits | 2026-10-03 | report | site-measured: logged-in generation on 2026-10-03; screenshot on file; not independently re-verified by a second party. Against the free grant: 6 credits is the whole daily check-in, so the free tier funds exactly one 2-second clip per day |
| Wan 2.5 | create.wan.video (logged-in session) | credit deduction, one 5-second video generation | 15 credits | 2026-10-03 | report | site-measured: logged-in generation on 2026-10-03; screenshot on file; not independently re-verified by a second party. Against the free grant: 15 credits is two and a half daily check-ins, so a 5-second clip is never fundable by one day's grant |
| Wan 2.5 | create.wan.video (logged-in session) | credit deduction, one 10-second video generation | 30 credits | 2026-10-03 | report | site-measured: logged-in generation on 2026-10-03; screenshot on file; not independently re-verified by a second party. Against the free grant: 30 credits is five daily check-ins, so the longest clip the free tier allows costs five consecutive days of showing up |
| Wan 2.5 | create.wan.video (logged-in session) | credit consumption, measured | 3 credits per second of generated video | 2026-10-03 | report | site-measured: derived — our arithmetic on the three measured deductions above (6 for 2 s, 15 for 5 s, 30 for 10 s all return 3 per second); the vendor states no per-second rate. This is the comparable figure to Runway's vendor-stated 12 credits per second |
| Wan 2.5 | create.wan.video (logged-in session) | free plan duration ceiling | 2 s, 5 s and 10 s available; 20 s and longer requires a paid account | 2026-10-03 | report | site-measured: the free account's duration control offers 2 s / 5 s / 10 s, and choosing 20 s or more prompts an upgrade; screenshot on file; not independently re-verified by a second party. The plan table lists 'Create longer videos (10-30s)' from Pro upward and gives the free column no duration row at all |

License: CC BY 4.0. Source: https://videofreetier.com/
