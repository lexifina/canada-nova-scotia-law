# Nova Scotia: law history in git

The law of Nova Scotia (CA-NS) as a git history: one file per provision, one commit per law on the day it took effect, and the law that made the change as the commit author. It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law).

**First build, deliberately small.** Language: English.

| Folder | Text | Versions | History |
| --- | --- | ---: | --- |
| `interpretation-act/` | Interpretation Act (R.S.N.S. 1989, c. 235) | 1 | Current consolidation dated 29 January 2026 |
| `human-rights-act/` | Human Rights Act (R.S.N.S. 1989, c. 214) | 1 | Current consolidation dated 26 January 2026 |
| `limitation-of-actions-act/` | Limitation of Actions Act (S.N.S. 2014, c. 35) | 1 | Current consolidation dated 3 February 2026 |

**Why only these.** The Office of the Legislative Counsel ([nslegislature.ca](https://nslegislature.ca/legislative-business/legislation)) publishes current consolidations only, with no past versions, and its host refused connections from the build machine. These three statutes were read from the Internet Archive's captures of 18 April 2026 and dated from the "created" date in each page's source. The amendment citations printed after each section are not kept in the text, so the history starts at these versions.

**Source:** [Office of the Legislative Counsel, Nova Scotia House of Assembly](https://nslegislature.ca/legislative-business/legislation), official, via the Internet Archive, retrieved 29 October 2026. See `LICENSE` and `REPRODUCE.md`.

Dates are the day the change took effect. This repository is not legal advice; for anything that matters, read the original.
