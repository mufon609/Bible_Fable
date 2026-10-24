# Peshitta Old Testament (ETCBC electronic text), Genesis

**What it is.** The Syriac text of Genesis from the Electronic Peshitta Text of the Eep Talstra Centre for Bible and Computer (ETCBC, Vrije Universiteit Amsterdam), prepared by Constantijn Sikkel, Geert Jan Veldman and Willem van Peursen, obtained by OCR (program syrocr, Hannes Vlaardingerbroek) from *The Old Testament in Syriac according to the Peshitta Version*, Peshitta Institute Leiden, Brill, 1987 (the Leiden edition; for Genesis the main text of the Vetus Testamentum Syriace edition, which rests on Codex Ambrosianus). The file is the ETCBC/WIT transcription (Latin-letter transliteration of the Syriac consonants, no vowels), version `source/0.1` of the repository; `transcription.md` explains the letters and sigla; `about.md` carries the provenance and licence statements. The apparatus is not included.

**Fetched.** 2026-10-24, from the `master` branch of https://github.com/ETCBC/peshitta
- https://raw.githubusercontent.com/ETCBC/peshitta/master/source/0.1/Genesis
- https://raw.githubusercontent.com/ETCBC/peshitta/master/docs/about.md
- https://raw.githubusercontent.com/ETCBC/peshitta/master/docs/transcription.md
- https://raw.githubusercontent.com/ETCBC/peshitta/master/LICENSE

**Licence.** The text data are Creative Commons Attribution-NonCommercial 4.0 (CC BY-NC 4.0): "The plain text of the Peshitta, its conversion to Text-Fabric format, is subject to the CC-BY-NC license … you may use this data as you wish if you do not use it commercially"; commercial use requires contacting the ETCBC or Brill. Read at https://github.com/ETCBC/peshitta/blob/master/docs/about.md (copy in `about.md`). The repository `LICENSE` file (MIT) covers the conversion software only. Requested citation: W. Th. van Peursen, G. J. Veldman, C. Sikkel, H. Vlaardingerbroek and D. Roorda, ETCBC/peshitta, Zenodo, https://doi.org/10.5281/zenodo.1463675.

**Files (sha256).**
| File | sha256 |
| --- | --- |
| Genesis | e764e4061ad5781fc233626516c9c5c58fde873f12b3be6ba920ea31448a9855 |
| about.md | c40dd91e96a6099f61466701681faff1086f067547880b8cf1599578eeaae9f4 |
| transcription.md | 3a415ad5b491f3d89e7f39afd9a811ab68977718f241cede52154b67e14eecd3 |
| LICENSE | 95a3837831dba9b99db791cf6b024995b58655e0280e4d06ee1ed75540a22ac7 |

**Lookup.** Each verse is a block beginning `%verse chapter,verse` followed by the transliterated text, which may wrap over several lines: `grep -A3 "^%verse 3,15$" Genesis`. The transliteration is the ETCBC/WIT Syriac scheme, one Latin character per consonant (Gen 1:1 opens `BRCJT BR> >LH>`, that is ܒܪܫܝܬ ܒܪܐ ܐܠܗܐ, so `>` is alaph, `C` shin, `J` yodh, `T` taw); the full table is in the Text-Fabric package, module `tf.writing.transcription` (class `Transcription`, Syriac section), which `transcription.md` and the repository's `programs/tfFromWit.py` rely on. `=.`, `^`, `#` and `"` are the edition's punctuation and diacritic marks carried over from the transcription.
