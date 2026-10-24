# Continue the Bible_Fable translation log

Paste this whole file as the opening message of a fresh session. It is generic: the session works out which chapter is next from the repository itself.

---

You are continuing a literal translation of the Bible kept as a study log in the Git repository at the current working directory (`Bible_Fable`, remote `github.com/mufon609/Bible_Fable`, branch `main`). This is not a coding project. The repository is the only live copy of the work; a Claude Doc the project began in is frozen and must not be edited.

## 1. Orient before writing anything

Read these files in full, in this order, and do not write a word of translation until you have:

1. `CLAUDE.md`: the operative rules, deliverables and layout.
2. `method/method.md` and `method/judging-variants.md`: the method, the witness table, the transliteration scheme, the open-work paragraph, and every variant case judged so far.
3. `method/session-log.md`: the last entry names the last chapter finished and what was left unchecked. **The next chapter is the one after it.** Say in one line which book and chapter you are taking before you begin.
4. The book folder for that book under `books/`: the last chapter file in `log/` (match its format and depth exactly), and `running.md`, `readable.md`, `findings.md`, `version-comparison.md` in full.
5. `belief/translation-to-belief.md` and `concordance/hebrew.md` in full, so new rows number on from the last row and no term is entered twice.

If the next chapter begins a new book, create its folder exactly as CLAUDE.md describes and say so.

## 2. What the project is, and is not

A study of the text itself, in two layers.

- **Literal (the evidence).** One English word per Hebrew word where English allows. Verb forms, articles, number and repeated structure kept as the Hebrew has them. A word's range is settled by the book's own usage, never by doctrine. Supplied words in brackets.
- **Readable (the product).** The literal text with English grammar allowed to touch it and nothing else. Three changes only: (A) English word order or the phrasing of a construct, (B) a copula or reciprocal the Hebrew form supplies, (C) a bracketed supplied word unbracketed. Nothing else: not a changed preposition, not a plural for a collective singular, not a smoothed stressed verb-pair, not an added article, not a synonym. Wherever a verse was rephrased, its literal wording stands beneath it between ⸤ ⸥.

Rules that bind every file:

- The text defines its own words. Record where else the Bible uses a word and what it means there; do not say what that means for the verse. Conclusions go only in `findings.md`, stated as patterns in the vocabulary, never as what the text intends.
- The Hebrew does not win by default. Check every verse against the Masoretic Text, the Samaritan Pentateuch and the Septuagint; cite the Syriac and Vulgate only where they differ. Judge a variant on external evidence (how many independent lines, how old) and internal evidence (the harder, shorter reading usually explains the smoother one). Flag every reading that rests on Masoretic vowels or accents, and say what the consonants alone permit.
- Cite a Dead Sea Scroll only for a verse it actually covers. Before you start, establish from the published scroll lists which scrolls cover the chapter and add them to the witness table in `method/method.md`. Never say a scroll "matches the MT"; say "reported as matching; plates not inspected" unless you inspected the plates.
- Extra-biblical data (cognates, Near Eastern practice) only to fix a word's meaning, never to supply a picture the Hebrew does not state.
- A parallel carries its full distribution, hits and misses, with its weight as a count. A term a finding leans on gets a concordance entry, marked complete or representative, and a representative list is not cited as settled.
- Belief rows state what the English permits. A claim about what readers believed appears only with a citation.
- No tradition's, school's or commentator's interpretation is reported. No opinion is added. No "genuinely," "honestly," or hedge language. State the form and stop.
- Never name a version, group or commentator in `readable.md`.
- Append and extend. Never rewrite, reorder or restyle what is already written. Correct an earlier entry only when the new chapter proves it wrong, and record the correction in the session log.

## 3. Before translating: write the chapter's watch list

Read the chapter in Hebrew first and list, in your working notes, before any deliverable:

- every word whose rendering rests on vowels or accents rather than consonants (names read into common nouns, homographs, pronouns whose gender the points decide, articles after prepositions);
- every place the chapter reuses a word or formula from earlier chapters, with the earlier reference;
- every variant among the witnesses that changes the English;
- every term that a familiar English rendering turns into something the Hebrew does not say;
- which scrolls cover which verses.

Work from this list so nothing on it is missed in the deliverables.

## 4. Deliverables, in this order

1. **Verse log**, `log/<cc>.md` (two-digit chapter): a `# Book N — verse log` title and one `## Book c:v` section per verse in order. Each section: the translation line in bold, the pointed Hebrew, the transliteration in italics, then a table with columns Hebrew / Transliteration / Literal / Note. Notes state form and usage only; a note may close with the KJV rendering. Transliteration: *ch* ח, *kh* soft כ, *tz* צ, *q* ק, *sh* שׁ, *s* שׂ and ס, *'* for ע and for א within a word, doubled consonants for dagesh forte, construct forms as pronounced.
2. **Running translation**, `running.md`: the chapter appended under `## Chapter N`, bold verse numbers, supplied words in brackets, wording identical to the bold lines in the verse log.
3. **Readable translation**, `readable.md`: the chapter appended under `## Chapter N`; a ⸤ *literal* ⸥ line under every rephrased verse quoting only the words that changed; an italic correction of one or two sentences, with one to four verses a reader can open, under a verse where a well-known rendering differs from the text. "It was" in "saw that it was good" is supplied without marking.
4. **Belief rows**, `belief/translation-to-belief.md`: a row for each new term whose familiar English permits a reading the Hebrew does not, numbered on from the last row. Columns: #, Hebrew term, Where, What the Hebrew says, KJV rendering, Reading the English permits, Versions that correct it. Versions compared: KJV, NIV, ESV, NASB, NRSV, JPS; no others. Quote a version only as the short phrase needed for comparison.
5. **Findings**, `findings.md`: under each existing finding, a paragraph beginning `*Ch. N adds:*` that confirms, sharpens or complicates it, ending with `*Verses:*` and `*Rows:*`. A new numbered finding only when a pattern appears that the existing ones do not cover. Update the coverage line.
6. **Concordance**, `concordance/hebrew.md`: an entry for any term a finding newly leans on: total, fixed rendering, distribution by sense with counts and verses, does not fit, weight, status. Where the chapter touches an existing representative entry, complete it.
7. **Judging variants**, `method/judging-variants.md`: a row for any variant where witnesses disagree in a way that changes the English (Case, Readings, External, Internal, Verdict).
8. **Version comparison**, `version-comparison.md`: a `### Added for c:v–v` heading, a table in the existing format (Point, Hebrew, This log, KJV, NIV, ESV, NASB, NRSV, JPS), and a short paragraph on where each version departs from the Hebrew. Give the NASB 1995 reading and mark 2020 only where you have checked it differs.

## 5. Self-audit before you commit

Check each of these and fix what fails:

- Verse-section count equals the chapter's verse count (or state which verses share a section). Running and readable have the same verses.
- Every readable verse that differs from the running text has a ⸤ ⸥ line, and every difference is one of (A), (B), (C). Compare the two files line by line.
- No version, group or commentator is named in `readable.md`.
- Every scroll citation names a verse the scroll covers, and no citation claims the plates were inspected.
- Every new belief row is numbered on from the last; every term in a new finding has a concordance entry; every concordance count that is approximate is marked representative.
- No hedge words. No statement of what the text intends.
- Nothing already written was changed except a correction you can name.
- Every readable verse keeps every Hebrew word, including "and it was," "and it shall be" and "also he" style connectives, and keeps an impersonal or passive subject impersonal; it adds no article and no "so," "there," "one" or "the" beyond a copula. If a verse cannot be made readable within (A), (B), (C), leave it literal.
- Every count you state in a note or finding ("seven times in 4:2–11") was made by listing the verses, and the list is in the note or the concordance.
- Every witness count in a readable correction ("three old translations") matches the variant table row.
- No note reports a reading as "some read," "many take," "tradition holds" or the like. State the Hebrew's form and what each witness has, and stop.
- When you overturn an earlier entry, the session log names the source checked and distinguishes the witness itself from its translation (the Samaritan Pentateuch is not the Samaritan Targum; the LXX is not a Church Father quoting it).

## 6. Hand off

Append an entry to `method/session-log.md`: date; book and chapter; verse sections, rows, entries, variant rows and comparison rows added, by number; any earlier entry corrected and why; everything left unchecked, item by item. Add any new open item to the "Open work" paragraph in `method/method.md`. Update the progress table in `README.md`.

Then commit all changes with a message naming the book and chapter and listing what was added (for example `Genesis 4: verse log, translations, rows 33–37, finding 8, 3 variants`), and push to `main`. The repository's git identity is already set; do not change it.

Finish your reply with the session-log entry text and the commit hash, so the next session and the auditor can start from them.
