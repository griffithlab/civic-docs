.. _variant-name:

Name
====
The **Variant Name** describes the specific variant being interpreted for clinical utility. Selecting a Variant Name in the Variant list for a Gene will bring up a Variant specific page with a description, aliases, HGVS expressions, ClinVar identifiers, Variant Type(s) and associated Evidence Items. 
 

Understanding Variant Names
---------------------------
The Variant Name concisely describes a defining feature of the variant for rapid and clear identification. The Variant Name should be the most specific description of the variant that the underlying sources allow. However, names can be generalized to categorical variants (also called “bucket” variants) such as Mutation or Exon 11 Mutation, if more granular detail is not provided. Categorical variants often arise during studies that pool larger numbers of patients with unspecified mutations in a given gene or gene region, in order to reach statistical conclusions. Variant Names often follow HGVS-like conventions (e.g. L858R). 


Adding New Variant Names
---------------------------
New CIViC Variant Names are entered into the database at the first instance of curation of evidence for the given variant. At the time of entering an Evidence Item for a new variant, the user generates the name by entering it into the Variant Name field, below the Gene Entrez Name field. Unlike Entrez name, which is drawn from a list of predetermined gene names, the variant name is free text written by the curator.

.. figure:: /images/figures/CIViC_screenshot-add-evidence-top.png
   :alt: Screenshot of Gene and Variant fields in the Add Evidence form

   Figure 1: Screenshot of Gene and Variant fields in the Add Evidence form
   
Curating Variant Names
----------------------
When curating the Variant Name field, the most specific Variant Name described by the source should be used (e.g. *KRAS* G12 or G13 rather than KRAS Exon 2 Mutation). The Variant Name can be very specific [e.g. *VHL* R176fs (c.528del)], or can refer to a collection of variants fitting a named category (i.e. categorical variants). Examples of categorical variants include *KRAS* G12 or G13, *EGFR* Exon 20 Insertion, and *PIK3CA* Mutation. Categorical variants may be associated with multiple ClinVar entries. The Variant Name field is not limited to genetic events and can include expression or epigenetic alterations such as *BRCA1* Underexpression or *CDKN2A* Promoter Hypermethylation. Other Variant Names, including star-allele nomenclature adopted by the pharmacogenetics field (e.g. DPYD*2A) are also supported. Variant Names can be associated with one or more :ref:`Variant Types <types>` derived from the Sequence Ontology.

**General Conventions:**

- Title case should be used
- Names and HGVS expressions should follow the HGVS 3’ rule. 
- Protein changes should be written in 1-letter form and exclude the preceding 'p.'. 
- HGVS for c. and g. nomenclature should be used and include the preceding 'c.' or 'g.' to differentiate it from protein nomenclature.
- Shorthand should be avoided (e.g., Mutation instead of Mut,Expression instead of Exp) unless part of HGVS nomenclature (e.g., E746_T751delinsVA)
- 'or' rather than '/' should be used to connect variants (e.g. G12 or G13, not G12/G13)
- Frameshift Variant Names should use the shorter HGVS-like protein naming style (e.g., P86fs). The longer protein nomenclature, which includes predicted downstream protein consequences can be included as an alias (e.g., P86Afs*46)
- Somatic variants are not typically described at the genome or transcript level in publications. Protein-effect level descriptions are appropriate for most somatic variants.


================================ ======== ================================ ======================================================================
Variant name                     Gene     Variant type (Sequence Ontology) Demonstrates support of…
================================ ======== ================================ ======================================================================
DPYD*2A Homozygosity             *DPYD*   Splice Donor Variant             pharmacogenomic nomenclature
ALK Fusions                      *ALK*    Transcript Fusion                fusions with an unknown partner common in FISH techniques
EML4-ALK                         *ALK*    Transcript Fusion                specific gene fusions
EML4-ALK E6;A20                  *ALK*    Transcript Fusion                fusions with known specific exon boundaries / specific fusion isoforms
BCR-ABL T315I                    *ABL1*   Missense Variant                 specific variants in the context of other variants
CDKN2A Promoter Hypermethylation *CDKN2A* N/A                              epigenetic modifications
p16 Expression                   *CDKN2A* N/A                              expression changes
rs3814960                        *CDKN2A* 5 Prime UTR Exon Variant         polymorphisms
FLT3-ITD                         *FLT3*   Inframe Insertion                imprecise insertions with shared consequences
Exon 11 Mutation                 *KIT*    Coding Sequence Variant          categorical variants covering specific transcriptional boundaries
DNA Binding Domain Mutation      *TP53*   DNA Binding Site                 categorical variants covering specific functional boundaries
Exon 14 Skipping Mutation        *MET*    Exon Loss Variant                categorical variants covering specific transcriptional consequences
Loss-of-function                 *BRCA*   Loss of Function Variant         categorical variants covering specific functional consequences
================================ ======== ================================ ======================================================================
