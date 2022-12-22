.. _evidence-drug:

Therapy
=======
Therapies in CIViC are associated with Evidence Items or Assertions of the Predictive Type, which describe sensitivity, resistance or adverse response to drugs or other treatments when a given Molecular Profile is present in a patient or a preclinical model system. The Therapy field may also be used to describe more general treatment types and regimes, such as FOLFOX or Radiation, as long as the literature derived Evidence Item makes a scientific association between the Drug (treatment type) and the presence of the Molecular Profile (Molecular Profiles are comprised of a variant or collection of variants).


Curating Therapies
------------------
If the Evidence Item’s Evidence Type is Predictive, a new button entitled “Add a Therapy” will become available (Figure 1). It is required to add a Therapy if the Predictive Evidence Type is chosen. After clicking “Add a Therapy”, a field to type the Therapy name will appear. The curator can type the name of a therapy such as erlotinib, and a menu will appear with Therapies drawn from NCIT that contain the name. The specified Therapy will possess an NCI Thesaurus ID whenever available. Although often searchable, trade names for treatments should not be used.

.. figure:: /images/figures/Thera_Fig1.png
   :alt: Overview of adding a therapy to predictive EID

   Figure 1: Adding a Therapy to a Predictive Evidence Item

After the Therapy is chosen from the menu, it will appear in the Add Evidence Form as shown in Figure 2. A popover menu can be accessed from the Therapy, and it contains information on how many Evidence Items and Assertions use the Therapy, as well as a link to the NCIT page for the Therapy.

.. figure:: /images/figures/Thera_Fig2.png
   :alt: Showing link to NCIT page for Therapies with an NCIT ID

   Figure 2: Link to NCIT page for Therapies with an NCIT ID

Multiple Therapies can be added to a single Evidence Item, however, if two or more Therapies are added to an Evidence Item the curator is required to provide a Therapy Interaction Type. Therapy Interaction Types can be either combination, sequential, or substitutes. The Therapies and Therapy Interaction Types should be explicitly stated in the source supporting the Evidence Item.

.. figure:: /images/figures/Thera_Fig3.png
   :alt: Overview of dding more than one therapy and specifying Therapy Interaction Type

   Figure 3: Adding more than one therapy and specifying Therapy Interaction Type

When a Therapy is not present in the NCIT, the Curator can add a new Therapy name to the Evidence Item (EID) field during EID curation, and it will then be added to the CIViC database (Figure 4). If the Therapy is not found, it may be helpful to search the NCIT directly (https://ncithesaurus.nci.nih.gov/) using relationships and mappings before creating a novel treatment in CIViC. The NCIT supports drug classes (e.g., EGFR Tyrosine Kinase Inhibitor, C2167), but the most precise therapy or combination should be used whenever possible (e.g., Afatinib, Erlotinib - Substitutes).

.. figure:: /images/figures/Thera_Fig4.png
   :alt: Overview of adding a Therapy not present in NCIT

Figure 4: Adding Therapy not present in NCIT

Therapies added to CIViC which are not in NCIT should be submitted to NCIT using this form to submit new terms to the `NCI Thesaurus <https://ncitermform.nci.nih.gov/ncitermform/>`__.
