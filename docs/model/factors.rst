Factors
=======

Factors were added to CIViC as a new Feature type, in order to capture a class of biomarkers with relevance for cancer. This new Feature type supports cancer biomarkers that are not associated to specific genes or genomic regions, but have prognostic impact such as microsatellite instability (MSI) in colorectal cancer, or contain predictive/therapeutic information, such as high Tumor Mutation Burden (TMB High), which is responsive to pembrolizumab in solid tumors. A Factor can be associated with multiple Variants, such as TMB High, or TMB Low, where in this example the Factor is "TMB", and the Variants are "High" or "Low". Like all Features in CIViC, Factors are curated using Feature-Variant pairs. 


The sections below will give the user an understanding of the Factor data model 



.. toctree::
   :maxdepth: 2
   :caption: Contents:

   factors/featpage.rst
   factors/varpage.rst
   factors/brouwse.rst
      
