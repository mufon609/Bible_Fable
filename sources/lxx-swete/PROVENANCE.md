# Septuagint, Swete's edition (First1KGreek transcription via nathans/lxx-swete), Genesis

**What it is.** *The Old Testament in Greek According to the Septuagint*, edited by Henry Barclay Swete (Cambridge University Press; vol. I, Genesis to IV Kings, 4th ed. 1909). Swete prints Codex Vaticanus (B) with its gaps filled from Alexandrinus or Sinaiticus; the apparatus is not transcribed. This copy is the word-per-line text produced by Nathan Smith's `lxx-swete` repository from the Open Greek and Latin Project's First1KGreek transcription (TLG 0527), rebased to the First1KGreek commit eb81494731fd632f582c4b94634127bdbd596b43 of 23 Jan 2025. First1KGreek describes its text as machine-corrected OCR; the proofread Sollupulo transcription in `../lxx-swete-sollupulo/` is the check on it. Not Rahlfs.

**Fetched.** 2026-10-24, from the `master` branch of https://github.com/nathans/lxx-swete
- https://raw.githubusercontent.com/nathans/lxx-swete/master/data/01.Genesis.txt
- https://raw.githubusercontent.com/nathans/lxx-swete/master/README.md
- https://raw.githubusercontent.com/nathans/lxx-swete/master/COPYING-Code
- https://raw.githubusercontent.com/OpenGreekAndLatin/First1KGreek/master/license.md (the upstream licence, saved as `First1KGreek-license.md`)

**Licence.** The Greek text and its annotations are Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0), as stated in the `lxx-swete` README (copy in `README.md`) and by the First1KGreek repository (GitHub licence field CC-BY-SA-4.0; full text in `First1KGreek-license.md`, read at https://github.com/OpenGreekAndLatin/First1KGreek/blob/master/license.md). The build scripts, not archived, are MIT (`COPYING-Code`). Swete's 1909 edition is itself out of copyright.

**Files (sha256).**
| File | sha256 |
| --- | --- |
| 01.Genesis.txt | b5abf507f757de3c96f3e44944515dba46d6e5b9edd8e653d7ce6096588c5ce6 |
| README.md | ca5869019f542d01ae0ecd9e0381ddbfe6bd0a6c14ed7edf52b8d0973634c325 |
| COPYING-Code | ae21033db0eb664b0be84881d8993a32357e0cf66e6961a37bba0844b8e695d2 |
| First1KGreek-license.md | ccf0e8ce183761bf82700126cc45a4e907b2cede024e65e3fef5c2338b9b7063 |

**Lookup.** One word per line, `book.chapter.verse<SPACE>word` with book 1 = Genesis: `grep "^1\.3\.15 " 01.Genesis.txt` prints Gen 3:15 word by word.
