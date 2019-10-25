Coordinates
===========
Primary and Secondary Coordinates are manually curated and verified representative genomic coordinates of the variant (Chromosome, Start, Stop, Reference base, and Variant base) for the assigned reference assembly (e.g., GRCh37)

Understanding Coordinates
-------------------------
Primary Coordinates are generated for all Variants. Secondary Coordinates are utilized for structural variants involving two loci (e.g., fusion variants). 


Curating Coordinates
--------------------

.. rubric:: Choosing representative coordinates

Although multiple genomic changes can often lead to functionally equivalent alterations (e.g., same amino acid change), CIViC uses representative coordinates to provide user-friendly variant context rather than enumerate all possible alterations that could cause the variant. When choosing a representative variant, it is preferable to use the most common or highly recurrent alteration observed. Genomic coordinates are 1-based with left-shifted normalization and include a specified reference assembly (GRCh37 preferred). Based on manually curated representative coordinates, an automated linkout to the ClinGen Allele Registry is created. This link provides additional information such as unique and referenceable identifiers for every registered variant with links to additional resources (e.g., gnomAD, ClinVar). If the required ClinGen Allele does not yet exist, the curator should create a ClinGen account and register it.

.. rubric:: Choosing a representative transcript
Multiple transcripts can often be expressed for a single gene. For this reason, a specific protein coding alteration, resulting from a genomic change, should always be expressed relative to a specific/individual transcript sequence. CIViC representative transcripts use the Ensembl archived version 75 (GRCh37), and should always include the transcript version number (i.e., ENST00000078429.1 instead of ENST00000078429). There is rarely only one correct transcript. Representative transcripts must contain the variant but are otherwise chosen based on priority criteria such as: wide use in the literature, having the longest open reading frame or most exons, containing the most common exons between transcripts, or having the widest genomic coordinates. These are consistent with Ensembl’s glossary definition of canonical.

.. rubric:: Defining variant coordinates for SNVs and small indels

Variant annotation for single nucleotide variants (SNV) and small insertion/deletions (indels) follow a 1-based coordinate system and utilize left-shifted normalization. Reference positions are indicated in green and variant positions in purple. Below, each representation is the text that would be entered into the CIViC Reference Base and Variant Base fields in the Variant Suggested Revision form.
