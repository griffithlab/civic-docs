Ideas
=====

New CIViC curators, commonly ask where they should focus their efforts and where can they find evidence of the clinical significance of cancer variants. There are many approaches and relevant resources that may help to identify and prioritize such evidence.

Remember that the focus of CIViC is on the **clinical** relevance of **cancer** variants. Before expending the effort to propose an addition to CIViC, ask yourself would a clinician potentially find this information useful in understanding and treating a patient's cancer? Could an oncologist use this evidence to better understand likely response to therapy (Predictive evidence), or outcome (Prognostic) for their patient? Would a pathologist find knowledge of the variant valuable in classifying (Diagnostic) the tumor into a subtype? Would a medical geneticist or genetic counselor be interested in the causative (Predisposing) significance of this evidence?

In addressing these questions, try to think about the distinction between the relevance of a variant to cancer biology and its relevance in a clinical setting. A variant may have great and diverse relevance to the biology of a cancer cell but have limited or no clinical applicability. For example, TP53 mutations are critical in many cancers and hundreds (if not thousands) of papers have been written about their complex roles in cancer biology. However, the scenarios in which TP53 mutations are **clinically** relevant are much, much narrower. A variant may NOT be clinically relevant despite being characterized as functional (gain or loss of function), a 'driver', 'recurrent', etc. In some, perhaps most cases, the clinical relevance of these variants may simply not be established yet. However, CIViC is about the **evidence that establishes their clinical relevance**. By contrast, in some cases, the biological relevance may be poorly understood while clinical utlity is established. Such evidence does belong in CIViC. A mechanistic understanding is desirable, but not required.

The above description, despite it length, is an oversimplification. The concept of clinical utility varies by Evidence type: Predictive, Prognostic, Diagnostic and Predisposing. There are many nuances to be considered. The "ideal" clinical interpretation and definition of clinical utility are open to debate. We welcome this debate and one of the goals of CIViC is to enable and capture it. If you believe some evidence is relevant to CIViC but have some doubts, please submit it so that the community can discuss with you.

The following list is not exhaustive but provides many examples of approaches to identify high quality evidence. If you know of a useful resource that is not listed below, please let us know about it. NOTE: some of these resources are open access, others are not. When entering evidence into CIViC, **never** copy content or ideas from another resource. Your contributions to CIViC should be based on published evidence, but in your own words.

.. rubric:: Example sources of CIViC evidence and high priority variants

- Published results from clinical trials involving cancers with specific
  variants (e.g. HER2 +ve breast cancer)
- Published evidence for the arms of basket clinical trials (e.g.
  `NCI-MATCH <https://clinicaltrials.gov/ct2/show/NCT02465060>`_,
  `ASCO-TAPUR <https://clinicaltrials.gov/ct2/show/NCT02693535>`_,
  `I-SPY2 <https://clinicaltrials.gov/ct2/show/NCT01042379>`_,
  `BATTLE-1 <https://clinicaltrials.gov/ct2/show/NCT00409968>`_,
  `BATTLE-2 <https://clinicaltrials.gov/ct2/show/NCT01248247>`_,
  `CUSTOM <https://clinicaltrials.gov/show/NCT01306045>`_, etc.).
- A gene, variant or paper, that you are an expert in. For example, this
  might be work from your own research/practice.
- Public discussions on cases submitted to the `ASCO Molecular Oncology
  Tumor Board <https://connection.asco.org/discussion?tid=201>`_
- The `CIViC publication queue <https://civicdb.org/curation/sources>`_,
  a place were CIViC curators add and discuss
  papers thought to contain valuable evidence.
- We created a `ranked list of relevant genes
  <https://github.com/genome/civic-server/tree/master/public/downloads/RankedCivicGeneCandidates.tsv>`_,
  based on a comprehensive
  survey of genes that are targeted by dozens of assays in clinical use.
- We also created a `ranked list of relevant publications <https://github.com/genome/civic-server/tree/master/public/downloads/CIViC-vs-OtherResources-Pubmed-Stats.xls>`_ by summarizing
  overlap between the publications used in CIViC and other companion
  resources.
- Our colleagues at the BC Cancer Agency have developed a natural language
  processing approach and resulting database of automatically mined CIViC
  relevant publications called: CIViC-mine (`coming soon
  <https://civicdb.org/>`_).
- Treatment guidelines (e.g. `NCCN guidelines
  <https://www.nccn.org/professionals/physician_gls/f_guidelines.asp>`_,
  `ASCO guidelines
  <https://www.asco.org/practice-guidelines/quality-guidelines/guidelines>`_,
  `ESMO guidelines <http://www.esmo.org/Guidelines>`_, etc.).
- Variants and papers referenced in other open access databases such as
  `ClinVar <https://www.ncbi.nlm.nih.gov/clinvar/>`_ and `OMIM
  <https://www.ncbi.nlm.nih.gov/omim/>`_.
- Companion resources of CIViC participating in the `GA4GH Variant
  Interpretation for Cancer Consortium (VICC) <http://ga4gh.org/#/vicc>`_ or others such as: `PMKB <https://pmkb.weill.cornell.edu/>`_,
  `OncoKB <http://oncokb.org/#/>`_, `MyCancerGenome <https://www.mycancergenome.org/>`_, `CanDL <https://candl.osu.edu/>`_, `BaseSpace KN <https://variantinterpreter.informatics.illumina.com/>`_, `Cancer Genome Interpreter <https://www.cancergenomeinterpreter.org/home>`_,
  `COSMIC <http://cancer.sanger.ac.uk/cosmic/drug_resistance>`_, `PCT <https://pct.mdanderson.org/#/home>`_, `PharmGKB <https://www.pharmgkb.org/>`_. A detailed comparison of these resources can be
  found in the `CIViC Related Resources Table <https://goo.gl/5WAZmd>`_. While these resources can be
  used for inspiration, do not plagiarize/copy any content from these
  sources that might violate their copyrights.
- Papers referenced by the `Atlas of Genetics and Cytogenetics in Oncology
  and Haematology <http://atlasgeneticsoncology.org/>`_
- Keyword searches in `PubMed <https://www.ncbi.nlm.nih.gov/pubmed/>`_ or `Google Scholar
  <https://scholar.google.com/>`_
- Papers from certain topical journals. The most cited journals in CIViC
  are summarized on the `CIViC Source Statistics page
  <https://civic.genome.wustl.edu/statistics/sources>`_
- Variants and related papers from the `Sarcoma Initiative
  <http://sarcomahelp.org/articles/chromosomal-translocations.html>`_.
- Variants from the `LOVD project <http://www.lovd.nl/3.0/home>`_.

Example Curation Activities
===========================

Most of the contents of CIViC are curator generated and edited. Below are a few examples of areas where curators are needed, culminating in a list of bite sized curation tasks that should require less than 3 minutes of your time.

.. rubric:: 1. Adding Evidence

Evidence records are the heart of the CIViC resource. Each corresponds to evidence for a single clinical assertion about a single variant in a single cancer type. Each evidence record is based on a single citable source (e.g. a peer-reviewed publication). The evidence record consists of a free-form executive summary describing the assertion and supporting evidence for it, and additional structured fields that describe the evidence (e.g. evidence type, relevant drug, etc.). To learn more about the elements of an evidence record refer to the :doc:`Evidence help docs <../model/evidence>`. For suggestions on where to find sources for evidence records, refer to the Source Ideas tab of this section. To add a new evidence record, you must login and hit the "ADD" button at the top of any page throughout the site.

.. rubric:: 2. Adding or improving Variant, Variant Group, and Gene Summaries

Once sufficient evidence accumulates for a variant, variant group or gene entity, a summary should be created. The summary should be an overview of the evidence records associated with the entity. The summary should focus on the most clinically actionable evidence and should summarize for each relevant gene what a clinician should be aware of for patients with a particular variant, or variants in a particular gene. Very brief background material may be included. Additional citations beyond those associated with the evidence records can be associated directly with the summary using the "Add Source" option in the edit form. To learn more about each major CIViC entity, refer to the :doc:`../model/variants`, :doc:`../model/variant_groups`, and :doc:`../model/genes` sections of the help pages.

.. rubric:: 3. Adding or improving Assertions

An important final product of the CIViC curation process is the Assertion. Gene and Variant Summaries (described above) provide an overall summary of the clinical relevance of genes and variants as documented by the entire body of CIViC evidence. In contrast, Assertions provide a consensus of the clinical significance (and supporting evidence) for a specific gene-variant, in a specific disease context. The assertion should represent the current state of understanding in the field and be associated with the appropriate AMP tier or ACMG codes and assessment for the variant. Once sufficient evidence has been documented, a new assertion can be submitted using the “ADD” button at the top of any page throughout the site. Reviewed and accepted assertions enter the queue for submission to ClinVar. Creating is assertions is among the most advanced curation tasks in CIViC.

.. rubric:: 4. Editing CIViC Content

CIViC content can be edited by clicking on the pencil icon as displayed for an example Variant here:

.. image:: ../images/figures/CIViC_edit_variant_screenshot.png

Gene, Variant, Variant Group and Evidence entities can all be edited. These edits may be expansive major updates to incorporate new evidence, error corrections, improvements to readability and style, or minor grammar and typo fixes. All such edits are welcome.

.. rubric:: 5. Comment on CIViC Content

Throughout the website are "Talk" pages where users can comment on the current contents of CIViC (specific Evidence, Variants or Genes) or on Suggested Changes. Curators are encouraged to be verbose in their comments on existing content. Critism, clarification, qualification, and questions are all appropriate. Comments from the authors of work being summarized or others with particular expertise in the area are especially desirable. When adding new evidence or summaries, comments may be used to describe the thought process of the curator. Small quotes (as allowed by the Fair Use doctrine) from source publications that support a submission may also be included (but please indicate these with quotes or use the block quote style).

.. rubric:: 5. Variant attributes

In addition to the variant summary (discussed above), there are several other structured values associated with variant records. These include:

- **Aliases.** Alternative names (synonyms) for the variant. For many variants, researchers from different groups may refer to variants by different names. Multiple and varying abbreviations or identifiers exist for most variants. A variant alias is generally any name the might help CIViC users determine the various ways used to indicate the same variant.
- **HGVS expressions.** CIViC supports and promotes variant identification using the `Sequence Variant Nomenclature <http://varnomen.hgvs.org/>`_ guidelines of the Human Genome Variation Society (HGVS), otherwise known as 'HGVS strings'. Curators may add one or more valid HGVS values for each variant. These may be entered in protein (p.), cDNA (c.), or genomic (g.) format. A particular CIViC variant (e.g. BRAF V600E) may have multiple valid genomic alterations that could create it, each with a distinct genomic HGVS expression. Similarly, multiple cDNA HGVS strings may correspond to multiple transcript sequences, possibly from various transcript annotation databases (e.g. Ensembl, RefSeq, LRG, etc.) or alternative isoforms of a gene.
- **Coordinates.** For each variant, the goal of CIViC initially is to determine unambiguous genomic coordinates for an example instance of the variant. For instance, if the paper refers to the variant as "V600E", the curator determines for a particular build of the human genome, the corresponding chromosome, start position, end position, reference base and variant base. Refer to the :doc:`Variants documentation <../model/variants>` on the left for more details.

.. rubric:: 6. Bite-size curation tasks

Only have a few minutes? Tackle one of the tasks below.

- `Suggest a Source <https://civicdb.org/suggest/source>`_.

  - Identify a publication containing a variant with clinical relevance.
  - Visit PubMed to identify the publication's `PubMed
    <https://www.ncbi.nlm.nih.gov/pubmed/>`_ ID.
  - Enter as much information possible to help curators. This form only requires 2 elements: PubMed ID and a comment to direct curators as to why you believe this publication has clinically-relevant information about a variant.
  - Your suggested source can be seen in the `Source Suggestion Queue <https://civicdb.org/curation/sources>`_ or by searching for the publication in the `Source Advanced Search <https://civicdb.org/search/sources/>`_ to find the dedicated CIViC publication page.

- Add a variant Alias.

  - Browse for variants you are familiar with using our `Browse <https://civicdb.org/browse/variants>`_ or `Advanced
    Search <https://civicdb.org/search/variants/>`_ pages.

- Read a summary for your favorite gene/variant and comment on the
  contents.

  - Use the `Browse <https://civicdb.org/browse/genes>`_ or `Advanced Search <https://civicdb.org/search/genes/>`_ pages to find your variant or gene of
    interest.
  - Use the `Activity Page <https://civicdb.org/activity>`_ to view recent activity. Clicking on any event will
    direct you to that event.

- Add a Variant Type.

  - Using the `Variant Advanced Search <https://civic.genome.wustl.edu/search/variants/8659ebdf-290f-4a0b-afa5-6146a3731e74>`_ page you can identify Variants without
    a Sequence Ontology Variant Type (e.g., Missense, Loss-of-function).
  - One you have identified a variant, clicking on one of the Variants in the
    list will take you to that page. Next to the Variant name, you will see a
    pencil icon which will take you to the edit page for that Variant.
