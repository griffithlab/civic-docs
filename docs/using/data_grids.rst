Data Grids
==========

Tabular lists of entities, displayed in data grids, comprise a major part of the CIViC user interface. This section details the various data grids that users will encounter while using CIViC.

Evidence Grid
-------------

.. thumbnail:: /images/figures/CIViC_evidence-grid-features_v2a.png
   :alt: Screenshot of the CIViC Evidence grid
   :title: Evidence grid
   :show_caption: True

|

The evidence grid displays lists of evidence items, and provides various methods to filter subsets of evidence items of interest to the user. 

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - EID
     - Evidence ID
   * - Molecular Profile
     - Molecular Profile associated with the Evidence
   * - Disease
     - Disease associated with the Evidence
   * - Therapies
     - Therapies (e.g. drugs) associated with the Evidence
   * - IT
     - Therapy Interaction Type
   * - DESC
     - Evidence description
   * - EL
     - Evidence Level
   * - ET
     - Evidence type
   * - ED
     - Evidence direction
   * - S
     - Significance
   * - VO
     - Variant origin
   * - R
     - Evidence Rating

Assertion Grid
--------------

.. thumbnail:: /images/figures/CIViC_assertion-grid-features_v2a.png
   :alt: Screenshot of the CIViC Assertion grid
   :title: Assertion grid
   :show_caption: True

|

Assertion grids display lists of assertion items, and provide various methods to filter subsets of assertions of interest to the user.

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - AID
     - Assertion ID
   * - Molecular Profile
     - Molecular Profile associated with the Assertion
   * - Disease
     - Disease
   * - Therapies
     - Therapies associated with the item
   * - IT
     - Therapy Interaction Type
   * - SUM
     - Assertion summary
   * - AT
     - Assertion type
   * - AD
     - Assertion direction
   * - S
     - Significance
   * - CAT
     - AMP/ASCO/CAT Category
   * - Evidence Count
     - Count of evidence items associated with Assertion

Activity Feed
-------------

.. thumbnail:: /images/figures/CIViC_activity-grid_v2a.png
   :alt: Screenshot of the CIViC Activity feed
   :title: Activity feed
   :show_caption: True

|

The Activity Feed (Curation Event Timeline) displays recent curation activity. Each event includes the responsible curator/editor, action (comment, addition, revision, etc), affected entities (gene, molecular profile, evidence, etc), organization, and timestamp. The displayed events can be optionally configured to show Child Events and filtered to specific actions types, curators, or organizations.   

Other Data Grids
----------------
CIViC also provides data grids for Genes, Molecular Profiles, Variants, Variant Groups, Clinical Trials, Diseases, Therapies, Phenotypes, Variant Types, and Sources. These grids are relatively self-explanatory.
