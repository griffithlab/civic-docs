Curating Molecular Profiles
===========================

The Molecular Profile (MP) data model is described in the Understanding MPs section (link to Understanding MPs). A curator adding Evidence Items (EIDs) to CIViC will utilize Molecular Profiles for curation of either a single or combination of variants. In the new workflow model (Figure 1), a curator will choose from two MP types:

**Simple Molecular Profile:** A simple Molecular Profile (MP) is comprised of a single variant. The simple MP replaces the CIViC Variant in the old curation workflow of CIViC, where each EID described a single variant associated with a single gene (Figure 1).

**Complex Molecular Profile:** A complex Molecular Profile (MP) is comprised of two or more variants. In the new CIViC workflow model, evidence for complex combinations of variants may be curated and different variants in a complex MP may be associated with different genes (Figure 1).

.. thumbnail:: /images/figures/curating_molecular_profiles_fig1.png

**Figure 1: Old, single variant workflow model and new Molecular Profile based CIViC workflow model for curation**

Molecular Profiles are named with the gene first, and then the specific variant name (Figure 2). This convention is followed for both simple and complex MPs. Thus in the Molecular Profile **“EGFR L858R OR BRAF V600E”** the user and curator knows which gene each variant in the MP is associated with.

.. thumbnail:: /images/figures/curating_molecular_profiles_fig2.png

**Figure 2: CIViC Variant versus a simple and a complex Molecular Profile**

An important thing for curators to note is the difference in the CIViC workflow and UI between variants and MPs.  When going to a gene page such as EGFR, the MPs associated with the gene are shown by default (Figure 3). There is also a tab called Variants on this page that will allow the user or curator to view the collection of variants associated with the gene.

.. thumbnail:: /images/figures/curating_molecular_profiles_fig3.png

**Figure 3: Molecular Profiles associated to a gene are displayed on the gene page in the user interface**

In the old CIViC workflow model (Figure 1), a user might search for a gene of interest, landing at the CIViC page for that gene. This page contained all of the variants which had curated information for that gene of interest. The user or curator could then select an individual variant of interest, each of which had their own page, and then see all of the Evidence Items (EIDs) curated for that variant at the bottom of the variant page. In the new workflow model, things are very similar, in that a user can go to the gene page, but now they see a list of Molecular Profiles that contain a variant of the gene for at least one of their elements. The majority of MPs on a gene page will usually be simple MPs containing variants for the gene as in Figure 3, where MPs such as EGFR L858R, EGFR T790M, and other familiar simple MPs are seen. At the end of the collection of simple MPs the user will find complex MPs which contain at least one variant from the gene of interest. These complex MPs can also contain variants associated with genes other than that of the gene page. Thus on the EGFR gene page, one finds the complex Molecular Profile BRAF V600E AND EGFR L858R AND EGFR T790M. So, to find a specific complex MP, a user can go to any gene page that has a variant that is part of the complex MP and find the MP there. 

.. thumbnail:: /images/figures/curating_molecular_profiles_fig4.png

**Figure 4: Browse Molecular Profile functionality**

Another approach for a user or curator to locate MPs of interest is to use the Browse functionality (Figure 4), which can be used for all top level entities in CIViC including Molecular Profiles, found at the left of the user interface. If the user wants to see all MPs which contain a variant called V600E, then as in Figure 4, the user can type that into the Variants field, and all MPs containing a variant named V600E will be shown, and in this case all V600E variants are associated to the gene BRAF. Both simple and complex MPs are shown. Note if a user were interested in all MPs containing a bucket variant such as EGFR Mutation, then the user could type Mutation into the Variants field, and then EGFR into the Genes field, in order to narrow down the display to MPs containing only EGFR Mutation, instead of seeing all MPs containing the variant named Mutation associated to any gene.

On the gene page, the user can also choose a Variants tab (Figure 3), and see all of the variants associated to the gene, such as L858R or T790M for EGFR. Clicking on one of these will take the user to a variant page, and on the variant are listed variant related information such as coordinates, and also a list is shown with all simple and complex MPs that contain the variant.   

**Creation of new complex Molecular Profiles when adding Evidence Items**

All Evidence Items (EIDs) in CIViC are associated with either a simple or complex Molecular Profile (MP). When adding new Evidence Items to CIViC, the curator can choose either a simple MP or a complex MP in the Molecular Profile field of the Add Evidence Item Form (Figure 5). 

.. thumbnail:: /images/figures/curating_molecular_profiles_fig5.png

**Figure 5: Choosing to add an Evidence Item for a simple or complex Molecular Profile**

Adding a simple MP in the Add Evidence Form requires the curator to first specify a gene, and then specify a variant associated with that gene. As with simple MPs, new complex Molecular Profiles are added to CIViC during the process of adding the first EID specific to that complex MP.  The Process by which a new complex MP is created in the Add Evidence Form is outlined in the workflow figures below (Figure 6).

.. thumbnail:: /images/figures/curating_molecular_profiles_fig6.png
.. thumbnail:: /images/figures/curating_molecular_profiles_fig6b.png

**Figure 6: Workflow for creation of new complex Molecular Profiles in the Add Evidence Form**

