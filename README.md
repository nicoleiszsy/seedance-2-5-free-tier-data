# AI video model free-tier data

A dated record of what each channel actually grants on the free tier of AI video models — daily credits, daily generation caps, sign-up bonuses, clip length, extension ceiling, output resolution, watermark behaviour, and API availability.

Free-tier terms are the least documented part of an AI video product. Vendors publish a launch post with a headline number, then adjust the daily grant, move the watermark switch, or gate a model behind a membership tier. This dataset collects those figures in one place and **stamps every row with the channel it came from and the date it was observed**.

66 observations across Seedance 2.5, PixVerse, Runway, Wan 2.5, Kling AI, Sora 2 and Grok Imagine, current to 2026-10-04. File names keep the `seedance-2-5-free-tiers` stem for link stability; the files themselves are the full dataset, not Seedance-only extracts.

## Files

| File | Format | Use |
|---|---|---|
| [`data/seedance-2-5-free-tiers.csv`](data/seedance-2-5-free-tiers.csv) | CSV, UTF-8 | spreadsheets, pandas, `csv` module |
| [`data/seedance-2-5-free-tiers.json`](data/seedance-2-5-free-tiers.json) | JSON | includes field notes and the licence in the envelope |
| [`data/seedance-2-5-free-tiers.md`](data/seedance-2-5-free-tiers.md) | Markdown table | pasting into a document, an issue, or a pull request |

## Fields

| Field | Meaning |
|---|---|
| `model` | the model the figure applies to |
| `channel` | the product, platform or API the figure was observed on |
| `metric` | what is being measured |
| `value` | the figure, quoted as observed — ranges and hedges are kept, not flattened |
| `observed` | the date the figure was read or recorded |
| `source_type` | `vendor` = stated by the vendor · `report` = reported by a user · `single-source` = one uncorroborated account |
| `note` | caveats, conflicts, and what is known to be missing |

## Reading it correctly

**Some rows contradict each other on purpose.** Where two observations disagree — the daily credit figure in July versus August, the vendor saying the API is "coming soon" while a developer reports it opened two weeks earlier — both rows are kept. Neither was averaged into a number nobody published. If you need one value, decide which source you trust; the dataset will not decide for you.

**These numbers move without announcement.** A row is a record of what was true on its date, not a promise about today. Check `observed` before quoting anything as current.

**Nothing here is estimated.** Where a figure could not be confirmed against a primary source, the row says so in `note` and `source_type` reflects it. There are no interpolated values.

**Measured, not only quoted.** Most `vendor` rows are what a company published. Twelve rows are what happened when someone ran the product: an unauthenticated attempt to open the generator and the login wall it hit; a daily check-in grant of 6 credits that appears on no vendor page; the credits deducted by a 2-second, a 5-second and a 10-second generation; the resulting per-second rate; the free plan's duration ceiling; PixVerse's 50-credit deduction for a 5-second generation; and Kling's 66-credit trial package, its 2026-11-03 expiry and its 720P rate; and Runway's model picker, where four models are marked FREE. Both grades are marked, and the second is the rarer one.

## What is deliberately not in here

- **No invented price per generation.** Where a vendor's own published numbers allow a rate to be derived — Wan's credit listings all work out to 5 credits per video and 0.25 per image — the derived value is recorded in that row's `note` and marked as our arithmetic on the vendor's wording, not as a unit price the vendor states. Where a measured deduction gives a different rate (Wan: 6 credits for 2 s, 15 for 5 s, 30 for 10 s, i.e. 3 credits per second), both figures are kept side by side and neither is averaged. Nothing is interpolated, and no model gets a cost figure its vendor did not publish.
- **No "best model" ranking.** This is a record of terms, not a benchmark.
- **No scraped marketing copy.** Where a vendor's own wording matters, it is quoted, not paraphrased into something stronger.

## Source

Maintained alongside **[videofreetier.com](https://videofreetier.com/)** — the same figures appear there with the surrounding context, and corrections land on that page first. The dataset is the machine-readable half; the site is the readable half.

## Contributing

If a figure is out of date or wrong, open an issue with the correct value **and the date you observed it**. A correction carrying a date is worth more than the original row. Please do not send a value without a date — it cannot be merged into a dated dataset.

## Licence

[CC BY 4.0](LICENSE). Use it, quote it, build on it; credit VideoFreeTier and link back to https://videofreetier.com/.
