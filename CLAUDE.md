# CLAUDE.md

This is not a coding project. It is a literal translation of the Bible from the original-language consonantal text, kept as a study log in Markdown. The repository is the source of truth; the Claude Doc the work began in (https://claude.ai/artifact/9LbrXU1bK7bpJjq4Q52QRQ) is frozen as of 2026-10-24 and is not updated.

## Start of every session

If the session was opened with `prompts/CONTINUE.md`, follow it; it repeats and expands these steps.

1. Read `method/method.md`, `method/judging-variants.md` and the last entry in `method/session-log.md`.
2. Read the book folder you are continuing: the last chapter in `log/`, and `running.md`, `readable.md`, `findings.md`, `version-comparison.md`.
3. Read `belief/translation-to-belief.md` and `concordance/hebrew.md` so new rows number on correctly and existing entries are not duplicated.
4. Match the existing format and depth exactly. Do not restyle.

## What the project is

A study of the text itself, in two layers: a literal text (the evidence) and a readable text (the product), with a one-line correction under any verse where a well-known reading differs from the original. Work from the consonantal text; check every verse against the Masoretic Text, Samaritan Pentateuch and Septuagint; cite the Syriac and Vulgate only where they differ; cite a Dead Sea Scroll only for a verse it actually covers (the witness table in `method/method.md` lists Genesis scrolls by verse). For the New Testament, the same discipline applies to the Greek witnesses; the method file will be extended when the project reaches them.

No tradition's, school's or commentator's interpretation is reported, and no opinion is added. State the form and stop.

## Scope

The project compares the texts that shaped what English readers believe, and nothing else. Ancient witnesses: the Masoretic Text (Leningrad), the Samaritan Pentateuch, and the Septuagint in Rahlfs–Hanhart; the Vulgate and the Peshitta only where they differ from the Hebrew, and only in the critical edition (Clementine/Weber–Gryson; Leiden); a Dead Sea Scroll only for a verse it covers. English versions: KJV, NIV, ESV, NASB, NRSV, JPS. No Targums, no Jubilees, no Josephus, no Church Fathers, no modern commentators, and no single manuscript cited as if it were a tradition (a scroll covering the verse is the one exception). If a reading needs a text outside this list, it is out of scope and is not recorded. Added 2026-10-24 after an audit found Onqelos, the Samaritan Targum, Jubilees, Josephus and Codex Alexandrinus cited in ch. 2–6; those citations are marked or removed and the session log says which.

## The rules (full text in method/method.md)

1. One English word per Hebrew word where English allows; verb forms, articles, number and repeated structure kept as the Hebrew has them; a word's range settled by the book's own usage, never by doctrine.
2. Variants: the Hebrew does not win by default. External evidence (independent lines, age) and internal evidence (the harder, shorter reading usually explains the smoother one). Flag anything that rests on Masoretic vowels or accents.
3. Parallels recorded, conclusions confined to Findings. A note says where else the Bible uses the word and what it means there; it does not say what that means for the verse.
4. Extra-biblical data (cognates, Near Eastern practice) only to fix a word's meaning, never to supply a picture.
5. A parallel carries its full distribution, hits and misses, and its weight as a count. A new term the Findings lean on gets a Concordance entry.
6. Belief table: state what the English permits; a claim about what readers believed only with a citation.
7. Readable text: three permitted changes only, (A) English word order or phrasing of a construct, (B) a copula or reciprocal the Hebrew form supplies, (C) a bracketed supplied word unbracketed. A correction only where the KJV rendering produced a reading the Hebrew does not permit, or where a modern rendering shared by four or more of the six versions does; any other difference belongs in the belief table, not under the verse. One or two sentences, with one to four verses a reader can open. "It was" in "saw that it was good" is supplied without marking.
8. Transliteration: *ch* ח, *kh* soft כ, *tz* צ, *q* ק, *sh* שׁ, *s* שׂ and ס; *'* for ע and for א within a word, unmarked at the start of a word; doubled consonants for dagesh forte; construct forms as pronounced.
9. Sources: every reading cited names the edition or site it was taken from, and that source is entered in `sources/README.md` the first time it is used; the register is the scope list, and a source that is not one of the admitted texts (see Scope) is not added to it. Within each witness, prefer the critical edition and name the copy; within the English versions, name the printing. A scroll is cited from its published plate or edition. An English rendering placed in a comparison table or belief row is checked against a copy of that version, not recalled, and the copy is named. A reading taken from a site rather than an edition says so in the note.

## Per-chapter deliverables, in this order

1. `books/<testament>/<nn-book>/log/<cc>.md`: one section per verse, in order. Format: `## Book c:v`, a bold translation line, the pointed Hebrew, an italic transliteration, then a table with columns Hebrew / Transliteration / Literal / Note. Notes state form and usage only; a note may end with the KJV rendering.
2. `running.md`: the chapter appended under `## Chapter N`, bold verse numbers, supplied words in brackets.
3. `readable.md`: the chapter appended, with a ⸤ *literal* ⸥ line under every rephrased verse and italic corrections. Never name a version, group or commentator in this file.
4. `belief/translation-to-belief.md`: a row for each new term that qualifies, numbered on from the last row. Columns: #, Hebrew term, Where, What the Hebrew says, KJV rendering, Reading the English permits, Versions that correct it. Versions compared: KJV, NIV, ESV, NASB, NRSV, JPS; no others.
5. `findings.md`: confirm, sharpen or complicate the existing findings by appending a "*Ch. N adds:*" paragraph under each; add a new numbered finding only when a pattern appears that the existing ones do not cover. Update the coverage line. A finding is a pattern in the words, never a conclusion about what the text intends.
6. `concordance/hebrew.md`: an entry for any term a finding newly leans on (total, fixed rendering, distribution by sense with counts and verses, does not fit, weight, status). Mark lists complete or representative; representative lists are to be checked against a full concordance before a finding cites them as settled.
7. `method/judging-variants.md`: a row for any variant where witnesses disagree in a way that changes the English (Case, Readings, External, Internal, Verdict).
8. `version-comparison.md`: a `### Added for c:v–v` table in the existing format (Point, Hebrew, This log, KJV, NIV, ESV, NASB, NRSV, JPS) followed by a short paragraph on where each version departs.

## Do not

- Cite a text outside the Scope list, or add one to the sources register.
- Rewrite, reorder or restyle anything already written. Append and extend. Correct an earlier entry only when the new chapter proves it wrong, and say so in the session log.
- Report what any tradition teaches a verse means.
- Name a version, group or commentator in `readable.md`.
- Use "genuinely," "honestly," or hedge language.
- Cite a Dead Sea Scroll for a verse it does not cover, or state that a scroll agrees with the MT without saying whether the plates were inspected.
- Add a finding that is a conclusion about intent rather than a pattern in the vocabulary.
- Put quoted modern-version text beyond the short phrase needed for comparison.

## End of every session

Append an entry to `method/session-log.md`: date, chapter covered, rows and entries added by number, any earlier entry corrected and why, anything left unchecked. The entry includes a "Sources consulted:" line naming the editions or sites opened. Add any new open item to the "Open work" paragraph in `method/method.md`. Then commit with a message naming the book and chapter (for example `Genesis 4: verse log, translations, rows 33–37`) and push.

## Layout for new books

One folder per book under `books/old-testament/` or `books/new-testament/`, named `<nn>-<book>` in canonical order (`01-genesis`, `02-exodus`, … `40-matthew`, … `66-revelation`), each with `log/`, `running.md`, `readable.md`, `findings.md`, `version-comparison.md`. Belief rows and the concordance stay project-wide; the concordance gains `greek.md` when the New Testament is reached. Archived source material goes in `sources/` with a line in `sources/README.md` naming its origin and licence.

## Writing style

Plain and specific. Short sentences. Facts, forms and counts; no adjectives of approval, no interpretation. Hebrew in pointed script in the Hebrew column, transliteration in italics in its own line, English verse references in the form `Gen 3:15`, `1 Kgs 2:37`.
