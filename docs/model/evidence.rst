Evidence Items
=======================
Evidence Items follow a structured knowledge model with 12 required fields (Gene name, Variant Name, Source Type, Variant Origin, Disease, Evidence Statement, Evidence Type, Evidence Level, Evidence Direction, Clinical Significance, and Trust Rating) with additional optional fields (Associated Phenotypes). Based on the Evidence Type, additional required or optional fields become available (e.g., Predictive Evidence Types require a Drug Name).

At the heart of CIViC is the clinical evidence statement. The clinical evidence statement is a piece of information that has been manually curated from trustable medical literature about a variant or genomic ‘event’ that has implications in cancer predisposition, diagnosis (aka molecular classification), prognosis, or predictive response to therapy. For example, “Patients with BRAF V600 mutations respond well to the drug dabrafenib”. A variant may be a single nucleotide substitution, a small insertion or deletion, an RNA gene fusion, a chromosomal rearrangement, an RNA expression pattern (e.g. over-expression), etc. Each clinical evidence statement corresponds to a single citable publication.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   evidence/overview
   evidence/gene
   evidence/molecular_profile
   evidence/statement
   evidence/level
   evidence/type
   evidence/direction
   evidence/clinical_significance
   evidence/origin
   evidence/disease
   evidence/drug
   evidence/associated_phenotype
   evidence/source
   evidence/clinical_trial
   evidence/evidence_rating
