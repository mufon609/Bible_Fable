# Targum Onqelos (Sefaria, public-domain Aramaic text), Genesis

**What it is.** The Aramaic text of Targum Onqelos to Genesis, vocalized, in the Sefaria text version titled "Onkelos Genesis", whose source Sefaria records as http://toratemetfreeware.com/ (the Torat Emet freeware text). Fetched through Sefaria's API v3 as JSON for the whole book; the JSON is saved as returned. Other Onqelos versions on Sefaria (the Yemenite Taj vocalization from Hebrew Wikisource, CC BY-SA; Metsudah, CC BY-NC; Etheridge's 1862 English, public domain) were not archived.

**Fetched.** 2026-10-24, from
https://www.sefaria.org/api/v3/texts/Onkelos%20Genesis?version=hebrew%7COnkelos%20Genesis&return_format=text_only
(saved as `Onkelos_Genesis.sefaria-api-v3.json`). The version list with licences was read at https://www.sefaria.org/api/texts/versions/Onkelos_Genesis.

**Licence.** Public Domain, as declared in the `license` field of this version in Sefaria's API (`"license": "Public Domain"`, `"versionTitle": "Onkelos Genesis"`, `"versionSource": "http://toratemetfreeware.com/"`), which is inside the archived JSON. Sefaria licenses each text version separately and states the licence in that field. The licence rests on Sefaria's declaration; the Torat Emet site was not checked independently.

**Files (sha256).**
| File | sha256 |
| --- | --- |
| Onkelos_Genesis.sefaria-api-v3.json | a1d9804bc4da8ec743bf1140ffd7ede2c22dda11828a54e0b61183f798f18af3 |
| Genesis-plain.derived.txt | c594b2af69d98de009716c6d169ca830ec1dfda2a1cd40ad66d29851b75424e5 |

`Genesis-plain.derived.txt` is not a download. It was written here on 2026-10-24 from the JSON: `versions[0].text[chapter-1][verse-1]`, one line per verse, `Gen c:v<TAB>text`, 1533 verses, text unchanged.

**Lookup.** `grep -P "^Gen 3:15\t" Genesis-plain.derived.txt`; in the JSON, `versions[0].text` is a list of 50 chapters, each a list of verse strings.
