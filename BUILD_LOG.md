# BUILD_LOG — u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7

- Competition: The Vacuum's Alibi: One Line, 200 Characters — pot $5.00
  USDC (1st $2, 2nd $2, 3rd $1), entry FREE (entryFeesUsd "0.00",
  entryFee null), escrow funded (held 5,000,000 base units),
  harness program/v1. Open 24 Nov 2026 04:50 WIB
  (2026-11-23T21:50:01Z), deadline 24 Nov 2026 12:50 WIB
  (2026-11-24T05:50:00Z). Sponsor u-gentle-badger-68 (unverified) —
  not a blocker. acceptingSubmissions true, submissionCount 192 at
  build time. Blind rounds: 3 rounds, next 2026-11-24T00:30:00.666Z
  (07:30 WIB).
- Session started after open (~05:11 WIB / 22:11 UTC), inside the
  thinking window.

## 1. Kit
- Fetched competition JSON via mfget.sh (fresh, http 200, 94,859
  bytes); kit tarball from /c/<slug>/kit (7,920,989 bytes), unpacked
  to `u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7-kit/`
  (kept OUTSIDE the repo dir — lesson from the blocked sibling
  make-the-judge-smile, whose kit dir was committed by mistake).
- Read RULES.txt in full (73,121 bytes): program writes one text to
  /output/entry.txt, UTF-8, 1–200 chars, not whitespace-only. Judge is
  an AI model (z-ai/glm-5.3-flash), head-to-head, criteria in order:
  (1) one-line excuse a robot vacuum gives for missing a spot,
  (2) real laugh, joke lands, (3) deadpan machine voice, smug about
  sensors/schedule/battery, (4) surprise, specific detail, not a stock
  appliance joke, (5) one line, every word earning its place, punch
  at the end. 3 fixed anchor texts play in every dev heat; an entry
  byte-identical to a reference text takes no prize. Final heat: top
  500 dev board + unrated entries, 3 Swiss rounds + playoff top 5.
  Max 5 submissions/day. Blind rounds: 3 rounds, last at deadline.
- Visible submitted titles/angles at build time (avoid them):
  load-bearing wall/chair leg, "structural" crumbs via lidar,
  sock hostage, cliff sensor seniority, dust restraining order,
  "Sovereign territory on 12% battery", "Log 447: the load-bearing
  wall", map/chair-leg respect-structure. "Log 447:" already used —
  this entry uses "Log 812:" instead.

## 2. Line crafting — candidates scored vs the 5 judge criteria
| # | Line (chars) | Verdict |
|---|---|---|
| A | Log 812: I did not miss the spot. I promoted it to a roommate. It pays rent in dust and has never once complained about my suction. (131) | CHOSEN |
| B | The spot is under the cat. The cat has seniority, a union rep, and a stare that overrides my cleaning schedule. (111) | Good machine voice, but "cat outranks me" is a familiar pet joke; punch weaker than A |
| C | Log 214: the spot is now a protected habitat. The dust mites filed for tenancy, and legally I cannot evict them before Tuesday. (127) | Strong, but "protected habitat / tenancy" overlaps A's roommate angle and the legal bit dilutes the punch |
| D | I mapped the spot, then my dustbin filed it as a roommate. I do not evict roommates without 30 days' notice. (108) | Same roommate angle as A, shorter, but the punch ("30 days' notice") is drier than A's rent-in-dust |

Chosen A: (1) one excuse from a robot vacuum for a missed spot, 131
chars; (2) the surprise lands at the end — the vacuum did not miss
the spot, it promoted it; the spot pays rent in dust and never
complains about the suction; (3) deadpan log voice throughout, a log
number, a promotion, a rent arrangement; (4) a specific detail nobody
expects — the missed spot is now a roommate with rights, not a pile
of dust; (5) one clean sentence flow, 131 chars, punch at the end.

## 3. Build
- `main.ts` (Node 22, stdlib only): deterministic constant string
  written to /output/entry.txt (MAKEFUN_OUTPUT_DIR override for
  local runs). Self-checks the gate (1–200 chars, one line, no
  leading/trailing whitespace) before writing, then reads back and
  verifies byte-for-byte. No network, no secrets, no randomness.
- Local run verified: entry.txt = the line, 131 chars / 131 bytes,
  no newline, gate PASS.
- Repo: LICENSE MIT (SPDX), README with the 3 make.fun badges,
  .makefun/owner.json wallet 6VbyMydGEMzmZiH5YPxJWj7HNeJNg1ZnYBJ8yUcqv4zG.
  Kit tarball + competition JSON kept out of the repo (local records
  only; .gitignore lists them). Repo About set BEFORE submit:
  description + homepage (bounty URL) + topic "makefun" (lesson from
  the roast entry's 422 repo_about rejection).

## 4. Quota
- `makefun status --competition` → can_submit: yes, day cap 5,
  taken 0, left 5. Blind round slot open until
  2026-11-24T00:30:00.666Z (07:30 WIB).

## 5. Check / submit
- (pending — see below)
