

.. _chapter01:

Summary
=======

A behavioural trust signal is only worth recording if the check that produced it can fail. This contribution
collects sixteen failure modes in which a validation step reports success while nothing has been validated,
states for each what the check actually observed, and separates the modes that a text-level pattern scan can
catch from the modes that require runtime evidence. It closes with a control run on our own scanner, in which
the scanner first passed a document that carried a visible placeholder and then failed it once the verdict
logic was made fail-closed.
