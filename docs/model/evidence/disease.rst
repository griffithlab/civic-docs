.. _evidence-disease:

Disease
=======
The disease field requires input that is known to the Disease Ontology database. (`Kibbe et al. 2015 <https://pubmed.ncbi.nlm.nih.gov/25348409/>`__) Disease Ontology (DO) database provides open-sourced ontology for the integration of biomedical data that is associated with human disease. Within the CIViC database, the disease should be the cancer or cancer subtype that is associated to the described Molecular Profile (variant or ensemble of variants) by the evidence being curated. The disease selected should be as specific as possible should reflect the disease type used in the source that supports the evidence statement. In CIViC, Disease is largely synonymous with cancer type or sub-type.

Curating Diseases
-----------------
The disease field will autofill based on existing diseases in the Disease Ontology (DO) database and the most specific disease subtype should be selected, if possible. Only a single disease can be associated with an evidence item. If the Molecular Profile and clinical evidence is implicated in multiple diseases in the source that is being curated, then multiple evidence items should be created. If the disease cannot be identified in the Disease Ontology database, the curator can add this new disease to CIViC during the curation of the associated Evidence Item (Figure 1). Alternatively, new DO terms, definitions, suggestions and questions in regard the Disease Ontology can be submitted to the `DO Term Tracker <https://sourceforge.net/p/diseaseontology/feature-requests/>`__.

.. figure:: /images/figures/Disease_Fig1.png
   :alt: Adding a new disease to CIViC
   
   Figure 1: A new disease term can be added to CIViC during the Evidence Item curation process

The current Diseases (cancer types) with associated with Evidence, Assertions and other information in CIViC can be explored on the `CIViC Disease Page <https://civicdb.org/diseases/home>`__.
