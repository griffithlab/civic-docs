Summary
=======

The Variant Summary is a user-defined description of the clinical relevance of this Variant. This description should discuss the Variant’s relevance to different cancer types, patient outcomes and treatment decisions. It can be thought of as an executive summary of what information a clinician would like to know about a Variant identified in a patient tumor.

The Summary is mostly a synthesis of the Evidence Statements available for the Variant. Although individual Evidence Statements do not capture biological/mechanistic impact of Variants on gene function, such information can be summarized briefly here. Since the Summary is a synthesis of Evidence Statements in CIViC, we recommend that a Variant Summary only be created after the number of Evidence Statements created for a Variant are a reasonable reflection of the state of the literature. As a simple rule of thumb, if a variant has less than 5-10 evidence statements (or higher for some variants), the Variant is probably NOT ready for a Variant Summary yet.

.. rubric:: Aliases

Variant Aliases are used to describe alternative names for a variant. Variants may be known by more colloquial terms, amino acid positions that reference transcripts of a different length, alternative IDs, etc which can be captured here. For example, `MTHFR A222V <https://civic.genome.wustl.edu/events/genes/3672/summary/variants/258/summary#variant>`_ is also known as rs1801133, C677T, and Ala222Val.

.. rubric:: HGVS Expression

Multiple valid HGVS strings following HGVS nomenclature (see `HGVS guidelines <http://varnomen.hgvs.org/>`_) can be entered here to represent a variant at different levels (DNA/RNA/protein).

.. rubric:: ClinVar IDs

Curators can associate multiple valid ClinVar IDs with a variant which will link directly to that ClinVar entity, allowing manual associations not easily resolved by programmatic methods. For more general variants, more than one ClinVar ID may be appropriate. Enter N/A for variants that aren’t expected to have a ClinVar record (e.g., Expression). Enter NONE FOUND to indicate a search was completed and no ClinVar record was found. This allows for the possibility of future searches and updates later.

.. rubric:: Sources

Although in-line citations are not currently supported, the addition of citations used to generate the Variant Summary beyond those captured in the Evidence Statements, particularly relevant reviews, is highly encouraged with the intention of directing other users to more in-depth information about the Variant. This can be accomplished using the Sources field and entered by specifying the PubMed ID associated with the publication.

See `EGFR T790M <https://civic.genome.wustl.edu/events/genes/19/summary/variants/34/summary#variant>`_ for examples of all of the above fields.
