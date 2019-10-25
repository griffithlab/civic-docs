.. _evidence-evidence_rating:

Evidence Rating
===============
The Evidence Rating is scored on a scale from 1-5 stars reflecting the curator’s confidence in the quality of the summarized evidence.

Understanding Evidence Ratings
------------------------------
The Evidence Rating depends on a number of factors, including study size, study design, orthogonal validation, and reproducibility. Although the overall publication/study/abstract might be high quality, the Evidence Rating may be low for an Evidence Item referring to a single conclusion in the study that is not well supported. The Evidence rating therefore does not rate the journal, publication, or Evidence Source itself, but instead evaluates in isolation the components of evidence extracted from the Evidence Source. While this remains a somewhat subjective measure, general best-practices for the Evidence Rating are detailed below.

Curating Evidence Ratings
-------------------------
In order to quickly discern how well the evidence derived from the pubmed or abstract evidence source supports a given evidence statement, a five star evidence rating system is used. Each evidence item is given a rating, from 1 to 5 stars, based on the quality of the evidence the statement summarizes. This rating depends on a number of factors, including study size, quality control, orthogonal validation, and reproducibility. It should be noted that this rating is largely subjective and may be debated (hopefully within the CIViC interface). Also the rating should be specific to the evidence statement. The overall publication/study might be high quality, but the evidence statement may refer to a single conclusion in the study, and that part of the study might not be well supported. For example, the assertion may relate to patients with a particular mutation, and the study might involve an impressive 500 patients, but if only 2 patients have the mutation in question, the quality rating may be low for this evidence statement.

.. list-table::
   :widths: 20 80
   :header-rows: 1

   * - Evidence Rating
     - Definition
   * - |star| |star| |star| |star| |star|
     - Strong, well supported evidence from a lab or journal with respected academic standing. Experiments are well controlled, and results are clean and reproducible across multiple replicates. Evidence confirmed using independent methods. The study is statistically well powered.
   * - |star| |star| |star| |star| |star-o|
     - Strong, well supported evidence. Experiments are well controlled, and results are convincing. Any discrepancies from expected results are well-explained and not concerning.
   * - |star| |star| |star| |star-o| |star-o|
     - Evidence is convincing, but not supported by a breadth of experiments. May be smaller scale projects, or novel results without many follow-up experiments. Discrepancies from expected results are explained and not concerning.
   * - |star| |star| |star-o| |star-o| |star-o|
     - Evidence is not well supported by experimental data, and little follow-up data is available. Publication is from a journal with low academic impact. Experiments may lack proper controls, have small sample size, or are not statistically convincing.
   * - |star| |star-o| |star-o| |star-o| |star-o|
     - Claim is not supported well by experimental evidence. Results are not reproducible, or have very small sample size. No follow-up is done to validate novel claims.

Curating Five-Star Evidence
~~~~~~~~~~~~~~~~~~~~~~~~~~~
The example `Evidence Item below <https://cividb.org/links/evidence/1199>`__ describes a Phase III clinical trial (PROFILE 1014) that evaluated the impact of the *ALK* - Fusions variant on therapeutic response with crizotinib for patients with lung non-small cell carcinoma. The clinical trial was a randomized, double-blinded, placebo-control study of 343 patients that evaluated progression free survival, objective response rate, and quality of life. The results were published in the New England Journal of Medicine.

.. figure:: /images/figures/evidence-summary_EID1199.png
   :alt: Screenshot of EID1199 summary, a five-star Evidence Item

   Figure 1: Screenshot of EID1199 summary, a five-star Evidence Item

Evidence Items with a 5-star rating should be strong, well-supported evidence from a lab or journal with respected academic standing. Experiments should be well controlled, and results should be clean and reproducible across multiple replicates. Evidence should be confirmed using independent methods and the study should be statistically powered. 

In general, Evidence Rating is a rating of the unit of evidence extracted from a data source (publication or ASCO abstract) and is not a rating of the publication or abstract itself. Thus, an isolated supplementary figure in a high quality and well-researched publication may yield a relevant piece of clinical information on a variant of interest, and an Evidence Item (EID) could be prepared from this figure. Due to the limited nature of the data supporting this type of Evidence Item, it would receive a lower Evidence Rating. This is because this rating would applies only to the evidence used to create this single EID, not to the publication as a whole.

Curating Four-Star Evidence
~~~~~~~~~~~~~~~~~~~~~~~~~~~
The example `Evidence Item below <https://cividb.org/links/evidence/1199>`__ describes a Phase 2A clinical trial with multiple arms that included evaluation of the therapeutic effect of pertuzumab and trastuzumab on 37 patients with *HER2* - Amplified colorectal cancer. The study was sufficiently powered to demonstrate an increase in patient response and remission provided their advanced, refractory state and relatively rare molecular alteration for that tumor type. The study was part of a clinical trial that was registered through the NIH and was published in the Journal of Clinical Oncology.

.. figure:: /images/figures/evidence-summary_EID5981.png
   :alt: Screenshot of EID5981's summary, a five-star Evidence Item

   Figure 2: Screenshot of EID5981's summary, a five-star Evidence Item

Evidence items with a 4-star rating should be strong, have well-supported evidence, well-controlled experiments, and convincing results. Any discrepancies from expected results are well-explained and not concerning.

This example was similar in design as the 5-start example, however, the reduced sample size contributed to the reduction in the start rating.

Curating Three-Star Evidence
~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The example `Evidence Item below <https://cividb.org/links/evidence/5982>`__ describes the same Phase 2A clinical trial from Supplementary Figure 23, but differs in the advanced solid tumor type being evaluated. In the subset of patients with bladder cancer, three of nine patients showed response to combination therapy with trastuzumab and pertuzumab, which supports sensitivity/response. Although this evidence item is derived from the same clinical trial, the reduction in Evidence Rating is representative of the smaller number of patients and large 95% confidence interval.

.. figure:: /images/figures/evidence-summary_EID5982.png
   :alt: Screenshot of EID5982's summary, a five-star Evidence Item

   Figure 3: Screenshot of EID5982's summary, a five-star Evidence Item

Evidence Items with a 3-star rating are convincing but not supported by a breadth of experiments. These Evidence Items be smaller scale projects, or novel results without many follow-up experiments. 

Even though these Evidence Items might contain reduced amount of data discrepancies from expected results should still be explained and not concerning. 

Curating Two-Star Evidence
~~~~~~~~~~~~~~~~~~~~~~~~~~
The example `Evidence Item below <https://cividb.org/links/evidence/5982>`__ describes a Phase II clinical trial that evaluated 29 patients with breast cancer who were being treated with either afatinib, lapatinib, or trastuzumab. In this study, 18 patients showed response to one of the therapeutics. The Evidence Rating for this evidence item was only 2 stars due to lack of evidence supporting the clinical claim (supports sensitivity/response). Specifically, the sample size was low for each of the three arms, there was no reported statistical significance. Additionally, the clinical endpoint for the study was objective response rate, which is not as strong of an endpoint as other metrics such as overall survival.

.. figure:: /images/figures/evidence-summary_EID887.png
   :alt: Screenshot of EID887's summary, a five-star Evidence Item

   Figure 4: Screenshot of EID887's summary, a five-star Evidence Item

Evidence items with a 2-star rating are not well supported by experimental data, and little follow-up data is available. 

Typically, Evidence Items received a 2-star rating if the experiments lack proper controls, have small sample size, or are not statistically convincing.  

Curating One-Star Evidence
~~~~~~~~~~~~~~~~~~~~~~~~~~
The example `Evidence Item below <https://cividb.org/links/evidence/895>`__ describes a B-level clinical study that evaluated 6 patients with *ERBB2* - Amplification for response to capecitabine, oxaliplatin, and chemoradiotherapy, with or without cetuximab. There was no difference in outcome between the 6 patients with the variant when compared to the 135 patients with no visible *ERBB2* - Amplification on *FISH* / *IHC*. The Evidence Item a heterogenous combination of variant detection methods, a low number of patients in the experimental arm (n=6) and overall low statistical power. Therefore, despite being a B-level Evidence Item, the curator assigned the EID a 1-star Evidence Rating.

.. figure:: /images/figures/evidence-summary_EID895.png
   :alt: Screenshot of EID895's summary, a five-star Evidence Item

   Figure 5: Screenshot of EID895's summary, a five-star Evidence Item

Evidence items with a 1-star rating contain claims that are not well-supported by experimental evidence. Typically, the results are not reproducible and/or have very small sample size. No follow-up is done to validate novel claims.

Typically, Evidence Items received a 1-star rating if the experiments lack proper controls, have small sample size, or are not statistically convincing.  
