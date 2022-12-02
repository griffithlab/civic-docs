.. _evidence-drug:

Drug
====
Drugs in CIViC are associated with Predictive Evidence Types, which describe sensitivity, resistance or adverse response to drugs when a given variant is present. The Drug field may also be used to describe more general treatment types and regimes, such as FOLFOX or Radiation, as long as the literature derived Evidence Item makes a scientific association between the Drug (treatment type) and the presence of the variant.

Curating Drugs
--------------
If the evidence item’s evidence type is predictive, a new field entitled, “Drug Names” will become available. Drugs specified will possess a NCI Thesaurus ID whenever possible, and when an NCIT ID is specified for the drug, it will link to the corresponding NCIT page. 

When a drug is not present in the NCIT, then the Curator can add the drug name by hand into the Evidence Item (EID) field during EID curation, and it will then be added to the CIViC database.

Drugs added to CIViC which are not in NCIT should be submitted to NCIT using this form to submit new terms to the NCIT: https://ncitermform.nci.nih.gov/ncitermform/

Multiple drugs can be added to a single evidence item, however, if two or more drugs are added to an evidence item, the curator is required to provide a drug interaction type. Drug interaction types can be either combination, sequential, or substitutes. The drugs and drug interaction types should be explicitly stated in the source supporting the evidence item.

Curating Interaction Types
--------------------------
The Interaction Type "combination" is used to indicate multiple drugs that are taken concurrently as part of a cocktail (e.g. Variant A predicts sensivity to the combination of Drug X and Y). The Interaction Type "substitutes" is used to indicate drugs that are to considered equivalent or alternatives to each other for the purposes of the current Evidence Item (e.g., Variant A predicts sensitivity to either Drug X or Drug Y). The Interaction Type "sequential" is the least common in CIViC and is used to indicate drugs that are taken in a series, in a particular order. 

The current Therapies (Drugs) associated with Evidence Items, Assertions and other information in CIViC can be explored on the `CIViC Drugs Page <https://civicdb.org/drugs/home>`__.

