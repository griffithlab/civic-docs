FAQ
===

.. contents:: Questions
   :backlinks: entry

How do I cite CIViC?
--------------------
A `manuscript describing CIViC <http://www.nature.com/ng/journal/v49/n2/full/ng.3774.html>`_ was first published in Nature Genetics (`PMID: 28138153 <https://www.ncbi.nlm.nih.gov/pubmed/28138153>`_). Please cite:

    Griffith M\ :sup:`*,†`, Spies NC\ :sup:`*`, Krysiak K\ :sup:`*`, McMichael JF, Coffman AC, Danos AM, Ainscough BJ, Ramirez CA, Rieke DT, Kujan L, Barnell EK, Wagner AH, Skidmore ZL, Wollam A, Liu CJ, Jones MR, Bilski RL, Lesurf R, Feng YY, Shah NM, Bonakdar M, Trani L, Matlock M, Ramu A, Campbell KM, Spies GC, Graubert AP, Gangavarapu K, Eldred JM, Larson DE, Walker JR, Good BM, Wu C, Su AI, Dienstmann R, Margolin AA, Tamborero D, Lopez-Bigas N, Jones SJ, Bose R, Spencer DH Wartman LD, Wilson RK, Mardis ER, Griffith OL\ :sup:`†`. 2016. *CIViC is a community knowledgebase for expert crowdsourcing the clinical interpretation of variants in cancer.* Nat Genet. 49, 170–174 (2017); doi: `doi.org/10.1038/ng.3774 <http://dx.doi.org/10.1038/ng.3774>`_. :sup:`*`\ These authors contributed equally to this work. :sup:`†`\ Corresponding author.

Additional CIViC-related publications can be found on our :doc:`citations <citations>` page.
     
What is CIViC?
--------------
CIViC is an open access, open source, community-driven web resource for Clinical Interpretation of Variants in Cancer. Our goal is to enable precision medicine by providing an educational forum to disseminate knowledge and encourage active discussion of the clinical significance of cancer genome alterations.

What is precision medicine?
---------------------------
Precision medicine refers to the customization of healthcare strategies to the individual using the unique features of the patient's environmental, behavioral and genetic context. With regards to cancer, this might involve the identification of specific somatic or germline mutations known to predict response to a targeted therapy. You can read more about this topic in summaries from the `White House <http://www.whitehouse.gov/the-press-office/2015/01/30/fact-sheet-president-obama-s-precision-medicine-initiative>`_ and the `New England Journal of Medicine <http://www.nejm.org/doi/full/10.1056/NEJMp1500523#t=article>`_

Why use a crowdsourcing model for variant curation?
---------------------------------------------------
The rapid expansion of biomedical literature presents an intractable challenge for investigators and clinicians to efficiently interpret and synthesize the complete array of knowledge available for each cancer-associated genomic variant for clinically-relevant use. Efforts to curate the clinical importance of variants have been undertaken by a diverse, but fragmented, community of individuals. Crowdsourcing leverages the resources of individuals to produce a centralized, open-sourced platform for this diverse community to discuss and share findings in their respective specialities. CIViC also serves as a platform for contributors keep up to date on recent advances.

Who is CIViC designed for?
--------------------------
CIViC is intended to bring together a diverse group of individuals interested in the clinical application and advancement of cancer genomics including health professionals (oncologists, pathologists and other clinicians), researchers (cancer genome and data scientists), and patient advocates. CIViC does not provide any medical or healthcare products, services or advice, and is not for medical emergencies or urgent situations. Information contained on this website is not a substitute for a doctor's medical judgment or advice. Patients should always discuss their specific, individual health concerns with a doctor or health care professional.

What are the characteristics of an 'ideal' CIViC curator/editor?
----------------------------------------------------------------
CIViC curators and editors should express a strong interest in clinical cancer genomics. Curators/editors should have expertise in relevant academic fields including basic cancer biology, oncology, genomics, clinical informatics, etc and ideally are training for or have already obtained a medical degree (e.g. PhD or MD). Additionally, we expect curators/editors to be open to sharing information with the community, be respectful of other contributors, professional, truthful, ethical, and unbiased. There is sometimes pressure in academia to present one's research findings in a clinically relevant context. When CIViC evidence statements are created, the curator/editor should conduct an objective assessment of how well the data supports any assertion of clinical relevance. All aspects of the CIViC project are open to debate and amendment, including these guidelines. In addition to adhering to the guiding principles of CIViC, a CIViC editor must also declare any conflicts of interest.

What is a *Variant*?
--------------------
A genetic variant is a non-exact copy of a biological sequence. This includes single nucleotide variants (SNVs), insertion/deletion events (indels), copy number alterations (CNVs), structural variants (SVs), transcript fusions, and other genomic/molecular events with cancer associations. The vast majority of variants described in CIViC represent mutations at the DNA level, however, alterations that manifest at the RNA, protein, or epigenetic level are also accepted so as long as there is a demonstrated clinical relevance. In general, the concept of a variant in CIViC is very flexible, but it is highly preferred that the variant be something that could be measured with some quantitative assay (NGS sequencing, qPCR, etc.). Combinations of one or more variants comprise a Molecular Profile.

What is a *Molecular Profile*?
------------------------------
There is a growing need for clinical annotation of combinations of variants from different genes. For example, double hit lymphoma is characterized by combinations of mutations in MYC, BCL2, or BCL6. In another example, PIK3CA mutation is thought to induce trastuzumab resistance in the context of HER2 overexpressing breast cancer. CIViC addresses this need via use of the Molecular Profile. Molecular Profiles (MPs) are comprised of one or more variants. A simple Molecular Profile is comprised of a single variant. A complex MP is comprised of a combination of two or more variants. The addition of MPs to CIViC V2 involved an essential change to the data model, in that CIViC Evidence Items (EIDs) are now associated to Molecular Profliles instead of directly to variants. This enables clinical annotation of combinations of variants which may not apply to the individual variants in isolation. Annotation of a single variant is accomplished by creating Evidence Items (EIDs) for simple molecular profiles (e.g. curation of a clinical trial showing BRAF V600E sensitivity of vemurafenib in melanoma). Now, annotation of multi variant combinations can be accomplished by creating EIDs for complex Molecular Profiles (e.g. Osimertinib resistance in "EGFR L858R and EGFR T790M and BRAF V600E positive" lung adenocarcinoma). Each MP in CIViC has an associated Molecular Profile page in the user interface containing a curator summary of the MP's role in cancer, aliases, links to pages for the individual variants that comprise the MP, and a list of all of the curated Evidence Items which are uniquely associated to the MP. 

What kinds of Variants belong in CIViC? What does not?
------------------------------------------------------
Variants, or combinations of variants, are accepted into CIViC provided there is evidence linking them to cancer with some clinical or functional relevance. Relevance to cancer biology alone is NOT sufficient unless there is also some documented relationship between the variants and diagnosis, predisposition, prognosis, functional or oncogenic relevance, or predictive value for a specific treatment. Variants related to diseases other than cancer should not be entered (there is some grey area for cancer-like conditions). CIViC accepts somatic, rare germline, and common germline variants related to cancer (as long as they have clinical or functional relevance), however, most variants in CIViC are somatic mutations. Variants are related to clinical evidence via Molecular Profiles (MPs), which are comprised of combinations of one or more variant, and Evidence Items (EIDs) are curated from literature and abstracts, and associated to MPs. The quality of evidence suggesting clinical relevance of a variant or combination of variants may vary considerably. Before contributing to CIViC please review :doc:`the curation documentation <../curating>` and familiarize yourself with :doc:`the CIViC knowledge model <../model>`.

What is an Evidence Statement?
------------------------------
An evidence statement is a brief description of the clinical relevance of a simple or complex Molecular Profile that has been determined by an experiment, trial, or study from a published literature source. It captures a Molecular Profile's impact on clinical action, which can be predictive of therapy, correlated with prognostic outcome, inform disease diagnosis (i.e. cancer type or subtype), predict predisposition to cancer in the first place, or relate to the functional impact of the variant. A single citation can be the source of multiple evidence statments, but each evidence statement has only one source. A single evidence statement should correspond to only one clinical interpretation and disease. For example, if a paper describes both predictive and prognostic relevance for a variant or combination of variants, two evidence statements should be created. If two publications draw the same conclusions about the clinical relevance of a Molecular Profile, these should also be entered as two evidence statements. Functional evidence may be less strictly related to a specific cancer subtype but curation of such evidence should still prioritize Molecular Profiles or genes whose functional significance are in some way relevant to clinical interpretation. As one example, a variant of unknown clinical significance, in proximity to another clinically relevant variant, might have some clinical significance if shown to have a similar functional effect as the variant with established clinical significance.

How is this information organized?
----------------------------------
An in-depth description of the knowledge model behind CIViC can be found :doc:`here <../model>`.

What information is currently in CIViC?
---------------------------------------
CIViC currently houses thousands of evidence statements, variants and genes across multiple cancer types and these numbers are growing rapidly with your help! Refer to the `CIViC Home page <https://civicdb.org/welcome>`_ for more detailed information.

How do I contribute information?
--------------------------------
The :doc:`curation pages <../curating>` detail the curation and editing process, and includes instructions on how to curate CIViC and apply for editorship.

My favorite Gene or Molecular Profile is not in CIViC?!?
-------------------------------------------
The extensive manual curation required to add evidence statements means that there might not yet be an evidence statement for every Molecular Profile or gene of interest. This is precisely why we need community-driven efforts to grow this database. For a gene or Molecular Profile to appear in CIViC, it must have an evidence statement associated with it. To add evidence statements and begin the discussion about your gene/variant/combination of variants of interest, go :doc:`here <../curating>`!

May I enter unpublished results from n-of-1 observations?
---------------------------------------------------------
At this time, a publication or abstract is considered a minimum requirement for all evidence statements in CIViC. N-of-1 results from early stage clinical trials or patients treated under compassionate use doctrines are allowed, but only if a case report has been published in a peer reviewed journal. We are considering options for centers that wish to use a local instance of CIViC to capture unpublished individual patient observations. We are also considering other source types including clinical trial records, and ClinVar records.

Why must my contributions be approved by an Editor?
---------------------------------------------------
In an effort to ensure quality (and prevent automated spam), we require that edits be submitted to the review queue before they are shown as accepted. Editors are used for this review step to protect the CIViC resource and will approve your revisions as soon as possible. An Editor may comment on your proposed addition or revision. You will be able to see your new content in a pending state while it awaits review. To expedite the review process, we encourage you to submit high quality evidence (evidence level of validated or clinical) as the top priority. Similarly, proposing evidence statements for a new variant or gene may take longer for the community to review.

What is a Disease Ontology ID (DOID)?
-------------------------------------
To provide a structured representation of the diseases associated with evidence statements, we ask that you use disease names as they exist in the Disease Ontology from `disease-ontology.org <http://disease-ontology.org>`_. This allows for consistent representation and minimized ambiguity when referring to diseases. Such ontologies also support more flexible data queries that allow disease groupings ranging from generic terms to highly specific subtypes. If the disease ontology is missing an important recognized sub-type of disease, we will try to work with them to update their resource. Please contact us if you find such cases.

Where does this information come from? Can I submit my abstract?
----------------------------------------------------------------
The information in CIViC is derived from peer-reviewed, published literature. Every evidence item currently requires a citation from PubMed, ASCO Meetings or ASH Meetings. This means that abstracts are not supported until they are peer-reviewed, published, and a PubMed or ASCO/ASH ID is assigned.

What if a drug is shown to have a negative effect on patients with a variant? Or the study was inconclusive?
------------------------------------------------------------------------------------------------------------
The knowledge model, specifically the Evidence Direction field, is used to indicate whether the study supports or refutes (including inconclusive determinations) any interaction between the Molecular Profile and a clinical action or result. The Clinical Significance field indicates the type of effect the Molecular Profile is determined to have on clinical results, for example, having a positive, negative or neutral/no impact. These descriptions provide human readable interpretations of evidence statements that either support or refute sensitivity or resistance predictions to therapeutics (or other clinical outcomes). For more detailed definitions and specific examples, please review the knowledge model :doc:`here <../model>`.

My evidence statement disagrees with evidence from another source, should I still add it?
-----------------------------------------------------------------------------------------
Absolutely. CIViC is a forum for discussion of disagreements in the field or literature. Simply log in, go to the Comment tab found on the Evidence, Variant, Molecular Profile, or Gene pages, and discuss this disagreement with the community.

I don't want to add evidence statements, can I still contribute?
----------------------------------------------------------------
Yes. Evaluation of the literature is a collaborative effort. If you don't want to add new evidence, you can edit or discuss existing evidence. You can also help to make sure the Molecular Profile Summary is an effective, concise, and accurate summary of the current set of evidence statements and state of knowledge in the field for the Molecular Profile. You can also add promising publications to the source suggestion queue.

What is MyGene.info?
--------------------
`MyGene.info <http://mygene.info>`_ is a web service that allows simple query and retrieval of gene annotation data. We use it in CIViC to automatically import gene details from `Entrez Gene <http://www.ncbi.nlm.nih.gov/gene>`_ such as gene name, synonyms, protein domains and pathways.

Is there an API that I can access?
----------------------------------
Yes! Please review the `API documentation <https://griffithlab.github.io/civic-v2/>`_ for more details.

What is the difference between "Supports a Negative association" and "Does not support a Positive association"?
---------------------------------------------------------------------------------------------------------------
This can be confusing. We have reserved "Does not support - Sensitivity" for statements that contradict previous statements that are supporting sensitivity associations. For example, they would read "Contrary to the previous study which found this mutation sensitive to drug X, this study reported no effect." The information that this study "Does not support" the prior study's conclusion is what we are trying to capture with these classifications.

Where do I begin to curate evidence statements? Are certain evidence types or genes a priority?
-----------------------------------------------------------------------------------------------
The evidence statements that make up CIViC are generated from peer-reviewed, published literature. Our top priority is high quality (4+ star rating) Evidence Level A and B statements that associate specific variants with clinical outcomes using well powered patient cohorts. To help direct users towards genes known to be associated with clinical outcomes, we have compiled a list of high priority genes which you can download `here <https://github.com/genome/civic-server/tree/master/public/downloads/RankedCivicGeneCandidates.tsv>`_. This list is based on a survey of 90 commerically available clinical gene panels developed by 40 distinct institutes and companies. If many independent groups feel that a gene is important to profile on their assay, it might be important. CIViC aims to spell out, with complete provenance, the evidence that each of these genes really is clinically important and why/how.

Can I use a review article to create an evidence statement?
-----------------------------------------------------------
Yes, but we urge caution when using such sources. It is generally preferable to find the primary source articles cited by the review article instead. Particularly, when a review article is describing contradictory findings from multiple studies. Individual evidence items created from each study should be created to capture this debate. The Molecular Profile Description might be a better place to cite relevant review articles.

How is CIViC licensed?
----------------------
The content of CIViC, hosted by `Washington University School of Medicine <https://medicine.wustl.edu/>`_ is released under the `Creative Commons Public Domain Dedication (CC0 1.0 Universal) <https://creativecommons.org/publicdomain/zero/1.0/>`_  and the source code for the `CIViC application <https://github.com/griffithlab/civic-v2>`_ is licensed under the `MIT License <http://opensource.org/licenses/MIT>`_.
