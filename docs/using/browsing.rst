Browsing
========

CIViC provides a series of Browse views for different entity types. These are displayed in the left menu and each provides filterable tables for one of the entities: 
`Assertions <https://civicdb.org/assertions>`_,
`Evidence <https://civicdb.org/evidence>`_, 
`Molecular Profiles <https://civicdb.org/molecular-profiles>`_,
`Genes <https://civicdb.org/genes>`_, 
`Variants <https://civicdb.org/variants>`_, 
`Variant Groups <https://civicdb.org/variant-groups>`_,
`Clinical Trials <https://civicdb.org/clinical-trials>`_,
`Diseases <https://civicdb.org/diseases>`_,
`Therapies <https://civicdb.org/therapies>`_,
`Phenotypes <https://civicdb.org/phenotypes>`_,
`Sources <https://civicdb.org/sources>`_ and
`Variant Types <https://civicdb.org/variant-types>`_.

Each table includes columns for key fields and, where appropriate, filters and sorting controls for narrowing results to entities of interest. Results may be sorted by more than one column at a time: hold the shift key while clicking on a column header to add stacked sort parameters.

Below each table a paging interface is provided to navigate through larger result sets.

Examples of the kinds of information provided in these tables are provided below.

Gene Table
----------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - Name
     - Gene Entrez Name
   * - Gene Aliases
     - A list of additional aliases (also from Entrez)
   * - Diseases
     - List of diseases associated with the Gene
   * - Therapies
     - A list of therapies (e.g. drugs) associated with the Gene
   * - Variant Count
     - A count of Variants associated with the Gene
   * - Evidence Count
     - A count of Evidence Items associated with the Gene
   * - Assertion Count
     - A count of Assertions associated with the Gene

Molecular Profiles Table
------------------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - Name
     - Name of Molecular Profile
   * - Aliases
     - A list of additional aliases associated with the Molecular Profile
   * - Entrez Genes
     - Entrez name of associated Gene(s)
   * - Variants
     - Name(s) of associated Variant(s)
   * - Diseases
     - List of diseases associated with the Molecular Profile
   * - Therapies
     - A list of therapies associated with the Molecular Profile
   * - Evidence Count
     - A count of Evidence Items associated with the Molecular Profile
   * - Assertion Count
     - A count of Assertions associated with the Molecular Profile
   * - Molecular Profile Score
     - Score summarizing the amount and strength of evidence curated for the Molecular Profile

Variant Table
-------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - Variant
     - Name of Variant
   * - Variant Aliases
     - A list of additional aliases associated with the Variant
   * - Entrez Gene
     - Entrez name of associated Gene
   * - Diseases
     - List of diseases associated with the Variant
   * - Therapies
     - A list of therapies associated with the Variant

Variant Group Table
-------------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - Name
     - Name of the Variant Group
   * - Variants
     - Names of the Variants in the Variant Group  
   * - Genes
     - List of Genes associated with the Group
   * - Variant Count
     - A count of Variants in the Group
   * - Evidence Count
     - A count of Evidence Items associated with the Group

Evidence Table
--------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - EID
     - Evidence ID of the Item
   * - Molecular Profile
     - Molecular Profile associated with the Item
   * - Diseases
     - Diseases associated with the Item
   * - Therapies
     - Therapies associated with the Item
   * - Description
     - Description of the Item
   * - EL
     - Evidence Level of the Item
   * - ET
     - Evidence Type of the Item
   * - ED
     - Evidence Direction of the Item
   * - S
     - Significance of the Item
   * - VO
     - Variant Origin of the Item
   * - R
     - Evidence Rating of the Item

Assertion Table
---------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - AID
     - Assertion ID of the Assertion
   * - Molecular Profile
     - Molecular Profile associated with the Assertion
   * - Diseases
     - Diseases associated with the Assertion
   * - Therapies
     - Therapies associated with the Assertion
   * - Summary
     - Curator's summary of the Assertion
   * - AT
     - Assertion Type
   * - AD
     - Assertion Direction
   * - CS
     - Significance
   * - CAT
     - AMP/ASCO/CAP Category
   * - Evidence Count
     - Count of Evidence Items associated with the Assertion

Source Table
------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - Type
     - Type of Source (PubMed, ASCO or ASH)
   * - Citation ID
     - PubMed or ASCO ID or ASH ID
   * - Authors
     - Authors on the Source
   * - Year
     - Year of Publication or Conference
   * - Journal
     - Name of Journal (PubMed) or meeting abstract citation (ASCO or ASH)
   * - Name
     - Title of the publication (PubMed) or meeting abstract citation (ASCO or ASH)
   * - Evidence Count
     - Count of Evidence Items associated with the Source

