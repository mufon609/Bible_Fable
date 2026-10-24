# Bible_Fable

A literal translation of the Bible from the original-language consonantal text, checked against the oldest witnesses, kept as a study log in plain Markdown.

The work is a study of the text itself. It records what the Hebrew (and, when the project reaches the New Testament, the Greek) says, word by word; where the oldest witnesses disagree; where the vowel points added a thousand years later decide a reading; and where a familiar English rendering permits a reading the original does not. It does not report what any tradition, school or commentator says a verse means, and it adds no opinion.

## Two layers

- **Literal (the evidence).** One English word per Hebrew word where English allows. Verb forms, articles, number and repeated structure kept as the Hebrew has them. Supplied words in brackets.
- **Readable (the product).** The literal text with English grammar allowed to touch it and nothing else. Wherever a verse was rephrased, the literal line stands beneath it between ⸤ ⸥. Where a widely read rendering differs from the text in a way that has shaped what people take the verse to mean, an italic line says what the text has and why. No version is named on that page.

## Where things are

```
method/                       project-wide rules and method
  method.md                   witnesses, rules, parallels, weight, transliteration, open work
  judging-variants.md         how variants are judged + the running table of cases (all books)
  session-brief.md            the standing instructions as first written; CLAUDE.md is the operative copy
  session-log.md              one entry per working session (the audit trail)
belief/
  translation-to-belief.md    one row per term whose familiar English permits a reading the original does not; rows numbered across the whole project
concordance/
  hebrew.md                   every Hebrew term a finding leans on: total, fixed rendering, distribution, misfits, weight, status
  greek.md                    (created when the New Testament is reached)
books/
  old-testament/01-genesis/   one folder per book, numbered in canonical order
    log/01.md, 02.md, …       the verse log, one file per chapter
    running.md                the literal translation, chapter by chapter
    readable.md               the readable translation with ⸤ ⸥ lines and corrections
    findings.md               numbered patterns in the vocabulary, with verses and belief rows
    version-comparison.md     tables comparing KJV, NIV, ESV, NASB, NRSV, JPS at the points that differ
  new-testament/40-matthew/   (same layout, when reached)
sources/                      archived source material kept with the project; see sources/README.md
prompts/CONTINUE.md           the starting prompt for a fresh session; it finds the next chapter from the session log
CLAUDE.md                     instructions for an AI session continuing the work
```

Verse-indexed material lives under its book. Term-indexed material (the belief rows and the concordance) is project-wide, because a Hebrew word's usage is traced across every book, not one.

## Progress

| Book | Chapters done | Belief rows | Findings | Variant cases | Concordance entries |
| --- | --- | --- | --- | --- | --- |
| Genesis | 1–3 | 1–32 | 1–7 | 12 | 15 |

Begun 2026-10-09 in a Claude Doc; migrated to this repository 2026-10-24. The repository is now the only copy that is kept up to date.

## Witnesses

Masoretic Text (Leningrad), Samaritan Pentateuch, Septuagint; Syriac and Vulgate where they differ; Dead Sea Scrolls only for verses a scroll actually covers. The Hebrew does not win by default: external evidence (how many independent lines, how old) and internal evidence (the harder, shorter reading usually explains the smoother one) decide each case, and anything that rests on Masoretic vowels or accents is flagged.

## Reading the log

Each verse section gives the translation line, the pointed Hebrew, a transliteration, and a table of the words that carry weight, with a note on form and usage. A note says where else the Bible uses the word and what it means there; it does not say what that means for the verse. Conclusions are confined to the Findings, stated as patterns in the words.
