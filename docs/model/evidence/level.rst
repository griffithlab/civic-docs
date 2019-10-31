.. _evidence-level:

Level
==============

Understanding Levels
--------------------
The evidence level describes the robustness of the study supporting the evidence item. Five different evidence levels are supported: “A - Validated association”, “B - Clinical evidence”, “C - Case study”, “D - Preclinical evidence”, and “E - Inferential association”. Evidence items with validated associations (A) have a proven or clinical consensus on the variant association in human medicine. Typically these evidence items describe Phase III clinical trials or have associated companion diagnostics. Clinical evidence (B) are typically large clinical trials or other primary patient data supporting the clinical association. These evidence items usually include more than 5 patients supporting the claim made in the evidence statement. Case studies (C) are individual case reports from clinical journals. Preclinical evidence (D) is derived from in vivo or in vitro experiments (e.g., cell lines or mouse models) that support clinical claims. Finally, inferential associations (E) indirectly associate the variant to the provided clinical evidence.

.. role:: green

.. role:: blue

.. role:: purple

.. role:: orange

.. role:: red

.. list-table::
   :widths: 5 15 20 60
   :header-rows: 1

   * - Level
     - Name
     - Definition
     - Example and further comments
   * - :green:`A`
     - :green:`Validated association`
     - Proven/consensus association in human medicine.
     - *"AML with mutated NPM1" is a provisional entity in WHO classification of acute
       myeloid leukemia (AML). This mutation should be tested for in
       clinical trials and is recommended for testing in patients with
       cytogenetically normal AML.* Validated associations are often in
       routine clinical practice already or are the subject of major
       clinical trial efforts.
   * - :blue:`B`
     - :blue:`Clinical evidence`
     - Clinical trial or other primary patient data
       supports association.
     - *BRAF V600E is correlated with poor
       prognosis in papillary thyroid cancer in a study of 187 patients
       with PTC and other thyroid diseases.* The evidence should be
       supported by observations in multiple patients. Additional support
       from functional data is desirable but not required.
   * - :purple:`C`
     - :purple:`Case study`
     - Individual case reports from clinical journals.
     - *A single patient with FLT3 over-expression responded to the FLT3
       inhibitor sunitinib.* The study may have involved a large number of
       patients, but the statement was supported by only a single
       patient. In some cases, observations from just a handful of
       patients (e.g. 2-3) or a single family may also be considered a
       case study/report.
   * - :orange:`D`
     - :orange:`Preclinical evidence`
     - In vivo or in vitro models support association.
     - *Experiments showed that AG1296 is effective in
       triggering apoptosis in cells with the FLT3 internal tandem
       duplication.* The study may have involved some patient data, but
       support for this statement was limited to in vivo or in vitro
       models (e.g. mouse studies, cell lines, molecular assays, etc.).
   * - :red:`E`
     - :red:`Inferential association`
     - Indirect evidence.
     - *CD33 and CD123 expression were significantly increased in patients with NPM1
       mutation with FLT3-ITD, indicating these patients may respond to
       combined anti-CD33 and anti-CD123 therapy.* The assertion is at
       least one step removed from a direct association between a variant
       and clinical relevance.

Curating Levels
---------------
Each evidence statement is the result of an experiment, trial or study in published literature. It is important to capture the nature of these experiments in the evidence entry. Evidence levels allow for the subject of an evidence item to be presented in a simple, standardized fashion. The evidence level is also an indication of how close each assertion is to actual application in the clinic. Please, note that while evidence statements of all levels are acceptable in CIViC, by far the highest priority are levels A and B, followed by C, D, E. Our top priority is to document the evidence for application of variant interpretations to real patients in the clinic today. The more time and development needed to determine the relevance of a variant to real patients in the clinic, the lower the priority for curation. Reviewing and approving evidence items requires a serious time committment by the community. Please keep this in mind and try to direct your efforts to the most immediately clinically relevant evidence first.

.. rubric:: A-Level Evidence Example

Below is an example of an `A-level (validated) Evidence Item <https://civicdb.org/links/evidence/1409>`__ for the *BRAF* - V600E variant. In this example, the Evidence Item is describing the Phase 3 randomized clinical trial that was submitted to the FDA for therapeutic approval of Vemurafenib with Dacarbazine for treatment of untreated, metastatic melanoma.

.. figure:: /images/figures/evidence-summary_EID1409.png
   :alt: Screenshot of an A-level (validated) evidence item summary

   Figure 1: Screenshot of an A-level (validated) evidence item summary

.. rubric:: A-level Curation Practices

Typically, A-level Validated Evidence Items describe Phase III Clinical Trials (for therapeutics or companion diagnostics), which are subsequently submitted to the FDA for pre-market approval.

In general, Evidence Items derived from any study cited in approvals, established practice guidelines, or considered the definitive practice-changing study, may be labeled Level A. In some cases Phase I trials can meet this requirement (see `EID1187 <https://civicdb.org/links/evidence/1187>`__).

Evidence Statements should include the gene/variant being evaluated, the study population, disease state, study size, statistical significance (e.g., p-value, confidence interval), duration of the study, and other relevant information that is required to assess the evidence for variant interpretation.

Evidence Items derived from publications describing practice guidelines (e.g. WHO diagnostic criteria) are labeled A-Validated Evidence Level. 

.. rubric:: B-Level Evidence Example

Below is an example of a `B-level (clinical) Evidence Item <https://civicdb.org/links/evidence/1410>`__ for the *BRAF* - V600E variant. In this example, the Evidence Item is describing a Phase 2 randomized clinical trial that was used to assess preliminary efficacy of the use of Vemurafenib for treatment of patients with previously treated skin melanoma.

.. figure:: /images/figures/evidence-summary_EID1410.png
   :alt: Screenshot of an B-level (clinical) evidence item summary

   Figure 2: Screenshot of an B-level (clinical) evidence item summary

.. rubric:: B-Level Curation Practices

B-level Evidence Items can describe trials submitted to the FDA during the approval process; however, relative to A-level Evidence Items, B-level Evidence Items typically have a smaller sample size or assess less significant outcomes (e.g., response rate instead of overall survival).

Phase I, II, and III clinical trials make up a significant percentage of Level B Evidence Items.

For curation of Phase I evidence, notes on treatment related adverse events may be added to the main evidence statement describing the variant-positive patient subgroup response to treatment, as dosing and adverse events are among the main focuses of Phase I studies.

B-level Evidence Items do not have to be derived from clinical trials but also can describe studies which attain a sufficient sample size to be considered more informative than a series of case studies, and ideally have some component of statistical conclusions in their results.

Greater than five patients are typically required for an Evidence Item to be considered a B-level Evidence Item.

Evidence Statements should include the gene/variant being evaluated, the study population, disease state, study size, statistical significance (e.g., p-value, confidence interval), duration of the study, and other relevant information that is required to assess the evidence for variant interpretation.

Categorical variants (sometimes called bucket variants colloquially) often appear in B-level Evidence Items describing clinical trials, which pool together patient populations with mutations of a certain class (e.g. “*PIK3CA* mutation”), in order to attain a disease specific, statistically significant, clinical result across the patient population (e.g. Trastuzumab resistance in *HER2* positive breast cancer).

.. rubric:: C-Level Evidence Example

Below is an example of a `C-level (case study) Evidence Item <https://civicdb.org/links/evidence/757>`__ for the *BRAF* - V600E variant. In this example, the Evidence Item is describing a single patient with the *BRAF* - V600E variant who demonstrated sensitivity/response to Pictilisib in the disease context of melanoma. This Evidence Item was classified as a Case Study because it described results for a single patient with advanced melanoma who had been enrolled in a larger Phase I clinical trial that evaluated 60 patients with advanced solid tumors and any *BRAF* variant for sensitivity to Pictilisib.

.. figure:: /images/figures/evidence-summary_EID757.png
   :alt: Screenshot of an C-level (case study) evidence item summary

   Figure 3: Screenshot of an C-level (case study) evidence item summary

.. rubric:: C-Level Curation Practices

C-level Evidence Items should describe a specific variant and likely will not apply to a categorical variant.

In some cases a clinical trial employing a categorical or bucket variant (e.g. *EGFR* mutation) will contain additional supplementary information on individual patient mutations and outcomes (e.g. CR, PR, SD or PD as best response). In such cases, along with the B-level Evidence Item based on the categorical variant, individual C-level case study Evidence Items can be curated for each listed variant.

Evidence Items involving fewer than five patients are typically considered to be C-level Evidence Items.

Evidence Statements should include the gene/variant being evaluated, the study population, disease state, study size, statistical significance (e.g., p-value, confidence interval, if applicable), duration of the study, and other relevant information that is required to assess the evidence for variant interpretation.

.. rubric:: D-Level Evidence Example

Below is an example of a `D-level (Preclinical) Evidence Item <https://civicdb.org/links/evidence/1005>`__ for the *BRAF* - V600E variant. In this example, 49 *BRAF*-mutant melanoma cell lines exhibited resistance to a combination of dactolisib and selumetinib treatment. Note that older drug names were used in this study, BEZ238 and AZD6244, but since then, the drug names have been updated to dactolisib and selumetinib. To reduce confusion, the more current names are used in the drug field and the curator has included both the old and new names in the Evidence Statement.

.. figure:: /images/figures/evidence-summary_EID1005.png
   :alt: Screenshot of an D-level (preclinical) evidence item summary

   Figure 4: Screenshot of an D-level (preclinical) evidence item summary

.. rubric:: D-Level Curation Practices

D-level Evidence Items typically describe animal models or cell line studies. The sample size for these studies can influence the Trust Rating, whereby increased numbers of mice or independent biological replicates used should increase the Trust Rating.

A concise description of the experiments performed should be prepared by the curator, supporting the Evidence Item Clinical Significance, and describing the controls that were used, and the significant findings that were observed. 

Evidence Statements should include the gene/variant being evaluated, the study population, disease state, study size, statistical significance (e.g., p-value, confidence interval), duration of the study, and other relevant information that is required to assess the evidence for variant interpretation.

When choosing a disease for Preclinical Evidence Items, it should reflect the context of the ultimate disease type that is being investigated and not necessarily the individual cell-line being evaluated. For example in `EID1356 <https://civicdb.org/links/evidence/1356>`__, the preclinical work was performed on BA/F3 however the conclusions supported work across multiple cancer subtypes, therefore the selected disease field for this Evidence Item was “Cancer”.

.. rubric:: E-Level Evidence Example

Below is an example of an `E-level (inferential) Evidence Item <https://civicdb.org/links/evidence/92>`__ for the *BRAF* - V600 Amplification variant. In this example, the Evidence Item is describing how *BRAF* - V600E Amplification could be a mechanism of selumetinib resistance in patients with colorectal cancer.

.. figure:: /images/figures/evidence-summary_EID92.png
   :alt: Screenshot of an E-level (inferential) evidence item summary

   Figure 5: Screenshot of an E-level (inferential) evidence item summary

.. rubric:: E-Level Curation Practices

E-level Evidence Items provide inferential support for the described variant. This could mean that the variant was not ever actually measured, or that the results from the study do not directly evaluate the claims made by the Evidence Item. 

E-level Evidence Items can be derived from in silico predictions, cell lines, animal models, or human studies.

Evidence Statements should include the gene/variant being evaluated, the study population, disease state, study size, statistical significance (e.g., p-value, confidence interval), duration of the study, and other relevant information that is required to assess the evidence for variant interpretation. Often these data are not available for E-level Evidence Items.
