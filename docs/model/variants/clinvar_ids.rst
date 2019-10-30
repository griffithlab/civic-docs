ClinVar IDs
===========
The CIViC Variant knowledge model supports curated ClinVar IDs for each variant. ClinVar IDs must be entered individually in the Variant editing interface and may capture ClinVar IDs not described by the representative coordinates. Manual entry is required (e.g., not automatically linked based on representative coordinates) to permit entries for complex or categorical variants.

Curating ClinVar IDs
--------------------
Curators can associate multiple valid ClinVar IDs with a variant which will link directly to that ClinVar entity, allowing manual associations not easily resolved by programmatic methods. For more general variants, more than one ClinVar ID may be appropriate. Enter N/A for variants that aren’t expected to have a ClinVar record (e.g., Expression). Enter NONE FOUND to indicate a search was completed and no ClinVar record was found. This allows for the possibility of future searches and updates later.

Categorical variants are associated with multiple ClinVar entries, if applicable. In the example below, each of the ClinVar IDs links to a specific missense variant that can change KRAS at amino acid positions G12 and/or G13.

.. figure:: /images/figures/variant-screenshot-G12-G3.png
   :alt: Screenshot of Variant G12/G13

   Figure 1: Screenshot of Variant G12/G13

The CIViC Variant knowledge model supports curated ClinVar IDs for each variant. ClinVar IDs must be entered individually in the Variant editing interface and may capture ClinVar IDs not described by the representative coordinates. Manual entry is required (e.g., not automatically linked based on representative coordinates) to permit entries for complex or categorical variants and to support alternate transcripts and reference build versions.
