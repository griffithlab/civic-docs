Variants Overview
=================

CIViC variants are usually genomic alterations, including single
nucleotide variants (SNVs), insertion/deletion events (indels), copy
number alterations (CNV's such as amplification or deletion), structural
variants (SVs such as translocations and inversions), and other events
that differ from the "normal" genome. In some cases a CIViC variant may
represent events of the transcriptome or proteome. For example,
'expression' or 'over-expression' is a valid variant. Regardless of the
variant, it must have an Predictive, Prognostic, Predisposing or
Diagnostic clinical relevance to be entered in CIViC. New curators should
generally avoid proposing new variants that are unlike any already in
CIViC.

**Variant Attributes**

.. list-table::
   :widths: 20 70 10
   :header-rows: 1

   * - Attribute
     - Description
     - Source
   * - Name
     - Description of the type of variant (e.g., 'V600E', 'BCR-ABL
       fusion', 'Loss-of-function', 'Exon 12 mutations'). Should be as
       specific and short as possible (i.e., specific amino acid changes).
     - CIViC
   * - Summary
     - User-defined summary of the clinical relevance of this
       Variant.
     - CIViC
   * - Alias
     - Alternative names for this Variant. May be more verbose (e.g.,
       'Val600Glu') versions, dbSNP IDs or alternative nomenclature used in
       the literature.
     - CIViC
   * - HGVS Expression
     - User-defined HGVS strings following HGVS
       nomenclature that represent this Variant at the DNA, RNA or protein
       level.
     - CIViC
   * - ClinVar ID
     - User-defined ClinVar ID referencing this Variant which
       will be linked directly to ClinVar. A value of "None Specified"
       indicates that the variant has not been evaluated for a ClinVar ID.
       A value of "None Found" indicates that an attempt was made to find a
       matching ClinVar Entry, but none exists. A value of "N/A" indicates
       that a ClinVar record is not applicable to the variant (e.g.
       "Overexpression" variants).
     - CIViC (ClinVar)
   * - Sources
     - A list of PubMed IDs referring to evidence supporting
       statements made in the Gene's description. Source descriptions (e.g.
       'Weisberg et al., 2007, Nat. Rev. Cancer') are pulled from the
       PubMed database at the time of submission, and are not editable.
     - CIViC (PubMed)
   * - CIViC Actionability Score
     - The CIViC Actionability Score assesses the
       quality and quantity of evidence submitted for each variant. The
       CIViC Actionability Score is calculated by adding all Evidence Item
       Scores for each variant. The Evidence Item Score is calculated by
       multiplying the evidence level (A=10 points, B=5 points, C=3 points,
       D=1 point, E=0.25 points) by the trust rating (Each Star = 1 point).
     - CIViC
   * - Variant Type(s)
     - One or more terms from the Sequence Ontology that
       describes the type of variant. Should be the most descriptive term
       applicable on a given branch (e.g., 'Conservative Missense Variant',
       'Stop Gained', 'Transcript Fusion').
     - CIViC (Sequence Ontology)
   * - **Primary Coordinates**
     -
     -
   * - Reference Build
     - NCBI or GRC human reference assembly version.
     - CIViC
   * - Chromosome
     - Name of the chromosome in which the variant occurs.
     - CIViC
   * - Start, Stop
     - Start and stop positions of the variant (1-based
       genome coordinate). Start must be less than or equal to stop.
     - CIViC
   * - Reference & Variant Bases
     - The nucleotide base of the reference and variant
       allele (e.g. 'C', 'A').
     - CIViC
   * - Representative Transcript
     - Ensembl transcript ID and version number
       for a known transcript of the gene that contains the variant (e.g.
       'ENST00000263967.3').
     - CIViC
   * - **Secondary Coordinates**
     -
     -
   * - Same as Primary
     - For fusion variants, the secondary coordinates are
       used to specify the 3' partner of the fusion gene.
     - CIViC
   * - **MyVariant.Info**
     -
     -
   * - MyVariant Info
     - Data retrieved from MyVariant.Info using the
       curated Primary Coordinates (chromosome, start, stop, reference
       base, variant base) described above as the query. Includes external
       IDs and links whenever possible with additional data displayed by
       clicking the "Details" button.
     - MyVariant.Info
