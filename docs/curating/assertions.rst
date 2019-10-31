Curating Assertions
===================
The CIViC Assertion (AID) functions as a summary of a body of evidence in the form of CIViC Evidence Items (EIDs) for a particular CIViC Variant. The Assertion also brings the unique function of incorporating information from practice guidelines (e.g. NCCN) and also integrating widely adopted clinical tiering systems (e.g. AMP-ASCO-CAP (`Li et al. 2017 <https://paperpile.com/c/hW1INu/jFZK>`__) and ACMG-AMP (`Richards et al. 2015 <https://paperpile.com/c/hW1INu/n8Pq>`__).

.. figure:: /images/figures/CIViC_assertion-summary-screenshot_overview_v1a.jpg
   :alt: Overview of an Assertion summary view

   Figure 1: The Assertion contains a brief one sentence summary and a longer Assertion Statement. It shows information on the CIViC Variant to which it applies. At the bottom section one sees the list of EIDs which support the Assertion. Selecting any supporting EID opens up that EID page

.. figure:: /images/figures/CIViC_assertion-fields_v1k.png
   :alt: Assertion fields

   Figure 2: Fields in the Assertion

The CIViC Assertion contains specific Variant Origin fields which are filled out during Assertion creation.

The Assertion contains a one sentence Assertion Statement which acts as a summary (“Non-small cell lung cancer with EGFR L858R mutation is sensitive to erlotinib or gefitinib” in Figure 1 above). 

For higher AMP-ASCO-CAP Tier (Li et al. 2017) Assertions, the more detailed Assertion Description section should list major practice guidelines and approvals associated with the Clinical Significance. For drug treatments this should contain recommended treatment line and cancer stage (e.g. “NCCN guidelines recommend (category 1) erlotinib and gefitinib for NSCLC with sensitizing *EGFR* mutations, along with afatinib and osimertinib.” in Figure 1)

.. figure:: /images/figures/CIViC_add-assertion-screenshot_v1.png
   :alt: Add Assertion form screenshot

   Figure 3: The Assertion Submission form is accessible by clicking the Add tab at the upper right corner of the user interface.

The CIViC Assertion is supported by Evidence Items (EIDs) for the Assertion Variant or related CIViC Variants. For instance, an Assertion on erlotinib sensitivity of *EGFR* L858R lung cancer may be supported by Evidence Items with the categorical CIViC Variant (sometimes colloquially called “bucket variant”) *EGFR* MUTATION. Note that if all of the supporting EIDs were of the categorical type, with no supporting EID specific to L858R, then an L858R Assertion would not be recommended.   

The Supporting Evidence grid allows users to associate Evidence Items with Assertions. This can be accomplished by filtering on the provided fields (e.g., EID, Gene, Variant) and selecting the yellow plus sign on the right. 

A sufficient amount of evidence should be added to an Assertion so that the collection of Evidence Items represents that state of the field for the disease, variant, and type of Evidence Statement.

As new evidence emerges which is relevant to a CIViC Variant which already has an accepted Assertion, then additional Evidence Items (EIDs) can be curated from this new evidence and added to the Supporting EIDs for the existing Assertion, potentially raising its ACMG classification or AMP Tier and Level.

All Evidence Items relevant to the Assertion should associated, even if they disagree with the Assertion Summary. Disagreements can be discussed in the Description section and rationale for discounting discrepant evidence should be recounted.


.. figure:: /images/figures/CIViC_assertion-types_v2a.png
   :alt: CIViC Assertion curation by Assertion Type

   Figure 4:  CIViC Assertion curation by Assertion type

CIViC Assertions summarize a collection of Evidence Items which reflect the state of literature for the given variant and disease. For Assertion Types typically associated with somatic variants (Predictive, Prognostic, or Diagnostic), AMP-ASCO-CAP 2017 guidelines are followed to associate the Assertion with an AMP Tier and Level, which involves consideration of practice guidelines as well as regulatory approvals associated with specific drugs, as well as consideration of available clinical evidence in the absence of explicit regulatory or practice guidelines. (Figure 4A)

CIViC Predisposing Assertions utilize ACMG-AMP 2015 guidelines to generate a 5-tier pathogenicity valuation for a variant in a given disease context, which is supported by a collection of CIViC Evidence Items, along with other data. ACMG evidence codes for an Assertion are supplied by a collection of supporting CIViC Evidence Items (e.g., PP1 from co-segregation data available in a specific publication), and additionally are derived from Variant data (e.g., PM2 from population databases such as gnomAD). ACMG evidence codes are then combined at the Assertion level to generate a disease-specific pathogenicity classification for the Assertion. (Figure 4B)

Assertions should should reflect the current state of practice guidelines and approvals:

- Practice guidelines, which are standard for the field from which the Assertion is derived, should be thoroughly consulted. Approved disease stage, and approved treatment lines should be outlined in the Assertion Description, if applicable.
- Approved companion diagnostics (e.g. Vysis Break-Apart Fish diagnostic for ALK-fusions) should be listed in the Assertion Description.
- Disease stage to which the assertion applies, as well as the line of treatment (e.g. first line, salvage, etc) should be made explicit in the Assertion Description. While the body of supporting Evidence Items may be derived from studies with differing patient populations with regard to stage and line of treatment, as well as preclinical studies in disease models, practice guidelines (e.g. NCCN etc) should be consulted for approved use cases.
- AMP Level and Tier (Li et al. 2017) should be associated with each Predictive, Diagnostic and Prognostic Assertion. For methods on assigning AMP-ASCO-CAP Tier / Level, See Figure 4A.
- Lower AMP-ASCO-CAP Tier Assertions can be written in the absence of practice guidelines, using Curator and Editor’s overviews of the field in order to assign the appropriate category. It is recommended to consult recent reviews in this case.
- All Evidence Items relevant to the Assertion should associated, even if they disagree with the Assertion Summary. Disagreements can be discussed in the Description section and rationale for discounting discrepant evidence should be recounted.
- Application of AMP-ASCO-CAP Tier and Level (Li et al. 2017) is dependant on practice guidelines (e.g. NCCN) ascribing prognostic value to the variant for the given disease, or failing this, the quality and level of evidence supporting the Assertion (Figure 4A).

Predictive Assertions
~~~~~~~~~~~~~~~~~~~~~
The Predictive Assertion screenshot below (Figure 5) describes that *BRAF* V600E confers sensitivity to combination therapy of dabrafenib and trametinib for patients with melanoma. The AMP-ASCO-CAP Category is Tier I - Level A for this CIViC Variant, Disease and Drug Sensitivity Assertion. This AMP-ASCO-CAP Tiering is a consequence of the presence of this variant and treatment in the Melanoma NCCN Guidelines (v2.2018).

.. figure:: /images/figures/CIViC_assertion-summary-AID7.png
   :alt: Screenshot of AID7, a predictive assertion

   Figure 5: Screenshot of a predictive Assertion, AID7. 

Curation Practices for Predictive Assertions
____________________________________________
All Evidence Items relevant to the Assertion should be associated, even if they disagree with the Assertion Summary. Disagreements can be discussed in the Description section and rationale for discounting discrepant evidence should be recounted.

AMP Level and Tier should be associated with each Predictive, Diagnostic and Prognostic Assertions [7]. For methods on assigning AMP-ASCO-CAP Tier / Level, See Figure 4A.

Practice guidelines, which are standard for the field from which the Assertion is derived, should be thoroughly consulted. Approved disease stage, and approved treatment lines should be outlined in the Assertion Description, if they are in place in guidelines. It is recommended to consult guidelines (e.g. NCCN) first, to allow them to structure creation of high Tier Assertions.

Lower AMP-ASCO-CAP Tier Assertions can be written in the absence of practice guidelines, using Curator and Editor’s overviews of the field. It is recommended to consult recent reviews in this case. 

Prognostic Assertions
~~~~~~~~~~~~~~~~~~~~~
Figure 6 shows a Prognostic Assertion with an exemplary Assertion Summary and Assertion Description. In this example, the Assertion describes that the *BRAF* V600E Variant confers poor outcome for patients with colorectal cancer. This variant has an associated FDA companion diagnostic test, is listed in the NCCN Guidelines for colorectal cancer (v2.2017), and falls under the Tier I - Level A AMP category.

.. figure:: /images/figures/CIViC_assertion-summary-AID20.png
   :alt: Screenshot of AID20, a prognostic assertion

   Figure 6: Screenshot of a prognostic Assertion, AID20. 

Curation Practices for Prognostic Assertions
____________________________________________
All Evidence Items relevant to the Assertion should associated, even if they disagree with the Assertion Summary. Disagreements can be discussed in the Description section and rationale for discounting discrepant evidence should be recounted.

Prognostic evidence in CIViC demonstrates variant association with better or worse patient outcome in a general manner, that is independent of any specific treatment context. Therefore, a larger collection of evidence showing similar prognostic outcomes under a range of different treatment or untreated regimes creates a stronger Prognostic Assertion.

Application of AMP-ASCO-CAP Tier and Level (Li et al. 2017) is dependant on practice guidelines (e.g. NCCN) ascribing prognostic value to the variant for the given disease, or failing this, the quality and level of evidence supporting the Assertion (Figure 4A).

Diagnostic Assertions
~~~~~~~~~~~~~~~~~~~~~
Figure 7 shows an example of a Diagnostic Assertion with an exemplary Assertion Summary and Assertion Description. In this example, the Assertion describes how an in-frame fusion between DNAJB1 and PRKACA can be used to diagnose a specific subtype of hepatocellular carcinoma (HCC). Presence of this fusion can be used to clarify that the patient has fibrolamellar HCC.

.. figure:: /images/figures/CIViC_assertion-summary-AID24.png
   :alt: Screenshot of AID24, a diagnostic assertion

   Figure 7: Screenshot of a diagnostic Assertion, AID24.

Curation Practices for Diagnostic Assertions
____________________________________________
All Evidence Items relevant to the Assertion should associated, even if they disagree with the Assertion Summary. Disagreements can be discussed in the Description section and rationale for discounting discrepant evidence should be recounted.

The evidence supporting the Assertion should sufficiently cover what is known regarding the diagnostic power for the variant in the specific disease context.

For Tier I Level A Diagnostic Assertions, details from relevant practice guidelines should be given, along with any additional specific information which is applicable (e.g., disease stage).  

Lower Tier and Evidence Level Assertions may be created for Diagnostic CIViC Variants not currently in practice guidelines. Variants backed by stronger clinical data may be Tier I Level B as above. Variants with smaller amounts of evidence for diagnostic potential will receive lower Tiers and Evidence Levels (Figure 4A).

Predisposing Assertions
~~~~~~~~~~~~~~~~~~~~~~~
Figure 8 shows an example of a Predisposing Assertion. In this example, an inframe deletion repeatedly observed in the literature is considered pathogenic for Von Hippel-Lindau Disease. Utilizing the ACMG guidelines [8], evidence codes were assembled from the literature (PP1, PS2) and Variant-level information (PM4, PM2) to be categorized as Pathogenic. Specific evidence is associated with codes in the Description and all evidence evaluated when producing the Assertion is associated with the Assertion.

.. figure:: /images/figures/CIViC_assertion-summary-AID17.png
   :alt: Screenshot of AID17, a predisposing assertion

   Figure 8: Screenshot of a predisposing Assertion, AID17. 

Curation Practices for Predisposing Assertions
______________________________________________
ACMG-AMP codes (Richards et al. 2015) supporting the Predisposing Assertion are derived from supporting Evidence Items, and other sources such as population databases (See Figure 4B). Any evidence codes applied should be explained in the Description section, allowing others to rapidly re-evaluate the evidence used.

All Evidence Items relevant to the Assertion should be associated, even if they disagree with the Assertion Summary. Disagreements can be discussed in the Description section and rationale for discounting discrepant evidence should be recounted.

Thoroughly evaluated Assertions can have a clinical significance of Variant of Unknown Significance using ACMG-AMP criteria. This permits other users to quickly re-evaluate this variant in the context of new evidence, potentially leading to reclassification, but reducing future curation burden if the variant is observed again.
