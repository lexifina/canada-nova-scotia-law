# How this repository was made (Nova Scotia)

This file is written by the build on 2026-10-29, the day the source data was retrieved.

## Sources

| Source | Address | Retrieved | Licence |
| --- | --- | --- | --- |
| Nova Scotia Statutes, Office of the Legislative Counsel (Internet Archive copies of nslegislature.ca) | <https://nslegislature.ca/legislative-business/legislation> | 2026-10-29 | Not stated beyond the personal-use notice printed on each statute; copied by the Internet Archive. |

Every word of law in this repository comes from these sources. Lexifina reads them and records each act's dated versions, and the laws that made each change, in one corpus file. This repository is built from that file.

## What is in it

| Act | Title | Versions | Span |
| --- | --- | ---: | --- |
| `interpretation-act` | Interpretation Act (Chapter 235) | 1 | 2026-01-29 to 2026-01-29 |
| `human-rights-act` | Human Rights Act (Chapter 214) | 1 | 2026-01-26 to 2026-01-26 |
| `limitation-of-actions-act` | Limitation of Actions Act (Chapter 35) | 1 | 2026-02-03 to 2026-02-03 |

The build made 3 commits:

| Commits | Kind |
| ---: | --- |
| 3 | first version of an act |
| 0 | one law on its in-force day |
| 0 | changes no amendment note explains, credited to the publisher |

Other counts:
- 0 commits on the branch `future`: laws not yet in force on 2026-10-29.
- 0 commits dated 1 January 1970: in force before 1970, with the real day in their `In-force` trailer.
- 1 laws in the record.
- 3 tags.

## Dates

Each commit is dated at noon (America/Halifax) on the day the change took effect. The other dates, enacted and published, are trailers.

When a law gives no date of its own, the default rule applies: This record dates each consolidation by the date the Office of the Legislative Counsel gives in its HTML source; commencement dates of the statutes themselves are not recorded. https://nslegislature.ca/legislative-business/legislation

## How the history is built

`tools/build.py` turns the corpus into this history in one pass: one commit per law, on the day it took effect. The same corpus always gives the same commit hashes. `tools/check_repo.py` reads every version back from git and compares it with the corpus. `tools/on.py` shows the law as it stood on any date. The corpus format is described in `tools/SCHEMA.md`.

- Corpus: sha256 `afa945632e7364d36a2e5309c5d5a2f65cd2bdb7c7410db4354fdf1f112778c6` (102263 bytes).
- Builder blob hashes (`git hash-object`): `build.py` `6229396f41c9d7f1d6f405becfbe4097b35b82da`, `check.py` `5e112e6a33b7e93d00112e55f01fbb4fb3fdd8da`, `on.py` `644a6c0857fbcc72562032b58d57aa113fee0641`.
- Python 3.12.10; git version 2.46.0.windows.1.

## Checks

Not yet run for this build.

No second build of this corpus has been compared yet.

## Decisions made by hand

- Scope: three statutes, the Interpretation Act (R.S.N.S. 1989, c. 235), the Human Rights Act (R.S.N.S. 1989, c. 214) and the Limitation of Actions Act (S.N.S. 2014, c. 35). They were chosen as core statutes whose Internet Archive captures read cleanly; the rest of the Revised Statutes is not included.
- Each statute has one version, credited to the publisher as "oldest version available" and dated from the "created" date in the Legislative Counsel HTML (29 January, 26 January and 3 February 2026). The statutes are current consolidations; no past versions are online.
- Part headings printed in capitals are not kept. The source prints "(2" without the closing bracket in one subsection of the Interpretation Act; it is written "(2)".
- The amendment citations printed after each section (for example "2007, c. 41") are not kept in the text; section headings are kept in the first line of each file.

## What AI did and did not do

The scripts that read the sources and build this repository were written by Claude Code running Claude Opus 5.5 (`claude-opus-5-5`) under Lexifina's direction.

No model wrote, translated or corrected legal text. No model runs at build time. Every word of law in this repository comes from the official sources above.

The commit messages are written by `build.py` from the source data.

Model use at data-build time:
- none
