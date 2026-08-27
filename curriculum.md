# Curriculum

Module created 2026-08-27. Two parallel tracks — see `README.md` for why.

## Bottom-up: MIT 6.041 Probability (Tsitsiklis)

Materials: `probability-mit-john-tsitsiklis/` (lectures M01–M03, recitations R04/R05/R06/R08,
assignments A3/A4, Bertsekas & Tsitsiklis textbook). Syllabus:
https://ocw.mit.edu/courses/6-041-probabilistic-systems-analysis-and-applied-probability-fall-2010/pages/syllabus/

State as of 2026-08-27: last touched no later than 2026-04-11 (repo's last commit before this
module). Assignment completion not verified — see `CLAUDE.md` § "Don't invent progress that
isn't verified." First session's job is to establish real state (open A3, check if it's blank
or solved) before planning further ahead.

Chosen over linear algebra (Strang, 23 lectures / 7 assignments, more stalled) and math stats
(UT/ITMO, largest archive, furthest in, also most stalled) because it's the least-abandoned
pile and matches what Maksim originally asked for (probability/stats, world-connected).

## Top-down: real phenomenon → math that explains it

`top-down/units/NN-slug/` — one folder per unit, each ending in a notebook/artifact plus a short
`README.md` (what the idea is, what the artifact shows, what was surprising).

1. **`01-heart-rate-distribution`** — why does resting HR / HRV vary the way it does day to day?
   Pull real data via the `mcp__coros__*` tools (available in the root KnowledgeNexus workspace,
   not in this repo directly), fit a distribution, plot it. First unit — in progress, see its
   own README once started.

Later units are chosen as-you-go, not pre-planned — that's the point of top-down. Good
candidates when unit 1 is done: a finance-investment question (does the mortgage prepayment math
actually save what it looks like it saves?), a training-load question (permutation test on
whether a program phase changed anything), a Better-Call-Saul-adjacent one (this is genuinely
fine — any real question you find yourself curious about qualifies).

## Review trigger

**Review at 8 combined sessions or 2026-09-24 (4 weeks from creation), whichever comes first.**
At that point reassess: cadence, split ratio between tracks, whether top-down's artifact
requirement is helping or becoming a tax, whether bottom-up should stay on probability or a
prior track (linear algebra, stats) deserves the resume slot instead. Update this file with the
outcome — don't let the current split become permanent by silence.
