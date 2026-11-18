

.. _chapter05:

A control run on our own scanner, reported as it happened
=========================================================

The scanner used here matches six text-level categories: placeholders, empty or stub values, hedge-only
statements, no-progress repetition, hallucination markers, and explicit contradictions. On 2026-11-17 it
was run against a corpus of 39 local build and patch scripts and returned no findings, which is reported
as a negative result only: it says the corpus carries no text-level markers, not that the corpus is correct.

A positive control was then constructed: a two-line document carrying ``TODO:`` in one field and ``N/A`` in
another. The scanner detected the placeholder and scored 80 of 100 — and still returned ``verdict: PASS``
with exit code 0, because the verdict threshold was "score at least 80". The detector worked and the gate
did not: a document with a visible placeholder passed. That is SF-001's family, produced by our own tool.

The verdict logic was changed to fail on any hit rather than on a score threshold. Re-run on the same
document: ``quality=80/100 FAIL``, one hit listed, exit code 1. Re-run on a clean text file: \`quality=100/100
PASS\`, exit code 0. Both controls are dated and reproducible with the command in the note.

This is the reason the catalogue is worth contributing: we did not find this by reasoning about silent
failure, we found it by pointing the tool at something we knew was broken and reading the verdict.
