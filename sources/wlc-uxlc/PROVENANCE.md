# Unicode/XML Leningrad Codex (UXLC), Genesis

**What it is.** The Unicode/XML Leningrad Codex, version UXLC 2.6, build 27.7 (18 Oct 2026), published by Tanach.us Inc. (Christopher V. Kimball), West Redding, CT. A transcription of the Leningrad Codex (B19A) with vowels and accents, forked in 2020 from the Westminster Leningrad Codex 4.20 (Groves Center, 25 Jan 2016) and since corrected against the colour images of the codex; the TEI header in `Genesis.xml` lists every change. The publisher asks that it not be represented as the WLC itself. For the unmodified WLC see `../wlc-morphhb/`.

**Fetched.** 2026-10-24, from
- https://tanach.us/Books/Genesis.xml
- https://tanach.us/Books/TanachHeader.xml
- https://tanach.us/TextFiles/Tanach.txt.zip (whole Tanach in plain text; `Genesis.txt` is `TextFiles/Genesis.txt` extracted from it unchanged)
- https://tanach.us/License.html

**Licence.** "All biblical Hebrew text, in any format, may be viewed or copied without restriction. Citation of the Tanach.us site as the source of the text is appreciated." Statement read at https://tanach.us/License.html (copy in `License.html`). Fonts and the site's other files are excluded from that grant and are not archived here. Requested citation: Unicode/XML Leningrad Codex: UXLC 2.6 (27.7), Tanach.us Inc., West Redding, CT, USA, Oct 2026.

**Files (sha256).**
| File | sha256 |
| --- | --- |
| Genesis.xml | 6c1aa3a69b57b77332d054f3ae9a01faa79b5fb1c2e7d08995a1ace82ff5a92b |
| Genesis.txt | 4d79281b5237e42d576221353b7dd667f2164743a442a1241997c913752f2fc6 |
| TanachHeader.xml | 8f50e67bb73d24a3d1a9fe673023b2c98913a924e510c6465a7387e3c214292b |
| Tanach.txt.zip | 71d958aec48ec62d11240bc5d13e7a2234ee921c1d162bdd1664f09c4688e446 |
| License.html | 21624abcf9cc16634080354616072331aefa3149bc17098953e39fd32dc8c9b7 |
| Genesis-consonantal.derived.txt | ff394292feb1c385d66f36d3f53977186d806a0b658998aca6068c65c8c0a6d1 |

`Genesis-consonantal.derived.txt` is not a download. It was made here on 2026-10-24 from `Genesis.txt` by removing every combining mark (vowels, accents, dagesh, shin/sin dots, meteg, rafe) and the joiner characters; letters, maqaf, sof pasuq and the pe/samekh paragraph marks are kept. One line per verse, `Gen c:v<TAB>text`. It is a convenience for consonantal reading; the pointed files are the source.

**Lookup.** `Genesis.xml`: `<c n="1">` holds `<v n="1">` holds one `<w>` per word (ketiv/qere as `<k>`/`<q>`). `Genesis.txt`: one verse per line, the line begins with the verse number, then `׃` and the chapter number, then the text, with chapter headings `Chapter N`. `Genesis-consonantal.derived.txt`: `grep -P "^Gen 3:15\t"`.
