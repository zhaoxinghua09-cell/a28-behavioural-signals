

.. _chapter04:

Which of these a machine can see, and which it cannot
=====================================================

A text-level scan can see markers of incompleteness: placeholders, stub values, hedges standing in for
a finding, "same as above" repetition, and statements that reveal the author did not have the data.

A scan cannot see SF-002, SF-008, SF-009, SF-010, SF-011, SF-012, SF-014 and SF-016, because in each of
those the artifact is well-formed and the defect lives in what the code did, not in what the text says.
Distinguishing them requires runtime evidence: the record of which items the loop actually visited, which
comparator returned which branch, which input digest was examined.

This asymmetry matters for A.2.8 directly. If behavioural signals are to be recorded, then for at least
half of these modes the record must carry execution evidence, and a text scan cannot substitute for it.
