Data Grids
==========

Tabular lists of entities, displayed in data grids, comprise a major part of the CIViC user interface. This section details the various data grids that users will encounter while using CIViC.

Evidence Grid
-------------

.. thumbnail:: /images/figures/CIViC_evidence-grid-features_v1d.png

The evidence grid displays lists of evidence items, and provides various methods to filter subsets of evidence items of interest to the user. 

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - EID
     - Evidence ID
   * - DESC
     - Evidence description
   * - DIS
     - Disease
   * - DRUGS
     - Drugs associated with the item
   * - EL
     - Evidence Level
   * - ET
     - Evidence type
   * - ED
     - Evidence direction
   * - CS
     - Clinical significance
   * - VO
     - Variant origin
   * - ER
     - Evidence Rating

Assertion Grid
--------------

.. thumbnail:: /images/figures/CIViC_assertion-grid-features_v1a.png

Assertion grids display lists of assertion items, and provide various methods to filter subsets of assertions of interest to the user.

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - AID
     - Assertion ID
   * - Summary
     - Assertion summary
   * - Disease
     - Disease
   * - Drugs
     - Drugs associated with the item
   * - AT
     - Assertion type
   * - AD
     - Assertion direction
   * - CS
     - Clinical significance
   * - Evidence
     - Count of evidence items associated with Assertion

Activity Feed
-------------

.. thumbnail:: /images/figures/CIViC_activity-grid_v2a.png

The Activity Feed (Curation Event Timeline) displays recent curation activity. Each event includes the responsible curator/editor, action (comment, addition, revision, etc), affected entities (gene, molecular profile, evidence, etc), organization, and timestamp. The displayed events can be optionally configured to show Child Events and filtered to specific actions types, curators, or organizations.   

Other Data Grids
----------------
CIViC also provides data grids for Genes, Molecular Profiles, Variants, Variant Groups, Clinical Trials, Diseases, Drugs, Phenotypes, Variant Types, and Sources. These grids are relatively self-explanatory.
