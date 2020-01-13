.. _curating-evidence:

Curating Evidence
=================
Evidence Items (EIDs) form the fundamental unit of the CIViC knowledgebase. EIDs derive structured clinical statements from peer reviewed publications and ASCO abstracts, which act as evidence sources for Evidence Items. The EID links back to its source. EIDs are hand-curated units of knowledge, and one evidence source may supply enough data to create multiple EIDs. EIDs are displayed throughout the CIViC application, for example as a summary (Figure 1) and as a data table row (Figure 3).

.. figure:: /images/figures/evidence-summary_EID6568.png
   :alt: Screenshot of an evidence item summary

   Figure 1: Screenshot of an evidence item summary

CIViC Evidence is added and curated via a moderation process that includes submitting, evaluating, accepting (or rejecting), and suggesting changes (Figure 2). CIViC Curators may add or suggest revisions to curated content at each step. Adding content involves submitting new Evidence Items or Assertions that subsequently undergo revision and review by CIViC Editors. Revision of content involves adding or revising the clinical summary and/or its associated features. Once changes are made within the CIViC database, the additions/revisions become visible directly or on a separate revision page depending on the type of submission. Curation is listed as a "submitted" (i.e., pending) until it is accepted by an Editor, who are given power to accept or reject Curator submissions. Curators may reject (but not accept) their own submissions/revisions.

.. figure:: /images/figures/CIViC_adding-updating-evidence_v2a.png
   :alt: Overview of CIViC content creation process

   Figure 2: Overview of CIViC content creation process

It is important to note that once evidence is submitted into CIViC as a new Evidence Item, then the EID is visible to the community in the unmoderated/non-reviewed state, and these EIDs are labeled in orange (Figure 3). This enables the public to comment or create moderations on the submitted evidence. It is also important to note that orange Evidence Items may be incomplete, not accurately fit into the CIViC data model, or contain problems which the moderation process is designed to capture and fix. Once a CIViC EID has been reviewed by editors, and all revisions reviewed and accepted, then the EID is accepted by an editor, and becomes labeled green.

.. figure:: /images/figures/CIViC_evidence-grid-features_v1d.png
   :alt: Evidence Item datagrid features

   Figure 3: Evidence Item datagrid features

When an Evidence Item has a pending revision, then it is labeled with a blue exclamation mark icon (Figure 3). Note that revisions can be made to EIDs in both the Submitted/Unreviewed Status (orange) and the Accepted/Fully Reviewed Status (green).

.. _curating-evidence-general:

General Evidence Item Curation Practices
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Evidence Items should generally be prepared from primary literature rather than from review articles. It is recommended that curators use reviews to identify primary literature referenced in the review and to curate individual Evidence Items based on these cited articles. Review articles can also be used to develop Gene and Variant summaries.

When curating new evidence, the curator should review the existing evidence already curated into CIViC for that Variant to look for the following issues:

- For clinical trials and case reports (Levels A, B, and C), overlapping patient populations (i.e. the same patient treatment and outcome described in multiple reports) should be avoided, or carefully noted to alert users of this nuance and avoid conclusions that mistake these studies as independent. Note also that reports describing different phases of the same patient treatment (i.e. erlotinib and subsequently afatinib), or different clinically relevant conclusions (i.e. predictive evidence and simultaneous diagnostic evidence) are independent/non-overlapping entities.

- For Predisposing EIDs describing germline variants, the same patient may appear in multiple studies. Curators should be careful to note these cases by reviewing existing germline EIDs for the same variant in CIViC. 

Disease stage, prior treatments, and other experimental details influencing evidence interpretation should be captured within an Evidence Item to maximize user comprehension of the underlying study and the appropriate context in which it is relevant. Such details are critical parts of clinical guidelines and can impact which clinical guidelines should be used as well as drug sensitivities (see `EID1008 <https://civicdb.org/links/evidence/1008>`__ and `EID1009 <https://civicdb.org/links/evidence/1009>`__).

Five types of EID exist in CIViC (Figure 4), giving structured clinical annotation to a Variant. Three types of clinical statements, Predictive/Therapeutic, Prognostic and Diagnostic, are usually associated with somatic variants, while Predisposing evidence is generally linked to germline variation. Functional studies are often performed in vitro, so associated EIDs will have the Unknown field selected for Variant Origin.

.. figure:: /images/figures/CIViC_evidence-item-primary-fields_v3a.png
   :alt: Structured annotation comprising the five types of CIViC Evidence Item

   Figure 4: Structured annotation comprising the five types of CIViC Evidence Item


Predictive Evidence
~~~~~~~~~~~~~~~~~~~
Predictive/Therapeutic Evidence Items (EIDs) are structured to capture variant annotation for drug sensitivity, resistance,  

Below is an example of an EID that illustrates the Predictive Evidence Type. This example describes the CLEOPATRA trial (NCT00567190), which evaluated 808 patients with *HER2*-positive metastatic breast cancer. These patients demonstrated significant sensitivity/response when treated with combination therapy of docetaxel, pertuzumab and trastuzumab.


.. figure:: /images/figures/evidence-summary_EID1077.png
   :alt: Screenshot of a predictive Evidence Item summary

   Figure 5: Screenshot of a predictive Evidence Item summary

Predictive Evidence Curation Practices
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Predictive Evidence Items should include the Drug Name(s) and Drug Interaction Type (for multiple drugs). 

The most current name of the Drug (excluding trade names) should be used in the Drug field to reduce duplication. The Evidence Statement should contain the drug name used in the study with the current name in brackets, when applicable.

Drug Interaction Types are required anytime more than one drug is mentioned for a given study. If multiple drug interaction types are at play (e.g., combinations and substitutes), considering separating these concepts into more than one Evidence Item.

If applicable, the Clinical Trial name and ID should be included in the Evidence Statement. Any clinical trial IDs available in PubMed for the Source linked to this Evidence Item will be automatically imported and linked to this Evidence Item when the PubMed Source is imported into CIViC.

The duration of exposure to the drug and confounding interactions (e.g., wash-out periods, previous treatment, cancer stage) should be listed.

Assigning a Clinical Significance of Sensitivity/Response can depend on factors such as response rate, which will vary significantly with disease and treatment. In some cases a response rate of 15% may represent a significant improvement, and merit a valuation of Sensitivity/Response. A general guideline for CIViC curation is to follow the author’s published (and peer-reviewed) interpretations and conclusions of the results.

Extensive guidelines, use cases, and examples for curation of predictive evidence are given in Figure 7 and Table 1.

Diagnostic Evidence
~~~~~~~~~~~~~~~~~~~
Below is an example of an EID that illustrates the Diagnostic Evidence Type. This example describes the World Health Organization guidelines for classifying chronic myelomonocytic leukemia (CMML). Specifically, if a patient has a PCM1-JAK2 fusion or a rearrangement involving PDGFRA, PDGFRB, or FGFR1, especially in the setting of eosinophilia, the patient does not have CMML.

.. figure:: /images/figures/evidence-summary_EID1077.png
   :alt: Screenshot of a diagnostic Evidence Item summary

   Figure 6: Screenshot of a diagnostic Evidence Item summary

Diagnostic Evidence Curation Practice
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Diagnostic Evidence Items should only be used if the variant assists in labeling the patient with a specific disease or disease subtype and should not be used to denote that the particular variant is prevalent in a specific disease.

Generally, Diagnostic Evidence Items describe variants that can help accurately diagnose a cancer type or subtype with high sensitivity and specificity, for which diagnoses may otherwise be challenging.

Diagnostic Evidence Items are very closely tied to the terms of the Disease Ontology (DO) in CIViC. The Disease Ontology works to actively generate mappings to other highly used ontologies, but the terms in the DO are generally accepted diseases which are part of medical practice. Therefore, literature proposing a novel disease type - for instance studies suggesting a novel cancer subtype defined by the presence of a specific oncogenic variant - are not generally admitted as part of the CIViC data model. Alternatively, if a curator with expertise in the field feels that the novel subtype has met with a sufficient level of acceptance, they may submit this type of Evidence Item using a non-DO term, and suggest that DO admit this term into the ontology.

Literature describing diagnostic practice guidelines (such as those of the World Health Organization) may be used in curation and submitted as A-level Evidence Items.

Literature describing small numbers of observations in patient samples of a certain variant, where the authors state that the variant may have diagnostic value, may be admitted as lower star Case Study (C-level) data. Similar literature employing larger numbers could be labeled as Clinical (B-level).

Guidelines and use cases for curation of diagnostic evidence are given in Table 1.

Prognostic Evidence
~~~~~~~~~~~~~~~~~~~
Below is an example of an Evidence Item that describes a Prognostic Evidence Type. This example describes a 406-patient trial whereby observation of any somatic TP53 mutation in chronic lymphoblastic leukemia conferred poor prognosis relative to wildtype TP53.

.. figure:: /images/figures/evidence-summary_EID1507.png
   :alt: Screenshot of a prognostic Evidence Item summary

   Figure 7: Screenshot of a prognostic Evidence Item summary

Prognostic Evidence Curation Practice
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Prognostic Evidence Items should include the measured outcome (e.g., overall survival, complete response, partial response), number of subjects and applicable statistics.

If described in the literature, a definition of the measured outcome should be given.

Prognostic evidence is characterized by either better outcomes for patient subpopulations with the given variant, which are not specific to any particular treatment context, or worse outcomes which are not indicative of variant resistance to a specific treatment. Instead, the change in outcome should be largely correlated to the presence of the variant.

In some cases, a variant subpopulation with worse outcome may benefit from subsequent therapy targeted to that variant (e.g., *HER2* amplification in breast cancer).

Guidelines, use cases, and examples for curation of prognostic evidence are given in Figure 7 and Table 1.

Curation Scenarios
~~~~~~~~~~~~~~~~~~
The table below (Table 1) gives an in depth set of cases for assigning the Clinical Significance to an Evidence Item (EID) where either the "supports" or "does not support" Evidence Direction is used in combination with a Predictive/Therapeutic, Diagnostic or Prognostic Clinical Significance annotation.

Note that "Reduced Sensitivity" Clinical Significance is used to compare the variant of interest to a known, sensitizing variant. It is not used to compare the efficacy of one drug for a variant against a different drug for the same variant. In the latter case, the curator may simply make a Predictive evidence item with independently evaluates the efficacy of the drug against the variant of interest. 

The "Sensitivity/Response" annotation is used to assess sensitizing variants, which are usually in the form of a primary sensitizing somatic mutation (e.g SNV, amplification, deletion, etc).

The "Resistance" annotation is used in situations where the variant of interest has been observed to induce resistance in a context where, in the absence of the variant, the system being assayed would be deemed sensitive which induce resistance to treatment (e.g. T790M mutation in cis with a  background variant of *EGFR* L858R). In cases where a variant fails to induce sensitivity, then that variant is best annotated with "Does not Support Sensitivity".       

.. figure:: /images/figures/CIViC_attributes-curation-table_thumbnail_v1b.png
   :alt: Use cases for curation of Predictive, Diagnostic and Prognostic Evidence Items with different Evidence Direction, and in different contexts including primary and secondary mutations

   Table 1: Use cases for curation of Predictive, Diagnostic and Prognostic Evidence Items with different Evidence Direction, and in different contexts including primary and secondary mutations. :download:`Download a more readable PDF version here <../images/figures/CIViC_attributes-curation-table_v1b.pdf>`

Both Predictive and Prognostic evidence types may be obtained from the same data set in some cases. Figure 8, displayed below, gives hypothetical examples of predictive and prognostic structured annotation derived from patient data.

.. figure:: /images/figures/CIViC_interpreting-predictive-prognostic-clinical-trials_v1d.png
   :alt: Examples for deriving Predictive and Prognostic Evidence Items (EIDs) from hypothetical clinical trial data.

   Figure 8: Examples for deriving Predictive and Prognostic Evidence Items from hypothetical clinical trial data.

Predisposing Evidence Type
~~~~~~~~~~~~~~~~~~~~~~~~~~
Predisposing Evidence Items are designed to capture clinical information associated with germline variants relevant for cancer. This EID type is closely associated with `ACMG Codes. <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4544753/>`__ The general format for a predisposing EID is a summary of the reported data relevant to the variant and disease of interest, followed by an enumeration of ACMG Codes derived from the reported information, which a brief justification for the presence of each code. 

Below is an example of an Evidence Item (`EID5546 <https://civicdb.org/events/genes/58/summary/variants/1810/summary/evidence/5134/summary#evidence>`__) that describes a Predisposing Evidence Type. This example describes a study where the VHL - R167Q (c.500G>A) Variant was described in a set of patients and evidence for the PP1 ACMG-AMP criteria was documented. Hemangioblastoma and pheochromocytoma were seen in patients and are reported as Associated Phenotypes, while the Disease is Von Hippel-Lindau Disease.

.. figure:: /images/figures/evidence-summary_EID5546.png
   :alt: Screenshot of a predisposing Evidence Item summary

   Figure 6: Screenshot of a predisposing Evidence Item summary

Predisposing Curation Practices
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Typically, but not always, Predisposing Evidence Items are written for rare or common germline variants. In rare circumstances, the patient can have a predisposing variant that develops as a result of a somatic mutation or mosaicism during embryogenesis that is widespread but not necessarily heritable.

ACMG-AMP evidence codes (Richards et al. 2015) (ACMG criteria) are derived from the evidence presented in the specific Source and are listed at the end of the Evidence Statement with a brief justification for each code’s use.
ACMG evidence codes not directly derived from Source associated with the Evidence Item (e.g. population databases for PM2) are captured at the Variant Summary or at the level of Assertion.

The above Predisposing Evidence Item (EID) lists the ACMG code PP1 as derived from the literature source, which alone results in a ACMG-AMP classification of VUS. Therefore, this Evidence Item is combined with other VHL - R167Q (c.500G>A) Evidence Items for Von Hippel Lindau Disease, in order to create CIViC Assertions, where the ACMG codes from the different Evidence Items are combined and evaluated for pathogenicity. The EID depicted here is part of Assertion number 4 (AID4), where the Evidence Items combine to pathogenic. Therefore Predisposing Evidence Items are not given Clinical Significance or Evidence Direction in isolation, and these fields are labeled N/A.

In some instances, a publication will contain relevant germline variant evidence for curation into CIViC and EID creation, but that evidence will not be sufficient to fulfill any of the ACMG criteria (especially in some cases where the gene or disease-specific criteria may be more stringent). In this case Curators should indicate this at the end of the Evidence Statement, by adding a brief statement such as “No ACMG criteria met”, in order to indicate to Editors and future Users that the evidence had been analyzed for the presence of ACMG codes during the curation process.

Functional Evidence Type
~~~~~~~~~~~~~~~~~~~~~~~~
Below is an example of an Evidence Item that describes a Functional Evidence Type. This example summarizes the impact of a novel *KIAA1549-BRAF* fusion event on the function of the *BRAF* protein. Specifically, the fusion product showed gain of function activity in cell lines relative to wildtype kinase. This activity was also demonstrated to be comparable to a known gain of function variant, *BRAF V600E*.

.. figure:: /images/figures/evidence-summary_EID7337.png
   :alt: Screenshot of a functional Evidence Item summary

   Figure 7: Screenshot of a functional Evidence Item summary

Functional Curation Practices
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Functional Evidence Items should describe how the variant alters biological function from the reference state. This can include a change in function or lack of change in function.

Clinical Significance for Functional Evidence Types adhere to the following rules:

.. list-table::
   :widths: 20 80
   :header-rows: 0

   * - Gain of Function
     - A variant whereby new/enhanced function is conferred on the gene product
   * - Loss of Function
     - A variant whereby the gene product has diminished or abolished function
   * - Unaltered Function
     - A variant whereby the function of the gene product is unchanged
   * - Neomorphic
     - A variant whereby the function of the gene product is a new function relative to the wildtype function
   * - Dominant Negative
     - A variant whereby the function of a wildtype allele gene product is abrogated by the gene product of the allele with the variant
   * - Unknown
     - A variant that cannot be precisely defined by gain-of-function, loss-of-function, or unaltered function.

Functional Evidence Items may be used to support certain ACMG codes (e.g. PM1). In these cases, the ACMG code should be listed in the Evidence Statement along with a brief justification for its inclusion.

In some cases, Functional Evidence Items may appear as supporting evidence for a Predisposing Assertion, for instance in support of a PM1 evidence code.

.. rubric:: Functional Evidence from Clinical Trials

When curating evidence obtained from clinical trials on performed with groups of patients, where data is pooled by mutation type (e.g. *EGFR* MUTATION), Level B clinical results may be obtained, which may report a statistically significant difference on a clinically relevant parameter such as partial response (PR) between wildtype vs. mutant patients. In addition, the publication may sometimes give outcomes on important individual patient parameters, such as variant, age, sex, best response, overall survival, etc. In these cases, this aggregate of data may be integrated into multiple Evidence Items in the following manner (THe figure below is loosely based on a data set in CIViC obtained from PMID:21531810, which can be seen in CIViC on `its Evidence Source page <https://civicdb.org/sources/1503/summary>`__).

.. figure:: /images/figures/clinical-evidence-extraction_FPO.png
   :alt: Obtaining Clinical and Case Study Evidence Items from clinical trial reports

   Figure 7: Obtaining Clinical and Case Study Evidence Items from clinical trial reports

Statistical results may be obtained from the study to annotate a Categorical (sometimes colloquially called bucket-type) CIViC Variant, which pools together a category of sequence variants (for example *EGFR* MUTATION). Significantly longer progression free survival (PFS) may be observed in the mutant group (grouped under the Categorical CIViC Variant) vs. the wildtype group, when given a certain drug. In this case, this result may be reported in a CIViC Level B Evidence Item under the CIViC Categorical Variant *EGFR* MUTATION, with Evidence Direction and Clinical Significance “Suggests Sensitivity/Response” to the drug used.

When a sufficient level of individual patient detail is present, including the individual patient variants along with an important clinical parameter such as their best response, then this data set can be used to generate a set of CIViC Level C Evidence Items for the patients, each one associated with the respective CIViC Variant that was observed in the individual patient, along with the outcome. Note that even if the entire group showed statistically significant improvement with the Categorial Variant, this does not mean every patient did better, e.g. if a patient with variant X123Y had progressive disease as best response, then this would result in a Level C EID with Evidence Direction and Clinical Significane of “Does not support Sensitivity” for the CIViC Variant X123Y. 
