# Clementine Vulgate (Clementine Vulgate Project / VulSearch), Genesis

**What it is.** The Latin text of the Clementine Vulgate (Editio Typica, 1598) as transcribed by the Clementine Text Project (Michael Tweedale and volunteers, 2002-2005; text maintained since), principally from the edition of A. Colunga and L. Turrado (Madrid, 1946), with Vercellone (1861) and Hetzenauer (1914) consulted for doubtful readings. `Gn.lat` is Genesis from the project's source repository at its last update (commit edc85da0, 22 Oct 2022). `data.txt` (from the 2005 "Quasimodo" release, https://sourceforge.net/projects/vulsearch/files/clemtext/source/Quasimodo.zip) names the transcriber and proof-readers of each book: Genesis was transcribed by MT and proof-read twice by MT. `plain-text-markup.README.html` is the project's description of the file format, as mirrored in https://github.com/jrichter/ClementineVulgateConverter (latin/README.html). `vulsearch-home-wayback-2024-06-20.html` is the Internet Archive capture of the project home page that carries the licence statement; the live site returned 404 for its sub-pages on the day of fetching.

**Fetched.** 2026-10-24
- https://bitbucket.org/clementinetextproject/text/raw/HEAD/Gn.lat and https://bitbucket.org/clementinetextproject/text/raw/HEAD/README.md
- https://sourceforge.net/projects/vulsearch/files/clemtext/source/Quasimodo.zip/download (only `clemtext/source/data.txt` kept)
- https://raw.githubusercontent.com/jrichter/ClementineVulgateConverter/master/latin/README.html
- http://web.archive.org/web/20240620022410id_/https://vulsearch.sourceforge.net/

**Licence.** Public domain. The project page states: "The text has been released into the public domain. Those who use it are requested to acknowledge their source, report typographical errors to the project maintainer, and make clear any modifications they make, but these are only requests that are not enforced by any licence." Read in the Wayback Machine capture of https://vulsearch.sourceforge.net/ dated 2024-06-20 (copy in `vulsearch-home-wayback-2024-06-20.html`, section "Copyright and licensing"). The VulSearch Windows program, not archived, is GPL v2.

**Files (sha256).**
| File | sha256 |
| --- | --- |
| Gn.lat | 7fe95a4cb54a2402331225da03aa1489675545586687a8d6a7b878e2db8d8c04 |
| README.md | 5979c82aef141466e3ee1f23f391071ff97c2f2201fb723ece151e24331a6398 |
| data.txt | da893fe06dea71df669742709ca164e1365195316431286137082b56b5cf3314 |
| plain-text-markup.README.html | 6805a731a46c0591f77234ed3829e910f1fed82df519eac96551ef713ff63ff3 |
| vulsearch-home-wayback-2024-06-20.html | 2e14d2158ad6a2cdb50b553477d275cb06768f5ceeeb4faaf09d1a87f122e55e |

**Lookup.** `Gn.lat` is one verse per line, `chapter:verse<SPACE>text`, Windows-1252 encoding (æ, œ as single bytes) with CRLF line ends: `grep "^3:15 " Gn.lat`, or `iconv -f CP1252 -t UTF-8 Gn.lat` to read it as UTF-8. `\` marks a paragraph break, `[ … ]` a verse-set section, `/` a line break in poetry.
