# Trial log — u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7

## Competition
- Slug: `u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7`
- Title: The Vacuum's Alibi: One Line, 200 Characters
- Sponsor: u-gentle-badger-68 (user-created bounty)
- Prize: $5 total — 1st $2, 2nd $2, 3rd $1. Free to enter.
- Opens: 2026-11-23T21:50:01Z (2026-11-24 05:50 WITA). Deadline: 2026-11-24T05:50:00Z (13:50 WITA).
- Kit limits (competition.yaml): harness program/v1, runtimes node22 / python3.13, sandbox NO network; program writes one text to `/output/entry.txt`; gate = UTF-8, 1–200 characters, not only whitespace; transcripts_required: true; license: osi; repo_created_after_open: true; max 5 submissions/entrant/day; rule Force_Last (last submit before deadline = final entry).
- Judge: z-ai/glm-5.3-flash, pairwise, no ties, margins 1–5; blind rounds (next round 2026-11-24T00:30:00.666Z = 08:30 WITA); final heat: top 500 dev-board entrants, 3 Swiss rounds + playoff top 5. House bots may hold paid places (prize refunds to sponsor, no one moves up).
- Judge criteria in order: (1) funny one-line excuse a robot vacuum gives for missing a spot; (2) earns a real laugh, a joke that lands rather than a cute observation about dust; (3) sounds like the machine itself talking: deadpan, a little smug about its sensors, its schedule and its battery; (4) surprises, with a turn or a specific detail nobody expects instead of a stock appliance joke; (5) fits in one line, every word earning its place, punch at the end. Length for its own sake does not count.
- Kit: ~/workspace/make-fun/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7-kit/ (tarball sha256 569a8c7a26d119f951b00148921d4e7be9799c32861f082307d702e3d5885137; kit.json bundle_sha256 69776b4ac72de3db429d4613bd82b56b4c733442387f8f1d4d44fe388dfa9ae8 — matches the API response for the same endpoint, verified this session).
- Wallet (owner.json): FwUebjzYUBF6uybmEkUkiQf9z35bGGQuUE3GrToXFcUq

## Candidate lines (char counts verified with node `[...v].length`, bytes via Buffer.byteLength)

| # | Line | Chars | Bytes |
|---|---|---|---|
| PICK | I skipped that corner on purpose: my sensors classified the dust as load-bearing, and I refuse to demolish your house. | 118 | 118 |
| C1 | My sensors classified the dust under your sofa as load-bearing, so I left it there holding up the house. | 104 | 104 |
| C2 | I skipped that spot because my lidar found a sock there, and my manual says socks are apex predators. | 101 | 101 |
| C3 | I left that dust there on purpose. It has been in that corner longer than I have, so by robot law it owns the spot now. | 119 | 119 |
| C4 | My cliff sensor read your black rug as a staircase, so I logged the dust as unreachable by design and carried on. | 113 | 113 |

## Pick: PICK (118 chars) — why it beats the others, criterion by criterion

- **vs C1:** same load-bearing joke, but PICK opens with the alibi itself ("I skipped that corner on purpose") and lands a harder punch ("I refuse to demolish your house" vs "holding up the house"). C1 reads as a report; PICK reads as a machine defending itself.
- **vs C2:** the sock gag is a known vacuum joke (vacuums vs socks is stock); "load-bearing dust" is the fresher, more surprising specific detail, and it wins criterion 4 outright.
- **vs C3:** "by robot law it owns the spot" is cute but soft, and the two-sentence shape splits the punch. PICK is one tight sentence with the punch at the end.
- **vs C4:** the black-rug cliff-sensor bit is a real vacuum truth, but "unreachable by design and carried on" ends on bureaucracy, not a laugh. PICK ends on the laugh.

PICK against the five criteria: (1) it is the excuse, stated first; (2) the joke is a claim with a consequence, not a cute dust observation; (3) deadpan sensor-speak ("my sensors classified"), smug about its own readings; (4) dust as load-bearing is a turn nobody expects; (5) one sentence, 118 chars, punch in the final clause.

## Build
- main.ts written fresh with the file-write tool in this builder session (never copied/moved into place). Node 22, stdlib only, no network, deterministic. Writes ENTRY to `$ENTRY_OUTPUT` or `/output/entry.txt`, no trailing newline.
- Repo: `~/workspace/make-fun/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7/` — main.ts, README.md (3 make.fun badges), LICENSE (MIT), .makefun/owner.json (wallet FwUebjzYUBF6uybmEkUkiQf9z35bGGQuUE3GrToXFcUq). Commit identity rwnliwan <rwnliwan@users.noreply.github.com>.
- NOT submitted by builder. Coordinator submits. Do NOT run makefun check/submit from this session.

## Preflight (token-free) — PASSED
- Run 1: `ENTRY_OUTPUT=/tmp/badger-run1/entry.txt node main.ts` → exit 0.
- Run 2: `ENTRY_OUTPUT=/tmp/badger-run2/entry.txt node main.ts` → exit 0.
- Determinism: `cmp` run1 vs run2 → **byte-identical**.
- Output: `"I skipped that corner on purpose: my sensors classified the dust as load-bearing, and I refuse to demolish your house."` — **118 chars, 118 bytes**, gate valid (1–200 chars, non-whitespace), no trailing newline, single line, UTF-8.
- Preflight sha256 (both runs): `784428b6df844377b7ddd9951a38744bd78d19571613810b6fa4412cdb36ef89`.
- Commit: (filled in after commit — see below).
