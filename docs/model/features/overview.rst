Overview of Features
====================

Features are used to classify different groups of biomarkers with clinical relevance for cancer to support curation of structured data relevant to that type of biomarker. Features in CIViC are currently Genes, Fusions, and Factors, with other Features under development and planned for the future. For example, Genes are specific regions of the genome, named using HUGO nomenclature, and associated with structured data such as refseq or ensembl transcripts, aliases, and protein structures. The original CIViC Variant data model was built entirely around Genes, and the majority of CIViC documentation is based on curation of variants directly associated to the Gene Feature class. But with that in mind, the data model for other Features broadly follows many aspects of the data model for Genes, including the relationship between Genes and Variants as seen below.


.. thumbnail:: /images/figures/Features1.png
   :alt: Screenshot of an A-level (validated) evidence item summary
   :title: Figure 1: Screenshot of an A-level (validated) evidence item summary
   :show_caption: True

|


.. thumbnail:: /images/figures/Feat_dataM2.png
   :alt: The Generalized Feature-Variant data model
   :title: Figure 2: Generalized Feature-Variant Data Model
   :show_caption: True

|


Features generalize a fundamental relation between a Gene and its Variants, so that for any instance of a Feature, multiple different variants may be associated with it. For example, a Fusion (Fusions are a class of Feature in CIViC) such as EML4::ALK can be associated with multiple Variants. In the case of Fusions, Variants may include different exon combinations, such as e6::e20 (EML4 exon 6 fused to ALK exon 20) and e20::e20, or the representative Fusion bucket variant when the specific breakpoints are not known (see section on Fusions and sections on other Feature types for more in-depth examples). With this generalization of the Gene-Variant data model to Features, it is especially useful to think of Variants in CIViC in terms of Feature-Variant pairs (e.g. BRAF V600E, HPV Positive, EGFR Mutation, EML4::ALK e6::e20, v::ALK Fusion). An overview of different Features in CIViC which are either implemented or under development is shown in the figure below:

.. thumbnail:: /images/figures/Feat_dataM3.png
   :alt: Figure of Feature Types in the CIViC Data Model
   :title: Figure 3: Feature Types in the CIViC Data Model
   :show_caption: True

|


