# Westminster Leningrad Codex (OSHB / morphhb), Genesis

**What it is.** The Westminster Leningrad Codex 4.20 as carried in the Open Scriptures Hebrew Bible (OSHB), with lemma and morphology attributes added by the Open Scriptures project. OSIS XML, pointed, with accents, one `<w>` per word; the WLC is the Groves Center's transcription of the Leningrad Codex B19A. Full-morphology release dated 2018-12-14 (see the header of `Gen.xml`).

**Fetched.** 2026-10-24, from the `master` branch of https://github.com/openscriptures/morphhb
- https://raw.githubusercontent.com/openscriptures/morphhb/master/wlc/Gen.xml
- https://raw.githubusercontent.com/openscriptures/morphhb/master/wlc/VerseMap.xml
- https://raw.githubusercontent.com/openscriptures/morphhb/master/LICENSE.md
- https://raw.githubusercontent.com/openscriptures/morphhb/master/README.md

**Licence.** The WLC text itself is in the public domain; the lemma and morphology data are Creative Commons Attribution 4.0 International (CC BY 4.0), attribution "Original work of the Open Scriptures Hebrew Bible available at https://github.com/openscriptures/morphhb". Read at https://github.com/openscriptures/morphhb/blob/master/LICENSE.md (copy in `LICENSE.md`).

**Files (sha256).**
| File | sha256 |
| --- | --- |
| Gen.xml | 0526e5c9a5fb4d907847645f954ed3d1268fa69decbd872056cedd2668d86449 |
| VerseMap.xml | 6cd269ca3dccef2cb944b9d9dd8afc950f929dab53a534f1268d23affa983163 |
| LICENSE.md | 9bf4a2890c25372e4c1dc750d550bfb4eacfbfcb63c53123b0628159370d1878 |
| README.md | 2da25acf89375558b843dab582bdf00833137baf1c8afe2b32cf09e251179999 |

**Lookup.** `Gen.xml`: `<verse osisID="Gen.3.15">` holds `<w lemma="…" morph="…">` elements; `grep -n 'osisID="Gen.3.15"' Gen.xml`. `VerseMap.xml` maps WLC verse numbering to the KJV numbering where they differ.
