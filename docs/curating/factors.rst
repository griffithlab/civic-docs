.. _curating-factors:

Curating Factors
================

Factors are a Feature type designed to capture a set of genomic phenomena associated with clinical impact in cancer such as Tumor Mutational Burden (TMB), Microsatellite instability (MSI), Kataegis, Chromothripsis, or the presence of HPV infection, among others. Each Factor is associated to a corresponding term from the NCI Thesaurus. Factors also share the common property that Factor associated Variants do not have coordinates, and instead Factors represent more global genomic phenomena. 




.. _curating-factors-general:

General Factor Curation Practice
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

As with all Features in CIViC, new Factors are mainly added when a new Evidence Item is curated for the given Factor. During this process, curators can add new Factors, or chose from existing ones. Evidence is curated for Molecular Profiles (MPs), which consist of one or more Feature-Variant pairs. Therefore Factor-Variant curation is an essential part of the process, and curators can choose from existing Variants for an existing Factor, or make new Variants for the chosen Factor. 


.. rubric:: Curation Process for Factors in CIViC

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/figures/factC5.png
   :alt: Curation Process for Factors
   :title: Figure 1: When new evidence is added, the curator first chooses what Feature type they will curate for. When Factor is chosen, the curator will either choose an existing Factor, or create a new one. After this the curator will choose from existing Variants for a Factor that is already in CIViC, or create a new Variant. If a new Factor has been created, then a new Variant will also be created, to finish off the Feature-Variant pair for the Molecular Profile that evidence is being curated for. After creation of the Factor, a link to NCIT should be added using the Revise functionality on the Feature page for the new Factor.
   :show_caption: True

|

Note that for a complex Molecular Profile (MP) consisting of multiple Feature-Variant pairs, where one or more of the Features is a Factor, then the above process still holds, and simply occurs within the context of the creation of other Feature-Variant pairs that make up the complex MP. 

The curation process for making new Factors is further outlined below:



.. rubric:: Adding Factors to CIViC

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/figures/factC6.png
   :alt: Adding Factors
   :title: Figure 2: (A) The curator chooses to Add Evidence Item at the upper right part of the user interface. (B) on the Add New Evidence form, the curator chooses the Factor from the available Feature types. (C) Using typeahead, the curator either chooses an existing Factor, or types in the name for a new Factor if needed. (D) The curator chooses from existing Variants for the chosen Factor, or creates a new Variant for that Factor if needed. 
   :show_caption: True

|


.. revising-factors-general:

General Factor Revision Practice
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Factors are revised using the Revise Factor form, accessed using the Revise button at the upper right of the Factor page. Here multiple fields are available for curation and revision. The Factor Name is usually chosen to be relatively short, in order to work within the different tables and views of the user interface (UI). A longer name for the Factor, called the Full Name, is available for curation, and often displayed in the UI next to the Name. The curator can also add the NCI Thesaurus Code that corresponds to the Factor. If no entry in the NCIT exists for the Factor, one should be submitted to NCI. Aliases for the Factor should be added, along with a Summary explaining the Factor. 


.. rubric:: Revise Factor Form

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/figures/factCb2.png
   :alt: Revise Factor Form
   :title: Figure 3: The Revise Factor page is available via the Revise button at the upper right on the Factor Page. Multiple fields are available for curation and revision in this view.
   :show_caption: True

|



Note that for the Factor-Variant pair such as **MSI Low**, there are three main pages available:

- **MSI** Feature Page
- **MSI Low** simple Molecular Profile Page
- **Low** Variant Page (where the Variant "Low" is uniquely associated to the Factor MSI)

Each of these pages has curatable and revisable fields, accessible using the Revise button at the upper right of the user interface.

Note also that any complex Molecular Profiles containing **MSI Low** as one of the Feature-Variant pairs, such as **BRAF V600E AND MSI Low** also have their own Molecular Profile Page, which also can be curated and revised by the same method of clicking the Revise button at the upper right of the user interface.

