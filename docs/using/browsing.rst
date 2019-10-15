Browsing
========

CIViC provides a `Browse section <https://civicdb.org/browse/genes>`_, organized into tabs, comprised of filterable tables for each of its entities: Genes, Variants, Variant Groups, Evidence, Assertions and Sources.

Each table includes columns for key fields and, where appropriate, filters and sorting controls for narrowing results to entities of interest. Results may be sorted by more than one column at a time: hold the shift key while clicking on a column header to add stack sort parameters.

Below each table a paging interface is provided to navigate through larger result sets.

Gene Table
--------------

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
   * - Drugs
     - A list of drugs associated with the Gene
   * - Variants
     - A count of Variants associated with the Gene
   * - Evidence
     - A count of Evidence Items associated with the Gene
   * - Assertions
     - A count of Assertions associated with the Gene

Variant Table
-----------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - Variant
     - Name of Variant
   * - Entrez Gene
     - Entrez name of associated Gene
   * - Diseases
     - List of diseases associated with the Variant
   * - Drugs
     - A list of drugs associated with the Variant
   * - Evidence
     - A count of Evidence Items associated with the Variant
   * - Assertions
     - A count of Assertions associated with the Variant
   * - Evidence Score
     - CIViC's Evidence Score for the Variant

Variant Group Table
-----------------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - Name
     - Name of the Variant Group
   * - Count
     - Number of Variants in the Group
   * - Genes
     - List of Genes associated with the Group
   * - Evidence
     - A count of Evidence Items associated with the Group

Evidence Table
-----------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - EID
     - Evidence ID of the Item
   * - Gene
     - Gene associated with the Item
   * - Variant
     - Variant associated with the Item
   * - Description
     - Description of the Item
   * - Diseases
     - Diseases associated with the Item
   * - Drugs
     - Drugs associated with the Item
   * - EL
     - Evidence Level of the Item
   * - ET
     - Evidence Type of the Item
   * - ED
     - Evidence Direction of the Item
   * - CS
     - Clinical Significance of the Item
   * - VO
     - Variant Origin of the Item
   * - ER
     - Evidence Rating of the Item

Assertion Table
-------------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - AID
     - Assertion ID of the Assertion
   * - Gene
     - Gene associated with the Assertion
   * - Variant
     - Variant associated with the Assertion
   * - Summary
     - Curator's summary of the Assertion
   * - Diseases
     - Diseases associated with the Assertion
   * - Drugs
     - Drugs associated with the Assertion
   * - AT
     - Assertion Type
   * - AD
     - Assertion Direction
   * - AS
     - Clinical Significance
   * - Evidence
     - Count of Evidence Items associated with the Assertion

Source Table
----------------

.. list-table::
   :widths: 25  75
   :header-rows: 1

   * - Column
     - Description
   * - Type
     - Type of Source (ASCO or PubMed)
   * - Citation ID
     - PubMed or ASCO ID
   * - Authors
     - Authors on the Source
   * - Year
     - Year of Publication or Conference
   * - Journal
     - Name of Journal (PubMed) or Citation (ASCO)
   * - Name
     - Title of the publication (PubMed) or abstract (ASCO)
   * - Evidence
     - Count of Evidence Items associated with the Source
