.. _evidence:

The CIViC Evidence Item
=======================

.. image:: images/GP-113_CIViC_schema-collaboration_SCHEMA_v3a.png
   :align: right
   :scale: 50%

At the heart of CIViC is the clinical evidence statement. The clinical
evidence statement is a piece of information that has been manually curated
from trustable medical literature about a variant or genomic 'event' that has
implications in cancer predisposition, diagnosis (aka molecular
classification), prognosis, or predictive response to therapy. For example,
“Patients with BRAF V600 mutations respond well to the drug dabrafenib”. A
variant may be a single nucleotide substitution, a small insertion or
deletion, an RNA gene fusion, a chromosomal rearrangement, an RNA expression
pattern (e.g. over-expression), etc. Each clinical evidence statement
corresponds to a single citable publication. Ready to jump into the
literature? First you will need to login (or create an account if you don't
have one yet). Once you are logged in, you can check out our `ranked list of
high priority genes
<https://github.com/genome/civic-server/tree/master/public/downloads/RankedCivicGeneCandidates.tsv>`_
or visit the `Source Suggestion queue <https://civicdb.org/curation/sources>`_ for inspiration.

.. content-tabs::

  .. tab-container:: tab1
     :title: Overview

     The rows in the following table describe the minimal components of a
     CIViC Evidence Item. Several Evidence Statements are synthesized at the
     Variant level into Variant Summaries but each Evidence Statement is
     directly linked to a single article in PubMed. *More specific guidelines
     about Evidence Item components can be found in additional help tabs*.

     **General Guidelines**

     - Evidence Statements should be:

       - derived from primary literature sources (not review articles) whenever
         possible.
       - as concise as possible while providing sufficient experiemental detail to
         interpret and evaluate the evidence (N values, statistics, etc).
       - a single Predictive, Predisposing, Diagnostic or Prognostic assertion,
         not a combination.
       - aimed at a general audience, avoiding field-specific acronyms and
         colloquialisms.

     - Multiple, separate Evidence Items can be and often are derived from a
       single publication.
     - Generally, assertions involving drugs should be classified as being of
       the Predictive Evidence Type.
     - Star Ratings should be based on the strength of the specific assertion.
       Multiple assertions from the same publication can have different star
       ratings.

     **Evidence Attributes**

  .. tab-container:: tab2
     :title: Variant Origin

     The Variant Origin identifies whether the variant is presumed as an
     inherited (germline mutation) or acquired (somatic mutation) event in the
     context of the study. We generally consider somatic events to be the first
     priority, as this is an area that has not been as well addressed by existing
     resources. However, germline mutations with established clinical relevance
     are acceptable. Germline polymorphisms (>1% allele frequency in the
     population) are considered low priority, again unless there is an
     established clinical significance. Polymorphisms described in association
     studies should be curated with great caution and may face additional
     scrutiny from CIViC moderators. For some variant types, the variant origin
     field may be unknown or N/A. For example, EXPRESSION variants are neither
     germline nor somatic. Fusion variants are an unusual case in that they are
     often observed in the transcriptome but are usually accompanied by an
     underlying somatic (or germline) mutation. Most fusions should be entered as
     somatic. If in doubt, please note the issue at the time of your submission
     to encourage discussion during the moderation stage.

     **Variant Origin Guidelines**

  .. tab-container:: tab3
     :title: Evidence Types

     When curating evidence statements from published sources, to discern
     whether a variant has a "clinical interpretation", we use the data model
     below. Evidence statements describe how a variant was demonstrated to (1)
     be predictive of drug response, (2) be correlated with prognostic
     outcome, (3) be of diagnostic utility in determining cancer subtype (aka
     molecular classification), or (4) predispose a person to a type of
     cancer. If an evidence item can not be placed in one of these four
     categories (Predictive, Prognostic, Diagnostic, Predisposing), it likely
     lies outside of the scope of CIViC. However, published statements about a
     gene or variant that cannot be placed within these categories can still
     be added to the gene and variant summaries.

     .. cssclass:: table-bordered
     .. list-table::
        :widths: 10 10 20 70
        :header-rows: 1
        :stub-columns: 1

        * - Evidence Type
          - Evidence Direction
          - Clinical Significance
          - Example
        * -
          - sth
          - sth
          - sth
        * - sth
          - sth
          - sth
          - sth

  .. tab-container:: tab4
     :title: Evidence Levels

     Each evidence statement is the result of an experiment, trial or study in
     published literature. It is important to capture the nature of these
     experiments in the evidence entry. Evidence levels allow for the subject
     of an evidence item to be presented in a simple, standardized fashion.
     The evidence level is also an indication of how close each assertion is
     to actual application in the clinic. Please, note that while evidence
     statements of all levels are acceptable in CIViC, by far the highest
     priority are levels A and B, followed by C, D, E. Our top priority is to
     document the evidence for application of variant interpretations to real
     patients in the clinic today. The more time and development needed to
     determine the relevance of a variant to real patients in the clinic, the
     lower the priority for curation. Reviewing and approving evidence items
     requires a serious time committment by the community. Please keep this in
     mind and try to direct your efforts to the most immediately clinically
     relevant evidence first.

     .. list-table::
        :widths: 10 20 70
        :header-rows: 1

        * - Level
          - Definition
          - Example and further comments
        * - A
            Validated association
          - Proven/consensus association in human medicine.
          - *"AML with mutated NPM1" is a provisional entity in WHO classification of acute
            myeloid leukemia (AML). This mutation should be tested for in
            clinical trials and is recommended for testing in patients with
            cytogenetically normal AML.* Validated associations are often in
            routine clinical practice already or are the subject of major
            clinical trial efforts.
        * - B
            Clinical evidence
          - Clinical trial or other primary patient data
            supports association.
          - *BRAF V600E is correlated with poor
            prognosis in papillary thyroid cancer in a study of 187 patients
            with PTC and other thyroid diseases.* The evidence should be
            supported by observations in multiple patients. Additional support
            from functional data is desirable but not required.
        * - C
            Case study
          - Individual case reports from clinical journals.
          - *A single patient with FLT3 over-expression responded to the FLT3
            inhibitor sunitinib.* The study may have involved a large number of
            patients, but the statement was supported by only a single
            patient. In some cases, observations from just a handful of
            patients (e.g. 2-3) or a single family may also be considered a
            case study/report.
        * - D
            Preclinical evidence
          - In vivo or in vitro models support association.
          - *Experiments showed that AG1296 is effective in
            triggering apoptosis in cells with the FLT3 internal tandem
            duplication.* The study may have involved some patient data, but
            support for this statement was limited to in vivo or in vitro
            models (e.g. mouse studies, cell lines, molecular assays, etc.).
        * - E
            Inferential association
          - Indirect evidence.
          - *CD33 and CD123 expression were significantly increased in patients with NPM1
            mutation with FLT3-ITD, indicating these patients may respond to
            combined anti-CD33 and anti-CD123 therapy.* The assertion is at
            least one step removed from a direct association between a variant
            and clinical relevance.

  .. tab-container:: tab5
     :title: Trust Ratings

     In order to quickly discern how much trust curators and users have in a
     single evidence statement, a five star trust rating system is used. Each
     evidence item is given a rating, from 1 to 5 stars, based on the quality
     of the evidence the statement summarizes. This rating depends on a number
     of factors, including journal impact, study size, quality control,
     orthogonal validation, and reproducibility. It should be noted that this
     rating is largely subjective and may be debated (hopefully within the
     CIViC interface). Also the rating should be specific to the evidence
     statement. The overall publication/study might be high quality in a high
     impact publication, but the evidence statement may refer to a single
     conclusion in the study, and that part of the study might not be well
     supported. For example, the assertion may relate to patients with a
     particular mutation, and the study might involve an impressive 500
     patients, but if only 2 patients have the mutation in question, the
     quality rating may be low for this evidence statement.

     .. list-table::
        :widths: 10 90
        :header-rows: 1

        * - Trust Rating
          - Definition
        * - .. raw:: html

               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
          - Strong, well supported evidence from a lab or journal with respected academic standing. Experiments are well controlled, and results are clean and reproducible across multiple replicates. Evidence confirmed using independent methods. The study is statistically well powered.
        * - .. raw:: html

               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
          - Strong, well supported evidence. Experiments are well controlled, and results are convincing. Any discrepancies from expected results are well-explained and not concerning.
        * - .. raw:: html

               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
          - Evidence is convincing, but not supported by a breadth of experiments. May be smaller scale projects, or novel results without many follow-up experiments. Discrepancies from expected results are explained and not concerning.
        * - .. raw:: html

               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
          - Evidence is not well supported by experimental data, and little follow-up data is available. Publication is from a journal with low academic impact. Experiments may lack proper controls, have small sample size, or are not statistically convincing.
        * - .. raw:: html

               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
          - Claim is not supported well by experimental evidence. Results are not reproducible, or have very small sample size. No follow-up is done to validate novel claims.
