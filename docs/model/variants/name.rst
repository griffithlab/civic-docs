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
When curating the Variant Name field, the most specific Variant Name described by the source should be used (e.g. *KRAS* G12 or G13 rather than KRAS Exon 2 Mutation). The Variant Name can be very specific [e.g. *VHL* R176fs (c.528del)], or can refer to a collection of variants fitting a named category (i.e. categorical variants). Examples of categorical variants include *KRAS* G12 or G13, *EGFR* Exon 20 Insertion, and *PIK3CA* Mutation. Categorical variants may be associated with multiple ClinVar entries. The Variant Name field is not limited to genetic events and can include expression or epigenetic alterations such as *BRCA1* Underexpression or *CDKN2A* Promoter Hypermethylation. Other Variant Names, including star-allele nomenclature adopted by the pharmacogenetics field (e.g. DPYD*2A) are also supported. Variant Names can be associated with one or more :ref:`Variant Types <variant-types>` derived from the Sequence Ontology.

**General Conventions:**

- Title case should be used
- Names and HGVS expressions should follow the HGVS 3’ rule. 
- Protein changes should be written in 1-letter form and exclude the preceding 'p.'. 
- HGVS for c. and g. nomenclature should be used and include the preceding 'c.' or 'g.' to differentiate it from protein nomenclature.
- Shorthand should be avoided (e.g., Mutation instead of Mut,Expression instead of Exp) unless part of HGVS nomenclature (e.g., E746_T751delinsVA)
- 'or' rather than '/' should be used to connect variants (e.g. G12 or G13, not G12/G13)
- Frameshift Variant Names should use the shorter HGVS-like protein naming style (e.g., P86fs). The longer protein nomenclature, which includes predicted downstream protein consequences can be included as an alias (e.g., P86Afs*46)
- Somatic variants are not typically described at the genome or transcript level in publications. Protein-effect level descriptions are appropriate for most somatic variants.
- Categorical variants should be singular and exclude the gene name (e.g., Fusion, Rearrangement, Mutation, Frameshift rather than 'ALK Fusions').
- Splice variants should not use IVS nomenclature.

The table below includes an extensive set of example variants for many of the common variant types supported in CIViC. When curating a new variant, curators should refer to these examples and follow the established conventions wherever possible. The {sequence variant} root concept of Sequence Ontology is implied for Variant Type when it's not otherwise specified. 




================================ ======== ================================ ======================================================================
Variant name                     Gene     Variant type                      Application and Notes
================================ ======== ================================ ======================================================================
V600E                            *BRAF*   Missense Variant                 A specific amino acid change. Variant Name encapsulates all the nucleotide changes that could have produced it. Somatic variants are not typically described at the genome or transcript level in publications.
S65W (c.194C>G)                  *VHL*    Missense Variant                 A specific amino acid change where the precise nucleotide change is provided or ascertainable. Protein change p. notation is implied, other HGVS notation (e.g. ‘ g.’ or ‘c.’) used  when applicable. This  degree of resolution is typically used for germline variants.
E709A and G719C                  *EGFR*   Missense Variant                 Multiple concomitant missense variants in the same gene (e.g. double mutants). Should not be used when patients with different mutations in the same gene are pooled and analyzed.
V600E or V600K                   *BRAF*   Missense Variant, 
                                          Copy Number Gain 
                                          {sequence feature}               Complex combination between two different types of variants in the same gene (e.g. missense and copy number gain).  Boolean order of operations and parentheses should be used when needed. 
(V600E or V600K) Amplification   *BRAF*   Missense Variant, 
                                          Copy Number Gain 
                                          {sequence feature}               Complex combination between two different types of variants in the same gene (e.g. missense and copy number gain). Boolean order of operations and parentheses should be used when needed. 
V600                             *BRAF*   Protein Altering Variant         Categorical variant involving a single amino acid position with multiple possible changes. 
Non-V600                         *BRAF*   Protein Altering Variant         Categorical variant excluding a common hotspot This variant describes all *BRAF* mutations that are not at the V600 locus. 
*214C (c.641_642insC)            *VHL*    Stop Lost                        Use * rather than Ter to indicate a stop codon.
D770_N771insNPG                  *EGFR*   Conservative In-frame Insertion  In-frame insertion of one or more amino acids.
V560del                          *KIT*    Conservative In-frame Deletion   In-frame deletion of one or more amino acids.
E746_T751delinsVA                *EGFR*   Delins {sequence feature}        Replacement of one or more amino acids with one or more amino acids.
Y772_A775dup                     *ERBB2*  In-frame Insertion               In-frame duplication of one or more amino acids.
P59fs (c.173_174insT)            *VHL*    Plus 1 Frameshift Variant, 
                                          Frameshift Truncation            Insertion of one or more nucleotides into DNA causing a frameshift.
E189fs (c.565del)                *VHL*    Minus 1 Frameshift Variant, 
                                          Frameshift Truncation            Deletion of one or more nucleotides causing a frameshift.
I206fs (c.615delinsAA)           *VHL*    Plus 1 Frameshift Variant, 
                                          Frameshift Elongation            Replacement of one or more nucleotides with one or more nucleotides causing a frameshift.
A149fs (c.444dup)                *VHL*    Plus 1 Frameshift Variant, 
                                          Frameshift Truncation            Duplication of one or more nucleotides inserted directly 3’ of the original copy of that sequence.
W288fs                           *VHL*    Frameshift Variant               All frameshifts originating at the codon containing the designated locus. Used when the specific DNA change resulting in the frameshift is unknown, thus the first amino acid to change is unknown. 
Exon 9 Frameshift                *CALR*   Frameshift Variant               All frameshifts originating in this exon.
Frameshift                       *MRE11*  Frameshift Variant               All frameshifts within a gene.
Exon 11 Mutation                 *KIT*    Coding Sequence Variant          Mutations within specific transcriptional boundaries.
Exon 14 Skipping Mutation        *MET*    Exon Loss Variant                All mutations causing specific transcriptional consequences. 
DNA Binding Domain Mutation      *TP53*   DNA Binding Site 
                                          {sequence feature}               Mutations within specific functional boundaries. 
Mutation                         *PIK3CA* Transcript Variant               All genetic variants within a gene. Widest categorical variant name for genetic variants.
EML4-ALK                         *ALK*    Transcript Fusion                Specific gene fusion: GENEA-GENEB. Fusions should be named 5’->3’ where GENEA  occurs at the 5’ end of the fusion transcript.  
EML4-ALK e6-e20                  *ALK*    Transcript Fusion                Fusion with known specific exon boundaries; specific fusion isoforms.
BCR-ABL T315I                    *ABL1*   Transcript Fusion,
                                          Missense Variant                 Complex genotype describing a concurrent fusion variant and a missense variant.  
Fusion                           *ALK*    Transcript Fusion                Fusion with an unknown partner (common for fusions detected by methods like FISH).
Rearrangement                    *MLL*    Structural Variant               A change in the structure genetic structure wherein a fusion protein is not necessarily implied to have been created (e.g. translocations, genetic fusions with a regulatory region).
FLT3-ITD                         *FLT3*   In-frame Insertion               Imprecise insertion with shared consequences. 
Exon 1-2 Deletion                *VHL*    Deletion {sequence feature}      Deletion of specific regions of a gene.
Partial Deletion                 *VHL*    Deletion {sequence feature}      All partial deletions where boundaries are not specified. When the size of the deletion is known but the specific exons are not, “Partial deletion of 0.7 Kb” can be included in the Evidence Statement, but not the Variant Name.
Deletion                         *VHL*    Deletion {sequence feature}      Presumed deletion of the whole gene. 
Underexpression                  *ATRX*   N/A                              Reduced or eliminated expression of protein or mRNA products, as detected by assays such as western blots, RT PCR, IHC. Do not use if the causal genomic alteration is known; the alteration would be the variant name.
Loss                             *ARID1A* N/A                              Broadest categorical variant in CIViC. Used when the source describes a mix of genetic and expression events or does not clarify how loss was ascertained. Do not use when authors expression assays are used to confirm genetic results (the genetic event would be the variant name). Loss can be used at the Assertion level to combine Underexpression and deleterious genetic variants.
Amplification                    *PIK3CA* Transcript Amplification         The number of gene copies is greater than two.
Overexpression                   *ERRBB2* N/A                              Increased expression of protein or mRNA products, as detected by assays such as western blots, RT PCR, IHC. Do not use if the causal genomic alteration is known; the alteration would be the variant name.
Splice Site (c.340+1G>A)         *VHL*    Splice Donor Variant             A splice variant that changes the 2 base region at the 5' end of an intron
Splice Site (c.341-2A>C)         *VHL*    Splice Acceptor Variant          A splice variant that changes the 2 base region at the 3' end of an intron
Splice Region (c.463+3A>G)       *VHL*    Splice Donor Region Variant      Splice region within 3-8 bases of the intron.
Splice Region (c.464-4C>T)       *VHL*    Splice Region Variant            Splice region within 3-8 bases of the intron.
Promoter Hypermethylation        *CDKN2A* N/A                              Epigenetic modification.
S473 Phosphorylation             *AKT1*   N/A                              Describe the specific phosphorylated residue(s), if known, or the whole gene if >2 residues or unknown residues were phosphorylated. 
rs3814960                        *CDKN2A* UTR Variant                      rsIDs can be used when easily understandable protein- or splice- altering p. or c. notations are not available.
DPYD*2A Homozygosity             *DPYD*   Splice Donor Variant             Pharmacogenomic nomenclature (can be any applicable variant type). 
p16 Expression                   *CDKN2A* N/A                              Use when distinct proteins (e.g. p16 vs. INK4) are transcribed from the same locus.
================================ ======== ================================ ======================================================================
