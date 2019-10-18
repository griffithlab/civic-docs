Curating Assertions
===================
The CIViC Assertion (AID) functions as a summary of a body of evidence in the form of CIViC Evidence Items (EIDs) for a particular CIViC Variant. The Assertion also brings the unique function of incorporating information from practice guidelines (e.g. NCCN) and also integrating widely adopted clinical tiering systems (e.g. AMP-ASCO-CAP (`Li et al. 2017 <https://paperpile.com/c/hW1INu/jFZK>`__) and ACMG-AMP (`Richards et al. 2015 <https://paperpile.com/c/hW1INu/n8Pq>`__).

.. figure:: /images/figures/CIViC_assertion-summary-screenshot_overview_v1a.png
   :alt: Overview of an Assertion summary view

   Figure 1: The Assertion contains a brief one sentence summary and a longer Assertion Statement. It shows information on the CIViC Variant to which it applies. At the bottom section one sees the list of EIDs which support the Assertion. Selecting any supporting EID opens up that EID page

.. figure:: /images/figures/CIViC_assertion-fields_v1k.png
   :alt: Assertion fields
   Figure 2: Fields in the Assertion

The CIViC Assertion contains specific Variant Origin fields which are filled out during Assertion creation.

The Assertion contains a one sentence Assertion Statement which acts as a summary (“Non-small cell lung cancer with EGFR L858R mutation is sensitive to erlotinib or gefitinib” in Figure 1 above). 

For higher AMP-ASCO-CAP Tier (Li et al. 2017) Assertions, the more detailed Assertion Description section should list major practice guidelines and approvals associated with the Clinical Significance. For drug treatments this should contain recommended treatment line and cancer stage (e.g. “NCCN guidelines recommend (category 1) erlotinib and gefitinib for NSCLC with sensitizing EGFR mutations, along with afatinib and osimertinib.” in Figure 1)

.. figure:: /images/figures/CIViC_assertion-fields_v1k.png
   :alt: Screenshot of Assertion submission form
   Figure 3: The Assertion submission form is accessible by clicking the Add tab at the upper right corner of the user interface.

The CIViC Assertion is supported by EIDs for the Assertion Variant or related CIViC Variants. For instance, an Assertion on erlotinib sensitivity of EGFR L858R lung cancer may be supported by Evidence Items with the categorical CIViC Variant (sometimes colloquially called “bucket variant”) EGFR MUTATION. Note that if all of the supporting EIDs were of the categorical type, with no supporting EID specific to L858R, then an L858R Assertion would not be recommended.

The Supporting Evidence grid allows users to associate Evidence Items with Assertions. This can be accomplished by filtering on the provided fields (e.g., EID, Gene, Variant) and selecting the yellow plus sign on the right. 

A sufficient amount of evidence should be added to an Assertion so that the collection of Evidence Items represents that state of the field for the disease, variant, and type of Evidence Statement.

As new evidence emerges which is relevant to a CIViC Variant which already has an accepted Assertion, then additional EIDs can be curated from this new evidence and added to the Supporting EIDs for the existing Assertion, potentially raising its ACMG classification or AMP Tier and Level.

All Evidence Items relevant to the Assertion should associated, even if they disagree with the Assertion Summary. Disagreements can be discussed in the Description section and rationale for discounting discrepant evidence should be recounted.

.. figure:: /images/figures/CIViC_add-assertion-form_screenshot.png
   :alt: Add Assertion form screenshot

   Figure 3: The Assertion Submission form is accessible by clicking the Add tab at the upper right corner of the user interface.

The CIViC Assertion is supported by Evidence Items (EIDs) for the Assertion Variant or related CIViC Variants. For instance, an Assertion on erlotinib sensitivity of EGFR L858R lung cancer may be supported by Evidence Items with the categorical CIViC Variant (sometimes colloquially called “bucket variant”) EGFR MUTATION. Note that if all of the supporting EIDs were of the categorical type, with no supporting EID specific to L858R, then an L858R Assertion would not be recommended.   

The Supporting Evidence grid allows users to associate Evidence Items with Assertions. This can be accomplished by filtering on the provided fields (e.g., EID, Gene, Variant) and selecting the yellow plus sign on the right. 

A sufficient amount of evidence should be added to an Assertion so that the collection of Evidence Items represents that state of the field for the disease, variant, and type of Evidence Statement.

As new evidence emerges which is relevant to a CIViC Variant which already has an accepted Assertion, then additional Evidence Items (EIDs) can be curated from this new evidence and added to the Supporting EIDs for the existing Assertion, potentially raising its ACMG classification or AMP Tier and Level.

All Evidence Items relevant to the Assertion should associated, even if they disagree with the Assertion Summary. Disagreements can be discussed in the Description section and rationale for discounting discrepant evidence should be recounted.

