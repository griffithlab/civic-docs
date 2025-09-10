Fusion Variants
===============

There are two general classes of Fusion variant. The first class is the “Fusion” class. Examples of Feature-Variant pairs with this Variant type are EML4::ALK Fusion, or v::ALK Fusion. In these examples the Fusion Features are EML4::ALK, or v::ALK, and the Variant in each case is "Fusion". This Variant type is meant to serve as a Categorical or Bucket Variant, capturing any specific Fusion of the EML4::ALK type, or any Fusion of the v::ALK type, where v stands for any of the multiple, known ALK Fusion partners that occur in the 5’ position. Fusion Variants of this type are often found in practice using assays such as break apart FISH, that can demonstrate the presence of the fusion, but not necessarily determine the fusion partner or the exon breakpoints.

- For an unknown gene component, the symbol “?” is used for the unknown gene component (see VICC documentation: https://fusions.cancervariants.org/en/latest/nomenclature.html#unknown-gene-component)
- For a variable gene component, the symbol “v” is used for the variable gene component (see VICC documentation: https://fusions.cancervariants.org/en/latest/nomenclature.html#multiple-possible-gene-component)

“Fusion” class variants are displayed with the fixed Variant name "Fusion". This Variant automatically gets created when a new Fusion Feature is added. Some examples of this are shown below:

.. rubric:: Two Fusion Variant Types in CIViC

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/fusin_1.png
   :alt: Fusion Types in CIViC
   :title: Figure 1: Two Fusion Variant types are present in CIViC. One type is the Fusion bucket or categorical Variant type, which captures any Fusion of the specific two Genes, regardless of exon combination. The second Fusion Variant type captures specific exon junction information. 
   :show_caption: True

|

The second class of Fusion variant is the exon specific, and appears in the interface as eX::eY. This class of Fusion-Variant pairs is designed to capture the specific exons that are fused together between Gene1 (5’ Gene) and Gene2 (3’ Gene), so the overall form of the Feature-Variant pair in this case is Gene1::Gene2 eX::eY, where X and Y are integers representing the fused exons from 5’ Gene and 3’ Gene, respectively. For eX::eY Variants, curators provide the following information when adding a new Variant of this type:

- Ensembl transcript IDs for all Genes in the fusion. Preferably the MANE Select or MANE Select Plus Clinical transcript, when available. Usually two Ensembl transcript IDs are provided, but if one of the genes is variable or unknown (v or ?), then only one transcript ID is provided.
- Exon numbers for each gene based on the chosen Ensembl transcript, where it is applicable. For a known 5’ Gene partner the number of the last exon included in the fusion product is provided. For a known 3’ Gene partner the number of the first exon included in the fusion product is provided. 
- Note that exon numbering should start with the first exon of the transcript regardless of where the coding sequence starts. In other words, exons that contain only UTR sequence are still counted.
- Optional offsets for each exon are also provided if more or less than the known exon sequence is involved in the fusion.

Curation specifics for Fusions are provided in the curation section. 
