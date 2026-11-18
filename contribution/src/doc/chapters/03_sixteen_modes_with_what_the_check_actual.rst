

.. _chapter03:

Sixteen modes, with what the check actually observed
====================================================

Each entry states the observable situation and the artifact-level question that exposes it. The identifiers
are catalogue references, not clause numbers.

.. list-table::
    :header-rows: 1

    * - ID
      - Mode
      - What the check actually observed
    * - SF-001
      - Zero items, pass
      - An empty set: the loop ran over nothing and the absence of failures was reported as success
    * - SF-002
      - Early return treated as skip
      - A branch that exits before validating, recorded as though validation had been waived deliberately
    * - SF-003
      - Swallowed exception
      - An error caught and discarded; the run continued with the value that caused it
    * - SF-004
      - Sentinel value
      - A placeholder standing in for a measurement, counted as data
    * - SF-005
      - Neutral marker not counted
      - A non-committal result ("unknown", "unclassified") excluded from the tally and therefore invisible in the total
    * - SF-006
      - Undeclared not checked
      - A field absent from the record, treated as satisfying the rule rather than as missing
    * - SF-007
      - Empty value is silent
      - An empty string or null accepted by a comparison that never distinguished empty from valid
    * - SF-008
      - Loading artifact as evidence
      - The act of loading a file counted as evidence that its content was examined
    * - SF-009
      - Exposure counted as usage
      - A capability being reachable counted as a capability being exercised
    * - SF-010
      - Local green, remote red
      - A check run against a local copy, reported as a result about the deployed system
    * - SF-011
      - Always-green oracle
      - A comparator whose branches both return success
    * - SF-012
      - Misattributed failure
      - A failure attributed to the wrong component, so the fix lands somewhere else
    * - SF-013
      - Stale copy contaminates the check
      - A cached or superseded input examined in place of the current one
    * - SF-014
      - Zombie process looks alive
      - A process that answers a liveness probe but no longer performs its function
    * - SF-015
      - Stale reference rot
      - A citation that resolved when written and no longer resolves, still carried as support
    * - SF-016
      - Swallowed failure returned
      - A failure converted into a default return value that the caller reads as success


The list is not offered as complete. It is offered as a set of cases that a group writing conformance
criteria can use as negative controls, because each one produces a passing report that a reviewer can
reproduce.
