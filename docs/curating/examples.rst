Examples
========

Most of the contents of CIViC are curator generated and edited. Below are a few examples of areas where curators are needed, culminating in a list of bite sized curation tasks that should require less than 3 minutes of your time.

.. rubric:: 1. Adding Evidence

Evidence records are the heart of the CIViC resource. Each corresponds to evidence for a single clinical assertion about a single variant in a single cancer type. Each evidence record is based on a single citable source (e.g. a peer-reviewed publication). The evidence record consists of a free-form executive summary describing the assertion and supporting evidence for it, and additional structured fields that describe the evidence (e.g. evidence type, relevant drug, etc.). To learn more about the elements of an evidence record refer to the :doc:`Evidence help docs <../model/evidence>`. For suggestions on where to find sources for evidence records, refer to the Source Ideas tab of this section. To add a new evidence record, you must login and hit the "ADD" button at the top of any page throughout the site.

.. rubric::  Adding or improving Variant, Variant Group, and Gene Summaries

Once sufficient evidence accumulates for a variant, variant group or gene entity, a summary should be created. The summary should be an overview of the evidence records associated with the entity. The summary should focus on the most clinically actionable evidence and should summarize for each relevant gene what a clinician should be aware of for patients with a particular variant, or variants in a particular gene. Very brief background material may be included. Additional citations beyond those associated with the evidence records can be associated directly with the summary using the "Add Source" option in the edit form. To learn more about each major CIViC entity, refer to the :doc:`../model/variants`, :doc:`../model/variant_groups`, and :doc:`../model/genes` sections of the help pages.

.. rubric:: 3. Editing CIViC Content

CIViC content can be edited by clicking on the pencil icon as displayed for an example Variant here:

.. rubric:: VARIANT V600E

Gene, Variant, Variant Group and Evidence entities can all be edited. These edits may be expansive major updates to incorporate new evidence, error corrections, improvements to readability and style, or minor grammar and typo fixes. All such edits are welcome.

.. rubric:: 4. Comment on CIViC Content

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
