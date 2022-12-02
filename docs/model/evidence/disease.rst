.. _evidence-disease:

Disease
=======
The disease field requires input that is known to the Disease Ontology database. (`Kibbe et al. 2015 <https://pubmed.ncbi.nlm.nih.gov/25348409/>`__) Disease Ontology (DO) database provides open-sourced ontology for the integration of biomedical data that is associated with human disease. Within the CIViC database, the disease should be the cancer or cancer subtype that is a result of the described variant. The disease selected should be as specific as possible should reflect the disease type used in the source that supports the evidence statement. In CIViC, Disease is largely synonymous with cancer type or sub-type.

Curating Diseases
-----------------
The disease field will autofill based on existing diseases in the Disease Ontology (DO) database and the most specific disease subtype should be selected, if possible. Only a single disease can be associated with an evidence item. If the variant and clinical evidence is implicated in multiple diseases then multiple evidence items should be created. If the disease cannot be identified in the Disease Ontology database, the “Could not find disease” box can be selected and a new field will appear that permits free text. Alternatively, new DO terms, definitions, suggestions and questions in regard the Disease Ontology can be submitted to the `DO Term Tracker <https://sourceforge.net/p/diseaseontology/feature-requests/>`__.

The current Diseases (cancer types) with associated with Evidence, Assertions and other information in CIViC can be explored on the `CIViC Disease Page <https://civicdb.org/diseases/home>`__.

