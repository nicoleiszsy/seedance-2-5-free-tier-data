# Seedance 2.5 free-tier data

A dated record of what each channel actually grants on the **Seedance 2.5** free tier — daily credits, daily generation caps, sign-up bonuses, clip length, extension ceiling, output resolution, watermark behaviour, and API availability.

Free-tier terms are the least documented part of an AI video product. Vendors publish a launch post with a headline number, then adjust the daily grant, move the watermark switch, or gate a model behind a membership tier. This dataset collects those figures in one place and **stamps every row with the channel it came from and the date it was observed**.

28 observations across Seedance 2.5, PixVerse and Runway, current to 2026-10-02.

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

## What is deliberately not in here

- **No price per generation.** Prices change, and the credit-to-generation conversion rate is not published anywhere that could be verified. Any currency figure would have been an invention.
- **No "best model" ranking.** This is a record of terms, not a benchmark.
- **No scraped marketing copy.** Where a vendor's own wording matters, it is quoted, not paraphrased into something stronger.

## Source

Maintained alongside **[videofreetier.com](https://videofreetier.com/)** — the same figures appear there with the surrounding context, and corrections land on that page first. The dataset is the machine-readable half; the site is the readable half.

## Contributing

If a figure is out of date or wrong, open an issue with the correct value **and the date you observed it**. A correction carrying a date is worth more than the original row. Please do not send a value without a date — it cannot be merged into a dated dataset.

## Licence

[CC BY 4.0](LICENSE). Use it, quote it, build on it; credit VideoFreeTier and link back to https://videofreetier.com/.
