Curating Molecular Profiles
===========================

The Molecular Profile (MP) data model is described in the :doc:`Understanding MPs section <../model/molecular_profiles/name>`. A curator adding Evidence Items (EIDs) to CIViC will utilize Molecular Profiles for curation of either a single or combination of variants. In the new workflow model (Figure 1), a curator will choose from two MP types:

**Simple Molecular Profile:** A simple Molecular Profile (MP) is comprised of a single Feature-Variant pair. The simple MP replaces the CIViC Variant in the old curation workflow of CIViC, where each EID described a single variant associated with a single Gene (Figure 1).

**Complex Molecular Profile:** A complex Molecular Profile (MP) is comprised of two or more Feature-Variants. In the new CIViC workflow model, evidence for complex combinations of Feature-Variants may be curated and different Variants in a complex MP may be associated with different Genes, Fusions, or Factors (Figure 1).

.. thumbnail:: /images/figures/curating_molecular_profiles_fig1.png
   :alt: Figure depicting the old, single variant workflow model and new Molecular Profile based CIViC workflow model for curation
   :title: Figure 1: Old, single variant workflow model and new Molecular Profile based CIViC workflow model for curation
   :show_caption: True

|

Molecular Profiles are named with the Feature first, and then the specific Variant name (Figure 2). This convention is followed for both simple and complex MPs. Thus in the Molecular Profile **“EGFR L858R OR BRAF V600E”** the user and curator knows which Feature (in this case Gene) each Variant in the MP is associated with.

.. thumbnail:: /images/figures/curating_molecular_profiles_fig2.png
   :alt: Figure depicting the difference between a CIViC Variant compared to simple and complex CIViC Molecular Profiles
   :title: Figure 2: CIViC Variant versus a simple and a complex Molecular Profile
   :show_caption: True

|

An important thing for curators to note is the difference in the CIViC workflow and UI between variants and MPs. When going to a gene page such as EGFR, the MPs associated with the gene are shown by default (Figure 3). There is also a tab called Variants on this page that will allow the user or curator to view the collection of individual variants associated with the gene.

.. thumbnail:: /images/figures/curating_molecular_profiles_fig3.png
   :alt: Figure depicting how CIViC Molecular Profiles are associated to a gene and are displayed on the gene page in the user interface
   :title: Figure 3: Molecular Profiles associated to a gene are displayed on the gene page in the user interface
   :show_caption: True

|

In the old CIViC workflow model (Figure 1), a user might search for a Gene of interest, landing at the CIViC page for that Gene. This page contained all of the Variants which had curated information for that Gene of interest. The user or curator could then select an individual Variant of interest, each of which had their own page, and then see all of the Evidence Items (EIDs) curated for that Variant at the bottom of the Variant page. In the new workflow model, things are very similar, in that a user can go to the Feature (Gene, Fusion, or Factor) page, but now they see a list of Molecular Profiles that contain a at least one Variant of that Feature. In the case of Gene Features, the majority of MPs on a Gene page will usually be simple MPs containing Variants for the Gene as in Figure 3, where MPs such as EGFR L858R, EGFR T790M, and other familiar simple MPs are seen. At the end of the collection of simple MPs the user will find complex MPs which contain at least one Variant associated to the Gene whose page they are on. These complex MPs can also contain Variants associated with Genes or generally Features other than that of the Gene page. Thus on the EGFR Gene page one finds the complex Molecular Profile EGFR L858R AND MET Amplification, or on the BRAF Gene page one finds the complex MP BRAF V600E AND MSI Low. Note these MPs will also be visible on the Met Gene page, or the MSI Factor page, respectively. So, to find a specific complex MP, a user can go to any Feature page that has a Variant that is part of the complex MP and find the MP there. 

.. thumbnail:: /images/figures/curating_molecular_profiles_fig4.png
   :alt: Figure depicting the CIViC browse view for Molecular Profiles
   :title: Figure 4: Browse Molecular Profile functionality
   :show_caption: True

|

Another approach for a user or curator to locate MPs of interest is to use the Browse functionality (Figure 4), which can be used for all top level entities in CIViC including Molecular Profiles, found at the left of the user interface. If the user wants to see all MPs which contain a Variant called V600E, then as in Figure 4, the user can type that into the Variants field, and all MPs containing a variant named V600E will be shown, and in this case all V600E variants are associated to the Gene BRAF. Both simple and complex MPs are shown. Note if a user were interested in all MPs containing a bucket variant such as EGFR Mutation, then the user could type Mutation into the Variants field, and then EGFR into the Genes field, in order to narrow down the display to MPs containing only EGFR Mutation, instead of seeing all MPs containing the Variant named Mutation, since many Gene Features have a bucket variant called Mutaion associated to them.

On the Gene page, the user can also choose the Variants tab (Figure 3), and see all of the Variants associated to the Gene, such as L858R or T790M for EGFR. Clicking on one of these will take the user to a Variant page, and on the Variant page are listed Variant related information such as coordinates, and also a list of all simple and complex MPs that contain the variant. Each Variant page is accessible from the respective Feature page that it is associated to.  

**Creation of new complex Molecular Profiles when adding Evidence Items**

All Evidence Items (EIDs) in CIViC are associated with either a simple or complex Molecular Profile (MP). When adding new Evidence Items to CIViC, the curator can choose either a simple MP or a complex MP in the Molecular Profile field of the Add Evidence Item Form (Figure 5). 

.. thumbnail:: /images/figures/curating_molecular_profiles_fig5.png
   :alt: Figure depicting how a CIViC user can choose to add a simple or complex Molecular Profile
   :title: Figure 5: Choosing to add an Evidence Item for a simple or complex Molecular Profile
   :show_caption: True

|

Adding a simple MP in the Add Evidence Form requires the curator to first specify a Feature, and then specify a Variant associated with that Feature. As with simple MPs, new complex Molecular Profiles are added to CIViC during the process of adding the first EID specific to that complex MP.  The Process by which a new complex MP is created in the Add Evidence Form is outlined in the workflow figures below (Figure 6).

.. thumbnail:: /images/figures/curating_molecular_profiles_fig6a.png
   :alt: Figure depicting the selection of a Gene for a Molecular Profile
   :title: Figure 6a: Workflow for creation of new complex Molecular Profiles in the Add Evidence Form - Selecting a Gene
   :show_caption: True

|

.. thumbnail:: /images/figures/curating_molecular_profiles_fig6b.png
   :alt: Figure depicting the selection of a Variant and boolean operator for a Molecular Profile
   :title: Figure 6b: Workflow for creation of new complex Molecular Profiles in the Add Evidence Form - Selecting a Variant and boolean operator
   :show_caption: True

|

.. thumbnail:: /images/figures/curating_molecular_profiles_fig6c.png
   :alt: Figure depicting the selection of additional variant(s) to create a complex Molecular Profile
   :title: Figure 6c: Workflow for creation of new complex Molecular Profiles in the Add Evidence Form - Selection additional variant(s)
   :show_caption: True

|

