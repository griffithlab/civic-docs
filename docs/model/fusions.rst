Fusions
=======

Fusions have been a part of CIViC since its earliest data models, but were associated directly with Genes as Gene-based Variants. This approach utilized a single Variant associated with a single Gene. To enhance the representation and features for Fusions, Fusions are now a distinct class of Features. Fusions in CIViC follow a relatively simple data model that is able to capture the main dimensions of complexity that characterize the clinical relevance of gene fusions. CIViC Fusions consist of two genes (following HGNC standards), or a stand-in symbol when then one gene is variable (v) or unknown (?) (See VICC standards linked below). Fusion names are auto-generated, with the 5’ gene first, the 3’ gene second and a double colon :: placed between the two gene names. In general, the CIViC Fusion data model is compatible with the VICC Gene Fusion Specification (https://fusions.cancervariants.org/en/latest/).


The sections below will give the user an understanding of the Fusions data model 



.. toctree::
   :maxdepth: 2
   :caption: Contents:

   fusions/types
   fusions/FeaturePage
   fusions/FusVar
   fusions/FusCor

