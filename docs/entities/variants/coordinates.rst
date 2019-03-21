Coordinates
===========
Genomic coordinates in CIViC are a single representation of a genomic alteration that can lead to a specific variant. Multiple genomic alterations may lead to the same variant (i.e., several changes at the basepair level can lead to the same amino acid change); however, CIViC currently provides only one possible example per variant.

Understanding Coordinates
-------------------------

Curating Coordinates
--------------------
- Choose one representative variant per gene.
- Coordinates are 1-based.
- Currently we prefer variants from reference genome build 37.
- Representative transcripts are from Ensembl.

  - Include Ensembl transcript ID and transcript version (e.g.,
    'ENST00000078429.1') and the Ensembl database version (e.g., 75). Refer
    to further documentation below for guidance on how to select a
    representative transcript.

- The start is always the numerically smaller coordinate.
- Complexities can be documented in the variant comments section.
- For fusions:

  - The fusion variant is entered under only one gene. Choose the 'important'
    gene. Often, but not always, this is the 3' gene.
  - The variant name is always 5' partner - 3' partner (e.g. BCR-ABL1,
    EML4-ALK, etc.)

..rubric:: Selecting a representative transcript

A representative transcript is a single transcript model used as an
example or reference point. It is also used to define the genomic
coordinates for the variant. We present a single representative
transcript that contains the variant of interest that ideally can be
exported using the API and converted bioinformatically to desired
outputs.

Features of a representative transcript:

- There is no one 'right' answer for representative transcript.
- It must:

  - contain the variant (except in rare cases like promoter mutations).

- It should:

  - be from Ensembl archived version 75 including the transcript version
    number (i.e., ENST00000078429.1 instead of ENST00000078429).
  - be a transcript that is in our IGV reference transcript file. (see below)

- It may:

  - be the transcript with the longest ORF or most exons.
  - be the transcript that contains the 'canonical exons’ that are used in
    many transcripts.
  - be the variant that has the greatest outer coordinates.
  - be the transcript that is widely used in literature.
  - be a transcript that is compatible with interpretation/visualization in
    the literature (source paper for evidence statements).

IGV reference transcript file

- This file is a custom gene track file that can be loaded in IGV for
  review of coordinates.
- It is based on a specific version of Ensembl (v75) and contains both
  transcript IDs and transcript version numbers.
- Ensembl defined ’canonical transcripts' are highlighted with asterisks
  (***ENST00000078429.1.v75***) as a suggestion when no specific transcript
  is otherwise indicated.
- The reference transcript file can be obtained from the civic-server git
  repository here:
  Ensembl-v75_build37-hg19_UcscGenePred_CIViC-Genes.ensGene

.. rubric:: Selecting variant coordinates based on variant type

Start and stop positions are dependent upon the reference genome and the
specific isoform/transcript being used.

.. list-table::
   :widths: 50 50

   * - **Single Nucleotide Variants (SNVs)**
     -
   * - .. image:: /images/ChoosingCoordinates_SNVs.png
          
     -  - Start and stop coordinates are the same
        - Secondary coordinates do not apply
   * - **Insertions**
     -
   * - .. image:: /images/ChoosingCoordinates_Insertions.png
          
     - - Secondary coordinates do not apply
   * - **Deletions**
     -
   * - .. image:: /images/ChoosingCoordinates_Deletions.png
          
     - - Secondary coordinates do not apply
   * - **Fusions**
     -
   * - .. image:: /images/ChoosingCoordinates_Fusions.png
          
     - - Secondary coordinates correspond to the 3' partner
       - Stop1 and Start2 coordinates correspond to the edge of the nearest exon
   * - **Whole Gene alterations (altered expression, deletion, amplification)**
     -
   * - .. image:: /images/ChoosingCoordinates_Whole_Gene.png
          
     - - Secondary coordinates do not apply
       - Variant coordinates include UTRs
   * - **Gene Segments ('hotspot' regions including exons or domains)**
     -
   * - .. image:: /images/ChoosingCoordinates_Gene_Segment.png
          
     - - Secondary coordinates do not apply
