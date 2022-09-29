Curating Assertions
===================
The CIViC Assertion (AID) functions as a summary of clinical evidence for a variant, disease and specific predictive (therapeutic), prognostic, diagnostic or predisposing clinical significance supported by Evidence Items (EIDs) appearing in CIViC, along with evidence drawn from other sources, such as databases of variant population frequency. The Assertion is designed to incorporate information from practice guidelines (e.g., NCCN) and also integrates widely adopted clinical tiering systems into structured fields, including:

- AMP-ASCO-CAP guidelines (`Li et al. 2017 <https://pubmed.ncbi.nlm.nih.gov/27993330/>`__) for clinical tiering of somatic variants
- ClinGen/CGC/VICC SOP (`Horak et al. 2022 <https://pubmed.ncbi.nlm.nih.gov/35101336/>`__) for classification of somatic variant oncogenicity 
- ACMG-AMP guidelines (`Richards et al. 2015 <https://pubmed.ncbi.nlm.nih.gov/25741868/>`__) for classification of germline variant pathogenicity 

.. figure:: /images/figures/CIViC_assertion-summary-screenshot_overview_v1a.jpg
   :alt: Overview of an Assertion summary view

   Figure 1: The Assertion contains a brief one sentence summary and a longer Assertion Description. It also displays fields describing the CIViC Variant to which it applies. The bottom of the Assertion view shows a list of CIViC Evidence Items (EIDs) which support the Assertion. Selecting any supporting EID opens up that EID page.

.. figure:: /images/figures/CIViC_assertion-fields_v1k.png
   :alt: Assertion fields

   Figure 2: Fields in the Assertion

The Assertion contains a one sentence **Assertion Summary** which states the specific variant, disease, and clinical significance with drug if applicable (e.g. “Non-small cell lung cancer with EGFR L858R mutation is sensitive to erlotinib or gefitinib” in Figure 1 above). 

Beneath the Summary is the **Assertion Description**, which contains background clinical information specific to the variant, disease, and predictive (therapeutic), prognostic, diagnostic or predisposing clinical significance. EIDs supporting the Assertion clinical significance may be listed in this description, and referenced using CURIE identifiers (e.g., civic:EID1234). For Assertions with a higher AMP-ASCO-CAP Tier (Li et al. 2017), the Assertion Description section should list major practice guidelines and approvals associated with the clinical significance. For drug treatments, this may contain a brief restatement of guideline recommended treatment line and cancer stage (e.g. “NCCN guidelines recommend (category 1) erlotinib and gefitinib for NSCLC with sensitizing *EGFR* mutations, along with afatinib and osimertinib.” in Figure 1)

.. figure:: /images/figures/CIViC_add-assertion-screenshot_v1.png
   :alt: Add Assertion form screenshot

   Figure 3: The Assertion submission form is accessible by selecting the Add tab at the upper right corner of the user interface. All editable fields of the Assertion are available in this view. The supporting evidence grid at the bottom of the page allows users to associate Evidence Items (EIDs) with the Assertion, which is accomplished by filtering on the provided fields (e.g., EID, Gene, Variant) and selecting the yellow plus sign on the right. 

The CIViC Assertion is supported by CIViC Evidence Items (EIDs) which describe the same variant, disease and clinical significance as the given Assertion. The  Assertion may also be supported by EIDs written for a more generalized variant. For example an Assertion regarding erlotinib sensitivity of *EGFR* L858R lung cancer may be supported in part by EIDs written for a more general variant such as the *EGFR* Mutation categorical/bucket variant. Note that an Assertion for a specific variant such as *EGFR* L858R cannot be entirely supported by EIDs based on more general variant types such as Mutation, and requires some supporting EIDs of the same specific variant type. Similar principles apply to the Disease, where an Assertion for a specific disease type may in part be supported by EIDs for a more general disease class (e.g. Cancer, DOID 162). Note that cited guidelines should be disease specific.    

A sufficient amount of evidence should be added to an Assertion so that the collection of Evidence Items represents the 'state of the field' for the Disease, Variant, and Clinical Significance. As new evidence emerges which is relevant to a CIViC Variant with an accepted Assertion, then additional Evidence Items can be curated from this new evidence, and added to the Supporting EIDs for the existing Assertion, potentially raising its ACMG-AMP classification or AMP-ASCO-CAP Tier and Level.

.. figure:: /images/figures/CIViC_assertion-types_v2a.png
   :alt: CIViC Assertion curation by Assertion Type

   Figure 4:  CIViC Assertion curation by Assertion type

CIViC Assertions summarize a collection of Evidence Items, along with certain evidence drawn from sources other than publications or meeting abstracts, which together reflect the state of literature and clinical knowledge for the given variant and disease. For Assertion Types dealing with actionable clinical information, (Predictive/Therapeutic, Prognostic, or Diagnostic), AMP-ASCO-CAP 2017 guidelines are followed to associate the Assertion with an AMP Tier and Level. For the highest tier Assertions, this involves consideration of practice guidelines as well as regulatory approvals for drug use in the specific context of the variant and disease. In the absence of explicit regulatory or practice guidelines, the supporting clinical and case study Evidence Items should be used to guide application of AMP Tier and Level (Figure 4A). 

Lower AMP-ASCO-CAP Tier Assertions can be written for variants that are not supported by practice guidelines or extensive clinical evidence, relying on case study or preclinical data. The supporting EIDs should reflect the state of the field regarding the emerging knowledge in such cases, and AMP Tier should be assigned based on the curator and editor’s overviews of the field. It is recommended to consult recent reviews in this case.

CIViC Predisposing Assertions utilize ACMG-AMP 2015 guidelines to generate a 5-tier pathogenicity valuation for a variant in a given disease context, which is supported by a collection of CIViC Evidence Items, along with other data. ACMG evidence codes for an Assertion are supplied by a collection of supporting CIViC Evidence Items (e.g., PP1 from co-segregation data available in a specific publication), and additionally are derived from Variant data (e.g., PM2 from population databases such as gnomAD). ACMG evidence codes are then combined at the Assertion level to generate a disease-specific pathogenicity classification for the Assertion (Figure 4B and Figure 8).

Other guidelines that curators should keep in mind include:
- While the body of supporting Evidence Items may be derived from studies with differing patient populations with regard to stage and line of treatment, as well as preclinical studies in disease models, the Assertion may describe more specific disease context based on reading of practice guidelines (e.g. NCCN etc), and any such descriptions added to the Assertion must explicitly cite the practice guidelines as the source. 
- Generally, practice guidelines may be summarized in the Assertion description, including disease stage to which the assertion applies, as well as the line of treatment (e.g., first line, salvage), but this information should be clearly labeled as being derived from published guidelines, and those guidelines explicitly cited. 
- Approved companion diagnostics (e.g. Vysis Break-Apart Fish diagnostic for ALK-fusions) may be listed in the Assertion Description.
- All Evidence Items relevant to the Assertion should be associated to it, even if they disagree with the Assertion Summary. Disagreements can be discussed in the Assertion Description section and the rationale for discounting discrepant evidence should be recounted.
- The CIViC Assertion contains specific Variant Origin fields which are filled out during Assertion creation. It is possible for some EIDs in the supporting evidence to have a different Variant Origin than that in the Assertion, but the Assertion should contain substantial support from Evidence Items with the same Variant Origin as in the Assertion.  

Predictive Assertions
~~~~~~~~~~~~~~~~~~~~~
The Predictive Assertion screenshot below (Figure 5) describes that *BRAF* V600E confers sensitivity to combination therapy of dabrafenib and trametinib for patients with melanoma. The AMP-ASCO-CAP Category is Tier I - Level A for this variant, disease and drug sensitivity assertion. The high AMP-ASCO-CAP Tier is a consequence of the presence of this variant and treatment in the Melanoma NCCN Guidelines (v2.2018).

.. figure:: /images/figures/CIViC_assertion-summary-AID7.png
   :alt: Screenshot of AID7, a predictive assertion

   Figure 5: Screenshot of a predictive Assertion, AID7. 

Curation Practices for Predictive Assertions
____________________________________________

Predictive Assertions are generally associated with somatic variants. Some germline variants may have pharmacogenomic properties that predict an adverse response to a treatment. In these cases, Predictive Evidence Items and an Assertion can be created with the Clinical Significance being Supports Adverse Response.



Prognostic Assertions
~~~~~~~~~~~~~~~~~~~~~
Figure 6 shows a Prognostic Assertion with an exemplary Assertion Summary and Assertion Description. In this example, the Assertion describes that the *BRAF* V600E Variant confers poor outcome for patients with colorectal cancer. This variant has an associated FDA companion diagnostic test, is listed in the NCCN Guidelines for colorectal cancer (v2.2017), and falls under the Tier I - Level A AMP category.

.. figure:: /images/figures/CIViC_assertion-summary-AID20.png
   :alt: Screenshot of AID20, a prognostic assertion

   Figure 6: Screenshot of a prognostic Assertion, AID20. 

Curation Practices for Prognostic Assertions
____________________________________________
Prognostic Evidence Items in CIViC describe a variant being associated with better or worse patient outcome in a general manner, independent of any specific treatment. Evidence should show better or worse outcome in the presence of the variant, ideally under different treatment regimes and also in untreated cases if such data is available. Therefore, a larger collection of evidence showing similar prognostic outcomes under a range of different treatment or untreated regimes creates a stronger Prognostic Assertion.


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


Oncogenic Assertion
~~~~~~~~~~~~~~~~~~~
The Oncogenic Assertion (Oncogenic AID) summarizes a collection of Evidence Items (EIDs) for a somatic variant, which together should reflect the state of knowledge in the field for this variant to reach a final oncogenic or benign classification. Oncogenic properties are interpreted as variant induced effects which promote one or more of the `Hallmarks of Cancer <https://pubmed.ncbi.nlm.nih.gov/21376230/>`__. Benign properties indicate a lack of oncogenic effect for a somatic variant, which ideally will be demonstrated in the context of well defined positive controls. This collection of EIDs can then be summarized into a CIViC Oncogenic Assertion (Figure 9). 


.. figure:: /images/figures/oncogenicity-codes.png
   :alt: Oncogenicity Codes classify a variant using a 5 tier evaluation.

   Figure 9: Oncogenicity Codes from the ClinGen/CGC/VICC Guidelines may be used to classify a variant using a 5-tier evaluation consisting of Benign, Likely Benign, Variant of Unknown Significance (VUS), Likely Oncogenic, or Oncogenic (Figure 10)

.. figure:: /images/figures/oncogenic-clin-sig-scores.png
   :alt: Oncogenic Assertion Clinical Significance Classifications based on score.

   Figure 10: Oncogenic Assertion Clinical Significance Classifications based on score.

The selection of Assertion Type in CIViC results in a particular choice of variant classification based on the aggregation of evidence codes (Figure 11). For Oncogenic Assertions, after the Oncogenic AID Type is chosen, the ClinGen/CGC/VICC `Oncogenicity Codes <https://pubmed.ncbi.nlm.nih.gov/35101336/>`__. can be added to the Assertion (Figure 12). In some cases, ClinGen Somatic Variant Curation Expert Panels (SC-VCEPs) may choose N/A as an evidence code, and instead utilize an SC-VCEP specific protocol for evaluation of oncogenicity. This protocol should be described in the Assertion Summary. 

.. figure:: /images/figures/assertion-code-guidelines.png
   :alt: Five Assertion types are available which are associated with different guidelines.

   Figure 11: Five Assertion types are available. AMP/ASCO/CAP Guidelines are used for tiering Predictive, Diagnostic, and Prognostic Assertions. Predisposing Assertions utilize the ACMG/AMP Guidelines. Oncogenic Assertions incorporate the ClinGen/CGC/VICC Guidelines, and users may also choose the special N/A evidence code, and then utilize an approved alternate oncogenicity guideline for Assertion creation. 

.. figure:: /images/figures/oncogenic-clingen-guidelines.png
   :alt: Oncogenic Assertions utilize the ClinGen/CGC/VICC 2022 Guideline.

   Figure 12: When curating Oncogenic Assertions utilizing the ClinGen/CGC/VICC 2022 Guideline, a menu of ClinGen/CGC/VICC Codes are made available in a menu from which the curator may choose one or more.

Curation of Oncogenic Assertions requires a brief Summary of the main conclusion of the Assertion. In the Assertion Description the curator should describe general relevant information about the variant’s oncogenic or benign properties, and importantly, describe how the appropriate guideline was used to arrive at the Clinical Significance, which is Likely Benign in the example below (Figure 13). Additionally external information such as population frequencies or data contradictions can be described here. The ClinGen/CGC/VICC Codes are added by the curator in the Add Assertion form, and a brief explanation for each Code used is given in the Assertion Description. For Codes that are derived from Evidence Items, the appropriate Curie link is also added by the curator (e.g. civic.EID:10277). The Disease field is required, and the term Cancer (DOID 162) may be used when the underlying evidence applies more generally. 

.. figure:: /images/figures/oncogenic-assertion.png
   :alt: Example Oncogenic Assertion.

   Figure 13: Example Oncogenic Assertion.

Curators should take note that the Clinical Significance of the Oncogenic Assertion (AID) and that of the Oncogenic Evidence Item (EID) do not overlap and instead consist of partially related but different annotations (Figure 14). This also holds for the Predisposing Evidence Item versus the Predisposing Assertion. EIDs provide discrete evidence from a single source and do not represent a final classification, only supporting evidence. The Assertion Clinical Significance provides a final classification as a result of the aggregation of information across studies for the variant (i.e., multiple EIDs and other evidence). The Oncogenic EID is set up on two opposing axes describing Protectiveness and Oncogenicity. The Oncogenic Axis is able to capture evidence supporting either a benign or an oncogenic effect for the variant, but only in rare cases will a single publication or meeting abstract yield enough evidence to obtain a classification of Oncogenic or Benign utilizing the `ClinGen/CGC/VICC Guidelines <https://pubmed.ncbi.nlm.nih.gov/35101336/>`__.. Because of this, Single EIDs are tagged with Oncogenicity Codes when appropriate, and used to support an overall Assertion (Figure 9). Importantly, note that an Oncogenic EID that utilizes the Protective Clinical Significance will have no analog at the level of Assertion.

.. figure:: /images/figures/oncogenic-evidence-vs-assertion.png
   :alt: Oncogenic Evidence in contrast to the Oncogenic Assertion.

Figure 14: Oncogenic Evidence in contrast to the Oncogenic Assertion.

