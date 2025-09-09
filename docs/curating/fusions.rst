.. _curating-fusions:

Curating Fusions
================

Fusions in CIViC are a distinct Feature type, and follow a relatively simple model, which aligns with the VICC (Variant Interpretation for Cancer Consortium) Gene Fusion Specification. Fusions consist of two gene partners, with the option for one of the genes to be unknown or not specified (multiple potential gene partners). The Fusion model allows for general Fusion Variants where the specific exons are not specified, and also can incorporate exon structure when it is known or of biological significance, as well as offsets which can contain intronic sequence. It additionally describes transcribed chimeric transcripts, as well as interactions between a rearranged regulatory element and the expression of a partner gene product, termed regulatory fusions. 

Fusion Features are associated to two Variant types, first being a categorical “Bucket” Variant termed Fusion (e.g. BCR::ABL1 Fusion), which captures evidence not associated with a specific exon junction structure. A second type of Fusion variant captures specific exon structure (e.g. EML4::ALK e6::e19). Regulatory Fusions were added utilizing a nomenclature defined by the VICC.




.. _curating-fusions-general:

General Fusion Curation Practice
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


The most common way Fusions are added to CIViC is via the Add Evidence form. This is located at the upper right corner of the user interface (UI). Once the form is open, curators choose the Fusion Feature type from a dropdown, and can next either pull up an existing Fusion from the pulldown menu, or crate a new Fusion. After that, a Variant is chosen either from existing Variants for the Fusion, or a new Variant is created for that Fusion. Fusion Variants are of two types, either an exon agnostic general or bucket Fusion variant, or an exon specific variant (eX::eY), where X and Y are the exon numbers.



.. rubric:: Fusion Curation Workflow

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/fusinC1.png
   :alt: Fusion Curation Workflow
   :title: Figure 1: (A) The curator adds new Evidence using the menu on the upper right of the user interface (UI). (B) The curator chooses to add new evidence for the Fusion Feature type. (C) Typeahead allows the curator to choose from existing Fusions that have already been curated in CIViC. (D) If the text entered by the curator does not match existing Fusions, the option to open the Fusion Builder is shown. The curator will then use the Fusion Builder to create a new Fusion Feature. (E) After choosing a new or existing Fusion, the curator will choose a Variant for curation. The generalized Fusion bucket Variant is always given as an option. (F) If the curator wants to use an exon specific Variant, they may start to type out that variant in the eX::eY form, where X and Y are numbers of the exons (UTR exons are counted in these numbers). If that eX::eY Variant for those specific numbers does not yet exist in CIViC, the curator may open the Fusion Variant Builder to create a new exon specific Variant.  
   :show_caption: True

|


For creation of new Fusion Features, a Fusion Builder option is given to the curator during the Add Evidence process. This Fusion Builder follows a straightforward procedure where the curator chooses HGNC gene names provided by Entrez for the Fusion. The curator may choose two genes when both are specified for the Fusion. In some cases, one partner in a Fusion may be unknown or not specified due to mulitple partners, and for these cases, a **?** or the letter **v** are used, respectively. This is often the case when break apart FISH assays are used, as in fusions involving ALK, which are represented in CIViC as **v::ALK Fusion**.



.. rubric:: Fusion Builder in the Add Evidence Form

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/fusinC2.png
   :alt: Fusion Builder
   :title: Figure 2: The Fusion Builder allows curators to add new Fusion Features to CIViC. (A) The curator may specify two genes provided by Entrez, when both Fusion parters are known. (B) If one of the parters is unknown or unspecified as in the case of multiple different partners, then the curator can choose Unknown or Multiple from the dropdown.  
   :show_caption: True

|


.. _curating-exons:

Fusion Coordinate Curation Practice
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For exon specific Fusion-Variants, where the Variant is of the form eX::eY, with X and Y being exon numbers, a Fusion Variant Builder is provided. 


.. rubric:: Fusion Variant Builder

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/fusinC3.png
   :alt: Fusion Variant Builder
   :title: Figure 3: The Fusion Variant Builder allows curators to create new exon specific Fusion Variants. The curators must provide a reference build and ensembl transcripts for each gene specified in the Fusion. 5' end exon and 3' start exon numbers relative to the chosen transcripts (counting UTR exons) must also be provided by the curator. When applicable, exon offsets, and direction of offset can be provided for either gene, if part of an exon is cut off, or if some intronic material is present in the transcribed Fusion.
   :show_caption: True

|



An overall model of how coordinates for Fusions in CIViC are interpreted is shown below. Note that when the CIViC interface calculates coordinates, the untranslated region (UTR) exons are included, and that the coordinate is calculated from the last DNA base within the given exon. Offsets are calculated from the position as specified in the figure.


.. rubric:: Interpreting Fusion Coordinates

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/fusin_7.png
   :alt: Fusion Coordinates
   :title: Figure 4: Fields in the Fusion Variant coordinate tables are filled out according to the scheme shown. For each partner gene, Start coordinate is always smaller than the Stop coordinate, regardless of strand orientation. Exon coordinates include untranslated regions (UTRs). The coordinate of the last base in the exon or UTR is used, and the Offset is counted from this base in a positive or negative direction. 
   :show_caption: True

|



Representative exon coordinates may also be specified for the generalized Fusion bucket Variant type. In this case, the chosen exons represent the most common or most clinically impactful combination seen in patients. Note also that representative exons may be specified for Fusions where one of the parters is Unknown or Multiple, as seen on the Fusion Variant page for the Feature-Variant pair **v::ALK Fusion** below:


.. rubric:: Variant Page for the v::ALK Fusion

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/fusin_CL.png
   :alt: Variant Page for the v::ALK Fusion
   :title: Figure 5: Shown is the Variant page for the v::ALK Fusion Feature-Variant pair. Representative coordinates have been curated for the 3' gene ALK, whereas the 5' gene coordinates are not curated, since multiple potential genes parters for ALK are possible for this Feature. 
   :show_caption: True

|


