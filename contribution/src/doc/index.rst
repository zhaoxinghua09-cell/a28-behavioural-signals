.. _chapter-overview:

Title
=====

Behavioural Trust Signals: Sixteen Ways a Check Passes While Nothing Is Checked

Abstract
--------

A behavioural trust signal is worth recording only if the check that produced it could fail. This contribution collects sixteen silent-failure modes, states for each what the check actually observed, and separates those a text-level scan can catch from those that require runtime evidence. It closes with a dated control run on our own scanner, in which the scanner first passed a document carrying a visible placeholder and then failed it once the verdict logic was made fail-closed.

History
-------

.. list-table::
    :header-rows: 1
    :widths: 12 34 14 12 22

    * - Version
      - Document
      - Date
      - Focus Group
      - Working Group
    * - 0.1.0
      - Behavioural Trust Signals: Sixteen Ways a Check Passes While...
      - 2026-11-10
      - TIDA
      - WG1 (CDRA)

Authors
-------

.. list-table::
    :header-rows: 1
    :widths: 30 40 30

    * - Name
      - Affiliation
      - Contact
    * - Steven Zhao
      - Independent expert (individual participant), ORCID 0009-0001-0512-1237
      - zhaoxinghua06@126.com

Keywords
--------

behavioural trust signals, silent failure, negative controls, conformance, benchmarks, agentic AI

Foreword
--------

This contribution is offered to the ITU-T Focus Group on Trust and Identity for
Humans and Agentic AI as input to its work. It states a position and proposes
interfaces; it does not assert consensus, and it does not claim that any element
has been adopted. Where the text refers to published material, that material is
identified in the body so that a reader can check the source rather than take the
summary on trust. Participation follows the ITU-T and FG-TIDA participation,
conduct and intellectual property rights rules.

This note is one of a set. The lifecycle framework of FG-TIDA-WG1-004
states the stages at which behavioural signals are read, and
FG-TIDA-WG2-006 states the evidence axis those signals belong to: a check
that cannot fail produces a signal with no evidence behind it.

DataTracker record: FG-TIDA-WG1-005..

.. toctree::
    :maxdepth: 3
    :numbered:
    :hidden:

    chapters/01_summary
    chapters/02_what_a_2_8_asks_and_what_this_note_answe
    chapters/03_sixteen_modes_with_what_the_check_actual
    chapters/04_which_of_these_a_machine_can_see_and_whi
    chapters/05_a_control_run_on_our_own_scanner_reporte
    chapters/06_mapping_to_the_terms_of_reference
    chapters/07_request_to_the_focus_group
    chapters/08_limits_and_what_is_not_claimed
