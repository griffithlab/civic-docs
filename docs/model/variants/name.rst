.. _variant-name:

Name
====
The Variant Name describes the specific variant being interpreted for clinical utility. Clicking on a variant name in the variant list for a gene will bring up a variant specific page with description, coordinates, alises, and associated Evidence Items. 

Understanding Variant Names
---------------------------
The variant name describes concisely some defining feature of the variant for rapid and clear identification. This will often follow HGVS-style conventions (e.g. L858R) and can also be highly generalized to categorical type (also called “bucket” type) variants such as MUTATION (for EGFR), or EXON 11 MUTATION (for KIT), which often arise during studies that pool larger numbers of patients with mutation in the given gene or gene region, in order to reach statistical conclusions. The variant name will reflect the specific biological alteration whenever possible (e.g. T790M) and also, whenever it is defined, refer to the underlying changes to the DNA sequence.

New CIViC Variants are entered into the database during the first instance of curation of evidence for the given variant. At the time of entering an Evidence Item for the new variant, the user generates the name by entering it into the Variant Name field, below the Gene Entrez Name field. Unlike Entrez name, which is drawn from a list of predetermined gene names, the variant is free text for the curator.

.. figure:: /images/figures/CIViC_screenshot-add-evidence-top.png
   :alt: Screenshot of Gene and Variant fields in the Add Evidence form

   Figure 1: Screenshot of Gene and Variant fields in the Add Evidence form
   
Curating Variant Names
----------------------
When curating this field, the most specific Variant Name described by the source should be used (e.g. KRAS G12/G13 rather than KRAS Exon 2 Mutation). The Variant Name can be very specific [e.g. VHL R176fs (c.528delG)], and in these cases HGVSor can refer to a collection of variants fitting a named category (i.e. categorical variants, sometimes called bucket variants). Examples of categorical variants include KRAS G12/G13, EGFR Exon 20 Insertion, and PIK3CA Mutation. Categorical variants are associated with multiple ClinVar entries, if applicable. Other Variant Names, including star-allele nomenclature adopted by pharmacogenetics field (e.g. DPYD*2A) are also supported.

================================ ====== ================================ ======================================================================
Variant name                     Gene   Variant type (Sequence Ontology) Demonstrates support of…
================================ ====== ================================ ======================================================================
DPYD*2A Homozygosity             DPYD   Splice Donor Variant             pharmacogenomic nomenclature
ALK Fusions                      ALK    Transcript Fusion                fusions with an unknown partner common in FISH techniques
EML4-ALK                         ALK    Transcript Fusion                specific gene fusions
EML4-ALK E6;A20                  ALK    Transcript Fusion                fusions with known specific exon boundaries / specific fusion isoforms
BCR-ABL T315I                    ABL1   Missense Variant                 specific variants in the context of other variants
CDKN2A Promoter Hypermethylation CDKN2A N/A                              epigenetic modifications
p16 Expression                   CDKN2A N/A                              expression changes
rs3814960                        CDKN2A 5 Prime UTR Exon Variant         polymorphisms
FLT3-ITD                         FLT3   Inframe Insertion                imprecise insertions with shared consequences
Exon 11 Mutation                 KIT    Coding Sequence Variant          categorical variants covering specific transcriptional boundaries
DNA Binding Domain Mutation      TP53   DNA Binding Site                 categorical variants covering specific functional boundaries
Exon 14 Skipping Mutation        MET    Exon Loss Variant                categorical variants covering specific transcriptional consequences
Loss-of-function                 BRCA   Loss of Function Variant         categorical variants covering specific functional consequences
================================ ====== ================================ ======================================================================
