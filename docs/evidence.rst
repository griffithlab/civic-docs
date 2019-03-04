.. role:: green

.. role:: blue

.. role:: purple

.. role:: orange

.. role:: red

.. _evidence:

Evidence Items
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



.. toctree::
   :maxdepth: 2
   :caption: Contents:

   evidence/overview
   evidence/variant_origin
   evidence/evidence_type
   evidence/evidence_level
   evidence/trust_rating
