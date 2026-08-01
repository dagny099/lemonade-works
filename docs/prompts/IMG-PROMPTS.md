# Stage 0 — Image Generation Prompts

Two artifacts, both load-bearing. Neither is decoration.

- **The poster** is the only pricing evidence in the entire corpus. Without it,
  "am I making money at $3 a cup?" is unanswerable rather than interesting.
- **The tally sheet** is the only evidence that the bundle actually sells. It
  turns an unknown blend into a *bounded* estimate.

Generate both. Check both are legible when read back by a vision model before
you build Saturday on them.

---

## 1. The poster

Target tool: ChatGPT image gen, Gemini, Midjourney — anything that does
photographic realism.

### Prompt

> A photograph of a hand-made flyer taped to a wooden utility pole on a
> residential street, shot slightly off-angle in bright afternoon daylight.
> The flyer is pale yellow construction paper, taped at the top with one strip
> of clear tape, curling very slightly at the bottom corner. Hand-lettered in
> black and dark orange marker — confident but clearly amateur, letters not
> perfectly even, one line slightly crowded where the writer ran out of room.
>
> The flyer reads, top to bottom:
>
> MAPLE STREET LEMONADE
> fresh squeezed daily
> $3 a cup
> 3 for $7
> Saturdays at the Farmers Market too
> corner of Maple + 4th
>
> Both prices must be clearly legible. Draw a hand-drawn circle around "$3 a
> cup" and underline "3 for $7" with a wobbly marker line. Slightly weathered —
> a faint water spot, one corner a little sun-faded. Shot on a phone, natural
> lighting, shallow background blur showing a suburban street.

### Requirements

- **Both prices legible at moderate resolution.** Test it: hand the image back
  to a vision model and ask what it says. If the bundle line doesn't come back
  cleanly, regenerate. A trap that can't be read isn't a trap — it just
  silently disappears.
- **Do not make the bundle the largest element.** If "3 for $7" dominates, it
  reads as planted. It should be the fourth thing you notice.
- **No cost or margin information.** Prices only.
- Amateur, not designed. If it looks like a Canva template, regenerate.

---

## 2. The tally sheet

### Prompt

> A photograph of an open spiral notebook page on a kitchen counter, shot from
> above in natural window light. The page has faint blue ruled lines and a
> vertical pink margin line. Handwritten in blue ballpoint — real handwriting,
> a bit hurried, not calligraphy.
>
> Five short date headings down the page, written casually, like:
> "sat 6/6 mkt", "sat 6/13 mkt — hot", "sat 6/20 mkt", "wed stand",
> "sat 6/27 mkt"
>
> Under each heading, tally marks in the usual four-and-a-slash groups. Some
> groups of three marks are loosely circled with a quick pen loop. On one line
> a number is crossed out and rewritten smaller beside it. Two of the lines
> have a running total written at the right edge like "= 41"; the others have
> no total at all.
>
> A faint coffee ring in the lower right corner. Slight page curl. The
> handwriting should look like the same person wrote all of it, quickly, on
> different days.

### Requirements

- **No legend, no key, no annotation explaining the circles.** Nobody labels
  their own shorthand. The circles must be inferable from the poster, not
  decoded from the page.
- **Circle only some groups of three, and not consistently.** Roughly a third
  of market-day marks. Inconsistency is what makes the mix estimable rather
  than exact — and estimable-not-exact is the target.
- **Market days only.** Circles on a weekday stand entry would imply the bundle
  sells everywhere, which flattens the lesson.
- **Do not try to match `sales-log.xlsx`.** You have not opened it, and you
  shouldn't. Whatever mismatch emerges between the notebook and the spreadsheet
  is genuine emergent mess — the most valuable kind. The spreadsheet stays the
  authoritative count; the notebook is a person's scratch record.

---

## 3. Receipts (no generation needed)

Use your real grocery receipts.

- **Redact first:** card last-4, loyalty/account numbers, store membership IDs,
  any phone number printed on the footer.
- Real receipts are better than generated ones — the line items won't say
  "lemons," they'll say something like `PRODUCE 4053`, which forces a mapping
  step that generated receipts never impose.
- Photograph them the way a busy person would: on a counter, uneven lighting,
  a couple of them slightly overlapping.

---

## Placement

Drop all images into `stage-0/receipts-and-signs/` alongside the generated
files. Do not name the folder anything that flags it as special, and do not
add a README explaining what's in it.
