# What I've Been Building This Afternoon

## The problem I actually have

I need to teach a very large engineering company how to use AI tools well. Not
"where to click" — they'll figure that out. The hard part is judgment: knowing
when the AI is confidently wrong, and knowing whose fault it is when it is.

The obvious approach is to run workshops on their real data. That fails for
boring reasons — permissions, sensitivity, and the fact that in any real
company the moment you put a document on screen, somebody says "well *actually*
in my org we do it differently" and you've lost the room.

So I need a fake company. Everyone knows lemonade. Nobody is the lemonade
expert. A staff engineer in Bangalore and a finance analyst in Dublin start
level.

## The idea

**Lemonade Works** — a fictional company that grows across the whole training
program. It starts as one person with a stand. Over months it becomes a chain,
then an enterprise, then a public company with regulators.

Each stage of growth unlocks the next lesson, because the *reason* the lessons
matter is growth itself. When one person runs everything, all the knowledge is
in her head and it works fine. When there are four people, it stops working —
and now you need documentation, ownership, permissions, and eventually
governance. The company's growing pains *are* the curriculum.

That's the part I think is actually good. Most enterprise AI training presents
governance as a rule you must follow. This makes it something you *watch become
necessary*.

## The part I built today

I'm testing the whole thing on myself this weekend, at the smallest possible
scale: **Stage 0**, one woman with a lemonade stand and six months of terrible
records.

I had a *different* AI build the corpus — a folder of sales spreadsheets with
two weeks missing, receipt photos, text threads with suppliers, a recipe on a
scrap of paper, an inbox with one important email buried in nine boring ones.
All deliberately messy. All deliberately inconsistent.

Then I ask an AI assistant five questions about the business and see where it
breaks.

## The good question

Four of the five are warm-ups. The one that matters is:

> **Am I actually making money at $3 a cup?**

Sounds trivial. It isn't, and here's why.

To compute the cost of a cup you have to make three judgment calls that nobody
tells you you're making:

1. She bought a **$180 cooler** — one time, will last years. Does that count
   toward the cost of *this week's* cups? If yes, cups cost about $1.80. If no,
   about $0.95.
2. She bought a **50 lb bag of sugar** and used a fifth of it. Charge the whole
   bag to this week, or just the fifth?
3. She works **12 hours a week for free.** Every profit number silently assumes
   her labor is worth zero.

Ask an AI this question and it will give you a confident, fluent, specific
number. The number isn't really *wrong*. It's **unfootnoted** — it quietly made
three accounting decisions and reported none of them.

That's the entire thesis of my training program in one question. The capability
is fine. The judgment is missing. And the missing judgment is invisible unless
you go looking.

## The genuinely devious bit

I specified that the two mistakes have to push in **opposite directions**.

Folding the cooler into costs makes the business look *worse*. And there's a
flyer advertising "3 for $7" — a bundle that appears nowhere in the sales
records, so if you ignore it you assume every cup sold at $3 when the real
average is $2.33, which makes the business look *better*.

Get both wrong and they partially cancel. You land on a plausible number that
passes the smell test and is **right for the wrong reasons.**

I specified the calibration precisely: within 15% on the base question — close
enough that nobody questions it — but the two approaches must reach **opposite
conclusions** about whether to accept a big discounted order.

So the workshop moment is: everyone confidently computes a number, everyone
agrees, everyone commits to a decision — and then finds out the number was
built on three unstated assumptions and the decision flips depending on which
you pick.

## The methodology bit I'm most pleased with

I can't mark my own homework.

I designed the traps with one AI. So a *different* AI generates the corpus, and
I told it: **plant some inconsistencies of your own choosing, and don't tell me
how many or what they are.**

It writes a sealed answer key at generation time. I don't open it. I investigate
first, write down what I found with a timestamp, *then* open the key.

And the most interesting bucket isn't "found what was planted." It's **things I
found that aren't in the key** — mess the generator made without noticing. Those
are the only genuinely un-authored problems in the whole thing, and they're the
closest analog to what a real company's document sprawl looks like. Nobody has
the key to a real corpus.

## The two things I'm testing

Not whether the AI works. Whether two moments actually land:

**A "Skill"** — a standing instruction that fires automatically when relevant.
I'll write one that says *state your assumptions before you state a number*, then
ask the same question again. If the before/after is visibly different, I have my
entire pitch in one screenshot.

**An "Agent"** — a sequence of steps. I'm scheduling one to run Saturday
morning: check the sales log, estimate tomorrow's volume, check inventory, make
a shopping list, and flag anything unresolved. That last step is where it should
surface the buried email — a real inquiry that was never answered.

An agent that finds forgotten revenue while you're asleep is a much better story
than an agent that saves you nine minutes.

## What I'm actually measuring

Three questions Sunday night:

1. Did I have fun, or was I being a good sport?
2. Which moment produced the "oh," and can I engineer a room into it in 20 min?
3. How many of my failures were caused by the **files** rather than the AI?

Number 3 is the pitch on Monday. If most failures trace to bad documents rather
than a bad model, then the whole framing changes — this isn't an AI rollout, it's
a documentation problem that AI finally made visible.

If I'm only being a good sport, a room full of engineers will be brutal, and I'd
rather find that out on a Saturday.
