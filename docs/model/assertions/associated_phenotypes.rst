Associated Phenotypes
=====================
Associated Phenotypes for an Assertion are phenotypes that have been observed and recorded in patients documented to have the specific variant for which the Assertion has been created. The Associated Phenotypes field is hand curated and terms are drawn from the Human Phenotype Ontology (HPO).

Curating Associated Phenotypes
------------------------------
Associated Phenotypes for an Assertion are a collection of the Associated Phenotypes taken from the Assertion’s supporting Evidence Items.

Any phenotypes added to an Assertion’s Associated Phenotypes field must occur in at least one of the supporting Evidence Items (EIDs). Note that when an HPO term is added to an EID, it has been reported in the specific evidence source for that EID in a patient with the specific CIViC Variant for that EID. 

Supporting EIDs for a given Assertion may be drawn from categories of different generality (i.e. an EID for “Cancer” may support an Assertion for melanoma). Therefore, curators should be careful to only draw HPO terms to use in the Assertion from EIDs that strictly match the Assertion Disease and Variant in a highly specific manner.

Note that the HPO Terms chosen for Associated Phenotypes for an Assertion do not give quantitative data. For instance a given HPO term may be found in multiple supporting EIDs for an Assertion, while a second HPO term may occur only once in the collection of supporting EIDs. In the Assertion, both terms will occur only once. Therefore the information on frequency of phenotype observation is not carried over into the Assertion. While the collection of evidence supporting an Assertion should do a good job of covering the field for that given variant , CIViC Clinical Significance, and disease, the system of publishing on variants and noting Associated Phenotypes may not yet be reliable enough to use literature curation as a measure for phenotype frequency, especially when the numbers are small. For variants with larger bodies of curated literature in CIViC, advanced search functions can give statistics on phenotype frequency occurring in literature for a given variant.   

