# Samaritan Pentateuch (CACCHT / DT-UCPH Text-Fabric dataset), text features

**What it is.** The consonantal text of the Samaritan Pentateuch as carried in the Text-Fabric dataset "The Samaritan Pentateuch", version 7.2.0, by Christian Canu Højgaard, Martijn Naaijer and Stefan Schorch (CACCHT project; Zenodo DOI 10.5281/zenodo.7734632). The text was supplied by the Samaritanus project (Martin-Luther-Universität Halle-Wittenberg, dir. Stefan Schorch) and transcribes MS Dublin, Chester Beatty Library 751 (Gen 1 to Deut 32:36) with MS Garizim 1 for the end of Deuteronomy; it is the base text of Schorch (ed.), *The Samaritan Pentateuch: A Critical Editio Maior* (de Gruyter, 2018-). Only the files needed to rebuild the running text are archived: node types, slot mapping, book/chapter/verse numbers, the word in Hebrew script, the transliterated word (with and without shin/sin disambiguation), and the inter-word material. Morphology, phrase and clause features are left in the repository. The dataset groups the additions after Gen 30:36 under verse 36 instead of 36a-c. Whole Pentateuch.

**Fetched.** 2026-10-24, from the `main` branch of https://github.com/DT-UCPH/sp, path `tf/7.2.0/`:
`otype.tf`, `oslots.tf`, `otext.tf`, `book.tf`, `chapter.tf`, `verse.tf`, `g_cons_utf8.tf`, `g_cons.tf`, `g_cons_raw.tf`, `trailer.tf`; plus `LICENSE` and `README.md` from the repository root (https://raw.githubusercontent.com/DT-UCPH/sp/main/…).

**Licence.** Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0). Read at https://github.com/DT-UCPH/sp/blob/main/LICENSE (copy in `LICENSE`), stated again in the `@licence` header of every `.tf` file and on the Zenodo record https://zenodo.org/records/22814616. Redistribution is permitted for non-commercial use with attribution; the authors ask that the dataset be cited as: Christian Canu Højgaard, Martijn Naaijer, & Stefan Schorch (2023), Text-Fabric Dataset of the Samaritan Pentateuch, Zenodo, https://doi.org/10.5281/zenodo.7734632, and the paper Naaijer, Højgaard, Schorch & Ehrensvärd (2024), *Research Data Journal for the Humanities and Social Sciences* 9(1), https://doi.org/10.1163/24523666-bja10051.

**Files (sha256).**
| File | sha256 |
| --- | --- |
| otype.tf | 65a248072d0dadd90ead7b1c66684045e58c4adc03e2154c126f45ffc4870c91 |
| oslots.tf | 49ed9a1caa5013f3517cb3ad9a13649189ff6d2ae11b546102019e679301a8bb |
| otext.tf | 97dfdf2331f8a9d546d108be9f73dbcd927726057aa8d66e75142316ad3ad32d |
| book.tf | c1bb969e6a10f70138503438a82299ebeed77c5e3046bdbc0fabf502a538f7b3 |
| chapter.tf | dcc90f71fe88b89eb2c56363d1eed3fdea35c1707cbedbc15897d6e2d06db5bf |
| verse.tf | baf7a1825606cc11dc9810aa29fbfe27d8e73b1c59c86153a65146ce1d583bd7 |
| g_cons_utf8.tf | 4d4d6fa3a3aa40a03d1af139eeab5c1e7537edaad909f44ee7f8fa2fc4d2be1c |
| g_cons.tf | 72b7cc5833286d283b39f6ad70125f8fa8642f007daacb8ac827e4d7c6fd630d |
| g_cons_raw.tf | 0d7db2ff7dcec405ffa058ee2986e24238b644aba77fb6dcab20b08d5d946f44 |
| trailer.tf | 63eda7bed2c3254cc20fd2580dff8acf6bdfd88a6d296d649e71a76bae94e242 |
| LICENSE | 41003d4a74749c0220e33dd415042164b5a1093ed401f36277234f772d22d3d0 |
| README.md | d1f546961eec2eb66a117412db3f82278344c21b9451d80733775dcc54accae9 |
| Genesis-plain.derived.txt | a511a92379fb58c7b4bd7f4243029885493216d1f9f2ad06696fb8d21e5cdf5c |

`Genesis-plain.derived.txt` is not a download. It was built here on 2026-10-24 from the `.tf` files above: for each Genesis verse node, the words whose slots fall in the verse, each word (`g_cons_utf8`) followed by its `trailer` (a space, or nothing where the next word is written attached). 1533 verses, 28,929 words. One line per verse, `Gen c:v<TAB>text`; shin and sin carry their dots as in the dataset.

**Lookup.** `grep -P "^Gen 4:8\t" Genesis-plain.derived.txt`. In the `.tf` files: a `.tf` file is a header, a blank line, then one value per line; a line `N<TAB>value` sets the node number, later lines count on by one. `otype.tf` gives node ranges per type (signs are the slots; words start at node 405426); `oslots.tf` gives, for each non-slot node from 399393 upward, its slot range; `book.tf`, `chapter.tf`, `verse.tf` label the book, chapter and verse nodes. Text-Fabric (`pip install text-fabric`, `use('DT-UCPH/sp')`) reads the full dataset directly.
