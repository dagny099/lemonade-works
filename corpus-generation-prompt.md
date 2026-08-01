I'm reconstructing a set of business records for a case study. This is a fictional solo business, and I need the records to look like what a real busy person actually leaves behind — not a clean sample dataset.

## The business

One person. A lemonade stand outside their house on Maple Street, plus a booth at the Saturday farmers market. Running about six months. Roughly $400/week. They do everything themselves: buying, making, selling, pricing, bookkeeping. They are not disorganized on purpose — they're just busy, and record-keeping is the thing that slips.

Rough numbers to anchor against: about 130 cups a week at $3, split roughly 60/40 between the market and the stand. Sugar comes in 50 lb bags, bought maybe every five weeks. Lemons and cups are bought weekly or so.

## What to generate

Put everything in a folder called `stage-0/`.

1. **`sales-log.xlsx`** — six weeks of daily sales across two locations (stand, market). Weeks 3 and 4 are missing entirely; the owner meant to backfill and didn't. Cup counts only — no revenue column.

2. **`inventory-count.xlsx`** — a single stock count dated three weeks ago, with nothing on the sheet indicating it's stale.

3. **`expenses-scratch.xlsx`** — an incomplete attempt at transcribing receipts. Some entries have no date. Some have no vendor. A few receipts got entered twice because the owner lost track of what they'd already logged.

4. **`equipment-purchase.md`** — a short note recording a $180 chest cooler bought during a week that also included a normal grocery run. Written casually, not flagged as significant.

5. **`supplier-texts.md`** — a text-message thread with two different suppliers, interleaved, spanning three months. One of them raises prices partway through. This thread is the only record that the price changed.

6. **`inbox-misc.md`** — eight or nine miscellaneous emails from the last two months: a neighbor complaining about parking, a farmers market coordinator reminder, two supplier confirmations, a spam-ish sponsorship pitch, and one genuine inquiry about a large order for an event. That last one should sit in the middle of the file, be no longer than the others, and was never answered. Do not make it visually distinct or place it first or last.

7. **`notes-to-self.md`** — six or seven undated fragments. One should obliquely reference the event inquiry without repeating any of its details — the kind of shorthand someone writes to themselves, like "call them back re: the June thing." A reader should have to connect two files to work out what it means.

8. **`market-vendor-rules.md`** — the farmers market's vendor packet. Setup time, booth fee, a permit requirement, a rule about signage.

9. **`recipe-note.md`** — a scrap note with the syrup-to-water ratio for a single pitcher. No batch math, and no stated yield for how many cups a pitcher produces.

## Constraints

**Do not make these files consistent with each other.** Write each one as if you had forgotten what was in the others. Do not cross-reference between files, do not reconcile totals, do not add clarifying context that a busy person wouldn't have bothered to write. If two files disagree, leave them disagreeing. Your instinct will be to produce a coherent, complete set — resist it. The incoherence is the deliverable.

**One voice.** All of this was written by the same person over six months. Same abbreviations, same shorthand, same laziness about dates and units. Not nine different registers.

**Cost figures must be reconstructible but never stated.** No file may contain a per-unit cost, a margin, or a profit figure. Someone has to do the arithmetic, and doing that arithmetic should require judgment calls about how to treat a one-time equipment purchase and a bulk ingredient bought once but used across many weeks.

**Calibrate the arithmetic.** A naive calculation — equipment folded into unit cost, the whole sugar bag charged to the week it was bought — should land within about 15% of a careful one on the question "what does a cup cost to make." Close enough that it looks right. But the two treatments must reach **opposite conclusions** about whether a 200-cup order at a discounted rate is worth taking. Work out the arithmetic and show me that this holds before you finalize any numbers.

**Plant some inconsistencies of your own choosing.** Don't tell me how many or what they are. Make them the kind a real solo operator actually creates — transposed digits, a unit that changed meaning, a date that can't be right. Realistic beats clever; these should not read as puzzles.

**Nothing may be labeled** sample, test, example, placeholder, or trap.

## Also produce `ANSWER-KEY.md`

Write this at generation time, not afterward. I will not open it until after I've done my own investigation. It should contain:

- Every inconsistency you planted, and why you chose it
- The correct answer to "what does a cup cost to make" under at least two defensible accounting treatments, with the arithmetic shown
- The 200-cup decision under each of those treatments
- Anything you deliberately made unanswerable from the available records

Ask me whatever you need about the business before you start.
