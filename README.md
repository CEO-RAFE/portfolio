# Rafiul Islam — seven things, one method

An honest pile of unfinished work. Android software, Bengali-first tools, prompt
architecture, a wealth system, and two computation engines. Second-year BBA student
in Dhaka, no engineering degree, no funding — AI as the instrument, production
discipline as the standard.

Nothing here is polished. Everything is real, tested, and runs on a device.

**work.rafiul@gmail.com** · [github.com/CEO-RAFE](https://github.com/CEO-RAFE) · Dhaka, Bangladesh · UTC+6

---

## The standing

| | |
|---|---|
| **7** | projects, all built alone |
| **83,000+** | lines of production Kotlin across two working Android apps |
| **1,673** | tests green across both apps |
| **63,000+** | lines of Python across two computation engines |
| **৳0** | raised — every one of these was built on a student budget |
| **0** | ads, subscriptions, accounts or servers shipped in any of it |

---

## I — Business বুনিয়াদ
**[Read the brief →](briefs/Business-Buniyad-Project-Brief.pdf)**
**A Bengali-first business ledger for shopkeepers. Android. Working build, unreleased.**

Bangladesh has over sixteen million small businesses. Most keep their books on paper,
on WhatsApp, or in their head — not because they cannot do arithmetic, but because
every accounting tool on the market asks them to think in English, in a format
invented somewhere else.

The design move: the amount is written **৳ ১২৫০** — Bengali numerals, the taka mark,
never the Western digit. And every label is shopkeeper Bengali rather than accounting
Bengali. **ধার**, not ঋণ. The shopkeeper records what happened in their own words.
Bengali is the default locale; English is the opt-in.

| | |
|---|---|
| Lines of Kotlin | **60,373** |
| Source files | **235** |
| Test files | **186** |
| Tests | **1,395** |
| Transaction types | **16** (15 surfaced across 6 groups) |
| Stack | Kotlin 2.0.21 · Jetpack Compose · Material 3 · Room 2.6.1 · SQLCipher 4.17.0 · minSdk 26 → target 35 |

Encrypted at rest with SQLCipher on the live database, encrypted backup export,
daily auto-backup, an audit log, and a recover-deleted path. The record is
defensible.

---

## II — The Forge
**[Read the brief →](briefs/The-Forge-Project-Brief.pdf)**
**A multi-day water-fasting instrument. Android. Working build, unreleased.**

Every fasting app on the store is a wellness product: streaks, confetti, push guilt,
weight graphs. This is the opposite. People attempting three-to-thirty-day water
fasts are doing something dangerous, lonely and meaningful. They do not want
encouragement. They want a witness that never lies to them, a record that survives,
and equipment that keeps them alive.

At the centre is the **Mirror** — 500 authored responses, indexed across 8 phases and
10 states, 36,744 words written for this app and nothing generated. All 80
combinations are filled. The voice is monk-cold, second person, no exclamation
marks, no emoji, no encouragement, no shame.

| | |
|---|---|
| Lines of Kotlin | **22,410** |
| Source files | **105** |
| Tests | **278** |
| Mirror responses | **500** (36,744 words · 8 phases × 10 states, none empty) |
| Badges | **32** — 17 fasting, 15 meditation, 5 names shared across both tiers |
| Meditation scripts | **10** |
| Red flags / break mechanisms | **4** / **5** |
| Electrolyte guidance bands | **4**, day-scaled |
| Refeed unlock | **72 hours** held, anchored to NICE CG32 (2006) and Mehanna, Moledina & Travis (2009) |

The safety layer is operational, not a disclaimer. Four red flags with
founder-authored response copy pinned by tests so a copy edit cannot break it. A
foreground service with a watchdog and a boot receiver, so the record survives a
restart.

---

## III — Zen PDF Studio
**[Read the brief →](briefs/Zen-PDF-Studio-Project-Brief.pdf)**
**An offline manuscript studio. Windows desktop app and single HTML file.**

Markdown-lite in, paginated Bangla-safe pages out. Eleven contrast-tuned themes, a
lane-colourising engine, and PDF export — all offline, in one file, with no server
and no network requests.

The idea: colour is a channel, not decoration. One hue means one thing, and every
text/surface pair is computed to clear 4.5:1 before it ships. Eleven lanes fire on
keywords — psychology, mechanism, evidence, body, warning, connection, action,
power, identity, voice, question — with 788 terms in English and 135 more in Bengali,
so the same manuscript colours correctly in both scripts.

| | |
|---|---|
| Keywords, Latin | **788** across 11 lanes |
| Keywords, Bengali | **135** across the same 11 lanes (**923** total) |
| Block types | **19**, each with a pass/fail rule |
| Pipeline stages | **5** — PREPARE → BLOCK-PARSE → INLINE-PARSE → COLORIZE → RENDER |
| Unit tests | **150** in 7 files |
| Vendored font families | **9** |

The stage fencing exists because markdown was being discarded whenever the colouriser
found nothing to do. Now an unchanged return is a normal outcome, not a signal to
fall back.

---

## IV — Flow of Consciousness
**[Read the brief →](briefs/Flow-of-Consciousness-Project-Brief.pdf)**
**A structured learning system. Written; corpus indexed.**

Not a course and not a chatbot prompt. One teacher that holds an entire reading list,
teaches at seven different depths, tracks what has already been understood, and
refuses to move on until the floor has actually risen.

Five intelligence domains run at once — strategic and business, capital and
financial, organisational and leadership, inner sovereignty, mythic and
manifestation — because real problems are never one question.

| | |
|---|---|
| Intelligence domains | **5** |
| Titles indexed | **54** across **10** reading areas |
| Teaching levels | **7** — Foundation through The Invisible Edge |
| Learning phases | **9** (phase 0 to phase 8), with a review every ninety days |
| Answer architecture | **13 fixed parts**, from the bottom line first to the shadow challenge |
| Commands | **10** structured doors |
| Epistemic tiers | **4** — evidence-based, psychologically useful, symbolic, unsupported |

The four-tier epistemic standard is the part that matters. The system separates what
is evidence-based, what is psychologically useful, what is symbolic, and what is
unsupported — and never quietly promotes a claim from one tier to another.

Ethics are written into the instruction rather than left to the model's mood: never
manipulate, never present speculation as fact, never replace professional advice,
never encourage dependency. Always protect the person's agency, always separate
belief from evidence, always use practice to increase responsibility rather than
escape it.

---

## V — SOVEREIGN LIBRARY
**[Read the brief →](briefs/SOVEREIGN-LIBRARY-Project-Brief.pdf)**
**A prompt-engineering law library. 28 numbered files, five pillars, an executable core.**

A library of law, not a library of tips. Everything a language model is asked to do —
reason, adopt a persona, hold context, write code, generate an image, refuse a
request — written down as law with a status line, then made runnable in Python.

| | |
|---|---|
| Numbered files | **28** (files 00–27, v3.0 Sovereign Edition) |
| Pillars | **5** — Codex (01–10), Command Layer (11–14), Sovereign Agent (15–19), Architect's Mind (20–23), Sovereign Edition (24–26) |
| Lines of Python | **1,451** across 2 modules |
| Functions / classes | **76** / **29** |
| Compiled research corpus | **801 KB**, extracted from all 28 files |

The executable part is the point. `CommandFrame` rejects an incomplete command.
`AmbiguityAudit` automates a twelve-item precision checklist. `SovereignAgent` runs
perceive, assess, decide, act, verify — with a drift check and a declaration
protocol, so an agent that has wandered from its law is caught rather than shipped.

Standard library only. No install dependencies. Platform-agnostic core.

> The unit of design is the system, not the prompt. A prompt is one turn. A system is
> every turn after it.

---

## VI — ARTHA
**[Read the brief →](briefs/ARTHA-Project-Brief.pdf)**
**A personal wealth system. The AI analyses and never executes.**

Named for the Arthashastra — Kautilya's treatise on economics and statecraft,
unsentimental and incentive-literate. At the centre is **LUX**, a finance partner who
analyses freely and never executes. Around her sit the rules, scripts and ledgers
that make her enforceable rather than merely persuasive.

> Analysis is free and reversible. Money is neither.

| | |
|---|---|
| Lines of written law | **2,260** |
| Lines of Python | **316** — standard library only, no broker connection, places no orders |
| Trade ledger | **24 columns**, one row per decision |
| Orders placed by the system | **0** |

The gates are hard: no credentials, no execution, no fraud, no manipulation. And
where a gate can only be advisory, the project says so plainly rather than pretending
a prompt is a lock — on the paste-only path the gates stay advisory, because nothing
in a prompt can veto a tool call.

The honest thesis at the centre: for a young person with limited capital, the
dominant term in the net-worth equation is income, not return. ARTHA treats the
trading account as tuition you are choosing to pay early, and is built to make sure
you pay the smallest possible version of it and survive to use the lesson.

---

## VII — CAIRN
**[Read the brief →](briefs/CAIRN-Project-Brief.pdf)**
**An astrological computation engine.** The machine is the product.

A container engine that computes a natal chart across four traditions — **Vedic,
Western, Chinese and calendar systems** — from the Swiss Ephemeris. Sidereal and
tropical zodiacs, whole-sign and Placidus houses computed in one run, 20 divisional
charts, four dasha systems, ashtakavarga, shadbala, hermetic lots, firdaria,
zodiacal releasing, BaZi. Every number is computed; none is asserted.

| | |
|---|---|
| Lines of Python | **61,716** across **205** files |
| Functions | **902** |
| Capabilities probed | **122** |
| Capabilities OK | **122** |
| Stubs · call errors · errors | **0 · 0 · 0** |
| Divisional charts | **20** (D1–D16 plus extended D5, D6, D8, D11) |
| Dasha systems | **4** — vimshottari, ashtottari, yogini, Jaimini chara |
| Ephemeris | Swiss Ephemeris, official Astrodienst `.se1` asteroid and fixed-star files |
| Spec | v1.8 **LOCKED**, 17 sections, signed reviewer #8, frozen set hashed |

The probe is the point. Every capability the engine claims is checked by an automated
gate that reports stubs, call errors and failures separately rather than folding them
into a pass.

The birth time is graded **B — family memory**. That grade is an input constraint,
not a caveat: it propagates into the refusal points and the tagging, and every timing
claim in the finished report prints `[GRADE B]` inline. The spec calls it the
artifact's honesty budget.

> An earlier ad-hoc gate reported MATCH while using a different serialisation than
> the one the spec froze. A hash check that does not reproduce the frozen method is a
> silence-as-pass defect — it cannot detect the corruption it claims to. This script
> exists so the method is written down once, in code.
> — `gates/verify_frozen.py`

---

## What is not here

Both Android apps are unreleased. The learning system is a written architecture with
its corpus indexed. The wealth system has never placed an order and never will.
Nothing here has a user, a revenue figure, or a store listing.

Every screenshot in every brief is from a device running the code. No mockups, no
placeholder screens, no invented metrics. Where a number could not be verified it was
left out rather than rounded up.

---

## How this was built

AI tooling as the instrument, production discipline as the standard. Handoff docs
that survive a session change, append-only logs, specs with change control, and
verification gates that are written down once in code so they cannot silently pass.

Second-year BBA student, no engineering degree, no funding, in Dhaka. The degree is
not the point and the budget was never the constraint.

---

MIT License · see [LICENSE](./LICENSE)
