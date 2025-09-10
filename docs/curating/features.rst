Curating Features
=================
Features are a top level entity in CIViC, enabling the classification of Variants into different classes.


.. rubric:: Overview of Features

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/figures/Features1.png
   :alt: Overview of Feature Types in CIViC
   :title: Figure 1: The three Feature types currently available in CIViC are Genes, Fusions, and Factors
   :show_caption: True

|






Adding New Features
~~~~~~~~~~~~~~~~~~~


.. rubric:: Adding New Features to CIViC

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/figures/Cur_Feat2.png
   :alt: Adding new Features to CIViC
   :title: Figure 2: New Features are most commonly added to CIViC using the Add Evidence functionality.
   :show_caption: True

|



Features are added to CIViC primarily by the Add Evidence functionality. This functionality allows the curator to see if the Feature they want to curate for is already in CIViC, and additionally if the Variant associated to the Feature is already in the CIViC knowledgebase. When the Add Evidence functionality is used, the curator sees the Molecular Profile fields that can be curated. Recall that a Molecular Profile (MP) consists of one or more Feature-Variant pairs. Simple MPs hold one Feature-Variant pair (e.g. BRAF V600E), and Complex MPs are combinations of two or more Feature-Variant pairs (e.g. BRAF V600E AND MSI High). When adding a new Feature, the curator first chooses the Feature type (Gene, Factor, or Fusion). The curator then types in the adjacent field, and typeahead functionality searches through the existing Features to see if the desired Feature already exists. Typeahead results are displayed below the field. If the typeahead does not yield the desired Feature, the curator is prompted to make a new Feature, as shown below. Once the new or existing Feature is chosen, a similar process is followed for adding a new Variant associated to the Feature, to create the Feature-Variant pair. For Complex MPs, this process is repeated for each element of the complex MP (See section on curating MPs).



.. rubric:: Making New Features When Adding Evidence Items

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/figures/Cur_Feat3.png
   :alt: Adding new Features to CIViC
   :title: Figure 3: When curating Evidence Items in CIViC, a curator chooses a Feature type (in this case they have chosen a Factor), and then they choose a specific Variant associated to that Feature. The interface allows for the creation of new Feature instances, and new Variants associated to the chosen Feature. 
   :show_caption: True

|



.. rubric:: Creation of New Features in CIViC

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/figures/Cur_Feat4.png
   :alt: Screenshot of creating a new Feature using Add New Evidence interface
   :title: Figure 4: If the desired Feature does not exist in CIViC, the curator has the option to create it in the Add New Evidence interface. 
   :show_caption: True

|




Revising Features
~~~~~~~~~~~~~~~~~

As with other CIViC entities, curators can click the Revise button in the upper right of the Feature’s page to create a revision, as seen in the images below. This will open up a form with a set of fields that can be curated for the Feature. The fields that are available depend on the type of Feature chosen (Gene, Factor, or Fusion). Note also that MPs consist of Feature-Variant pairs, and Variants also have curateable fields which depend on the Variant’s Feature type. Revising Variants is very similar to Revising Features, as each Variant has its own page, with a Revise button accessible on the upper right of the screen.




.. rubric:: Revising a Feature in CIViC

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/figures/Cur_Feat5.png
   :alt: Revision of a Feature
   :title: Figure 5: Functionality to revise Features is accessed using the Revise button at the upper right corner of the interface on the Feature page (In this example the Feature is the Factor MSI)
   :show_caption: True

|



.. rubric:: Page for Feature Revision in CIViC

..
  Filename: BGA-113_variant-group_model  Artboard: model

.. thumbnail:: /images/figures/Cur_Feat6.png
   :alt: Screenshot of Feature Curateable Fields
   :title: Figure 6: Depending on the class of Feature, different curatable fields will be available. Above are the curatable fields for the Factor 
   :show_caption: True

|








