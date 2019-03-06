Getting started as a CIViC Curator
==================================

CIViC curators are a community of users dedicated to improving the CIViC
knowledgebase and its contents.

Prerequisites:

- Create an account. Creating an account requires only that you have login
  creditials for one of our supported OAuth providers (currently Google, ORCiD,
  or GitHub).

Although curators are not required to have any specific training, background
or skill set, curator-generated content can only be "Accepted" once it is
reviewed by a CIViC Editor. Editors are experts in cancer genomics, oncology,
pathology and other relevant fields. This gate-keeper model allows significant
contributions from curators with any level of experience while maintaining the
quality of an expert-driven resource. Curators can be promoted to Editors once
they have demonstrated sufficient understanding of the CIViC data model and
requirements for cancer variant interpretation.

Even small contributions can make a big impact on how up-to-date and
comprehensive the CIViC resource is. Examples of small curation activities
include: commenting on existing entries, identifying additional literature
sources, improving the wording of a variant interpretation, adding variant IDs
or aliases, etc.

.. content-tabs::

  .. tab-container:: tab1
     :title: Introductory Materials

     **The Cancer Analysis Bottleneck**

     With the recent advent of rapid and affordable tumor genome sequencing,
     interpreting the clinical significance of cancer variants from the wealth
     of existing and rapidly evolving medical literature has become a major
     bottleneck to realizing the potential of precision cancer medicine.

     Associating cancer variants with concrete clinical actions by manual
     curation of high quality evidence is a great challenge. Creating useful
     interpretations requires integrating complex information from diverse
     sources ranging from preclinical lab experiments to clinical trial
     results. Creating and maintaining such interpretations will require the
     concerted effort of many experts at a large scale.

     *Recommended reading:* `Organizing knowledge to enable personalization of
     medicine in cancer <https://www.ncbi.nlm.nih.gov/pubmed/25222080>`_

     **Cancer Variant Interpretation - Evidence Statements, Variant Summaries
     and Gene Summaries**

     For a primer on the fundamentals of cancer variant interpretation, we
     highly recommend that new users start by reading the CIViC paper and
     three recently published Standards and Guidelines proposals:

     - `CIViC is a community knowledgebase for expert crowdsourcing the clinical
       interpretation of variants in cancer.
       <http://www.nature.com/ng/journal/v49/n2/full/ng.3774.html>`_
     - `ACMG/AMP - Standards and guidelines for the interpretation of sequence
       variants. <https://www.ncbi.nlm.nih.gov/pubmed/25741868>`_
     - `ClinGen - Somatic cancer variant curation and harmonization through
       consensus minimum variant level data (MVLD).
       <https://www.ncbi.nlm.nih.gov/pubmed/27814769>`_
     - `AMP/ASCO/CAP - Standards and guidelines for the interpretation and
       reporting of sequence variants in cancer.
       <https://www.ncbi.nlm.nih.gov/pubmed/27993330>`_

  .. tab-container:: tab2
     :title: Example Activities

     Most of the contents of CIViC are curator generated and edited. Below are
     a few examples of areas where curators are needed, culminating in a list
     of bite sized curation tasks that should require less than 3 minutes of
     your time.

     **1. Adding Evidence**

     Evidence records are the heart of the CIViC resource. Each
     corresponds to evidence for a single clinical assertion about a
     single variant in a single cancer type. Each evidence record is
     based on a single citable source (e.g. a peer-reviewed
     publication). The evidence record consists of a free-form
     executive summary describing the assertion and supporting
     evidence for it, and additional structured fields that describe
     the evidence (e.g. evidence type, relevant drug, etc.). To learn
     more about the elements of an evidence record refer to the
     :doc:`Evidence help docs <evidence>`. For suggestions on where to find sources for
     evidence records, refer to the Source Ideas tab of this section.
     To add a new evidence record, you must login and hit the "ADD"
     button at the top of any page throughout the site.

     **2. Adding or improving Variant, Variant Group, and Gene Summaries**

     Once sufficient evidence accumulates for a variant, variant group
     or gene entity, a summary should be created. The summary should
     be an overview of the evidence records associated with the
     entity. The summary should focus on the most clinically
     actionable evidence and should summarize for each relevant gene
     what a clinician should be aware of for patients with a
     particular variant, or variants in a particular gene. Very brief
     background material may be included. Additional citations beyond
     those associated with the evidence records can be associated
     directly with the summary using the "Add Source" option in the
     edit form. To learn more about each major CIViC entity, refer to
     the :doc:`variants`, :doc:`variant_groups`, and :doc:`genes` sections of the help
     pages.

     **3. Editing CIViC Content**

     CIViC content can be edited by clicking on the pencil icon as
     displayed for an example Variant here:

     **VARIANT V600E**

     Gene, Variant, Variant Group and Evidence entities can all be edited.
     These edits may be expansive major updates to incorporate new evidence,
     error corrections, improvements to readability and style, or minor
     grammar and typo fixes. All such edits are welcome.

     **4. Comment on CIViC Content**

     Throughout the website are "Talk" pages where users can comment
     on the current contents of CIViC (specific Evidence, Variants or
     Genes) or on Suggested Changes. Curators are encouraged to be
     verbose in their comments on existing content. Critism,
     clarification, qualification, and questions are all appropriate.
     Comments from the authors of work being summarized or others with
     particular expertise in the area are especially desirable. When
     adding new evidence or summaries, comments may be used to
     describe the thought process of the curator. Small quotes (as
     allowed by the Fair Use doctrine) from source publications that
     support a submission may also be included (but please indicate
     these with quotes or use the block quote style).

     **5. Variant attributes**

     In addition to the variant summary (discussed above), there are
     several other structured values associated with variant records.
     These include:

     - **Aliases.** Alternative names (synonyms) for the variant. For many variants,
       researchers from different groups may refer to variants by different
       names. Multiple and varying abbreviations or identifiers exist for most
       variants. A variant alias is generally any name the might help CIViC
       users determine the various ways used to indicate the same variant.
     - **HGVS expressions.** CIViC supports and promotes variant identification
       using the `Sequence Variant Nomenclature <http://varnomen.hgvs.org/>`_ guidelines of the Human Genome
       Variation Society (HGVS), otherwise known as 'HGVS strings'. Curators may
       add one or more valid HGVS values for each variant. These may be entered
       in protein (p.), cDNA (c.), or genomic (g.) format. A particular CIViC
       variant (e.g. BRAF V600E) may have multiple valid genomic alterations
       that could create it, each with a distinct genomic HGVS expression.
       Similarly, multiple cDNA HGVS strings may correspond to multiple
       transcript sequences, possibly from various transcript annotation
       databases (e.g. Ensembl, RefSeq, LRG, etc.) or alternative isoforms of a
       gene.
     - **Coordinates.** For each variant, the goal of CIViC initially is to
       determine unambiguous genomic coordinates for an example instance of the
       variant. For instance, if the paper refers to the variant as "V600E", the
       curator determines for a particular build of the human genome, the
       corresponding chromosome, start position, end position, reference base
       and variant base. Refer to the :doc:`Variants documentation <variants>` on the left for
       more details.

     **6. Bite-size curation tasks**

     Only have a few minutes? Tackle one of the tasks below.

     - `Suggest a Source <https://civicdb.org/suggest/source>`_.

       - Identify a publication containing a variant with clinical relevance.
       - Visit PubMed to identify the publication's `PubMed
         <https://www.ncbi.nlm.nih.gov/pubmed/>`_ ID.
       - Enter as much information possible to help curators. This form only
         requires 2 elements: PubMed ID and a comment to direct curators as to why
         you believe this publication has clinically-relevant information about a
         variant.
       - Your suggested source can be seen in the `Source Suggestion Queue <https://civicdb.org/curation/sources>`_ or by
         searching for the publication in the `Source Advanced Search <https://civicdb.org/search/sources/>`_ to find the
         dedicated CIViC publication page.

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

  .. tab-container:: tab3
     :title: Source Ideas

     New CIViC curators, commonly ask where they should focus their efforts
     and where can they find evidence of the clinical significance of cancer
     variants. There are many approaches and relevant resources that may help
     to identify and prioritize such evidence.

     Remember that the focus of CIViC is on the **clinical** relevance of **cancer**
     variants. Before expending the effort to propose an addition to CIViC,
     ask yourself would a clinician potentially find this information useful
     in understanding and treating a patient's cancer? Could an oncologist use
     this evidence to better understand likely response to therapy (Predictive
     evidence), or outcome (Prognostic) for their patient? Would a pathologist
     find knowledge of the variant valuable in classifying (Diagnostic) the
     tumor into a subtype? Would a medical geneticist or genetic counselor be
     interested in the causative (Predisposing) significance of this evidence?

     In addressing these questions, try to think about the distinction between
     the relevance of a variant to cancer biology and its relevance in a
     clinical setting. A variant may have great and diverse relevance to the
     biology of a cancer cell but have limited or no clinical applicability.
     For example, TP53 mutations are critical in many cancers and hundreds (if
     not thousands) of papers have been written about their complex roles in
     cancer biology. However, the scenarios in which TP53 mutations are
     **clinically** relevant are much, much narrower. A variant may NOT be
     clinically relevant despite being characterized as functional (gain or
     loss of function), a 'driver', 'recurrent', etc. In some, perhaps most
     cases, the clinical relevance of these variants may simply not be
     established yet. However, CIViC is about the **evidence that establishes
     their clinical relevance**. By contrast, in some cases, the biological
     relevance may be poorly understood while clinical utlity is established.
     Such evidence does belong in CIViC. A mechanistic understanding is
     desirable, but not required.

     The above description, despite it length, is an oversimplification. The
     concept of clinical utility varies by Evidence type: Predictive,
     Prognostic, Diagnostic and Predisposing. There are many nuances to be
     considered. The "ideal" clinical interpretation and definition of
     clinical utility are open to debate. We welcome this debate and one of
     the goals of CIViC is to enable and capture it. If you believe some
     evidence is relevant to CIViC but have some doubts, please submit it so
     that the community can discuss with you.

     The following list is not exhaustive but provides many examples of
     approaches to identify high quality evidence. If you know of a useful
     resource that is not listed below, please let us know about it. NOTE:
     some of these resources are open access, others are not. When entering
     evidence into CIViC, **never** copy content or ideas from another resource.
     Your contributions to CIViC should be based on published evidence, but in
     your own words.

     **Example sources of CIViC evidence and high priority variants**

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

  .. tab-container:: tab4
     :title: Monitoring

     CIViC curation is meant to function as a community effort with multiple
     curators discussing and editors reviewing all content. For this reason it
     is valuable as a curator to know when your contributions are being
     discussed, modified, and reviewed. Curators can monitor their activity in
     a variety of ways, depending on the updates desired.

     **User Profile**

     From your User Profile, a curator can see cumulative statistics of CIViC
     activities, a table of your submitted evidence items, and your most
     recent activity:

     1. A curator's cumulative statistics are displayed in the top right. These
        statistics contribute to your rank in different categories on the
        `Community Page <https://civicdb.org/community/main>`_.
     2. The Evidence table shows all of a curator's submitted evidence items and
        their current state (Submitted, Accepted, Rejected). Here are some tips
        for exploring this table:

        - Custom sort by clicking on the column headers.
        - Filter using the text boxes below the column headers.
        - Download using the "Get Data" button at any time.
        - By default, Rejected Evidence Items are hidden but can be displayed using
          the button in the top right corner of the Evidence grid.

     3. Recent activity is shown below the Evidence table where the last 25
        actions you have performed in CIViC are displayed for quick reference.
        Clicking on an event will redirect your browser to that action.

     **Notifications**

     Actions within CIViC by any curator trigger event notifications. You are
     automatically subscribed to an Evidence, Variant or Gene notification
     stream by submitting, suggesting revisions, or commenting on one of these
     entities in CIViC, allowing you to monitor subsequent activity related to
     the content you care about most in CIViC.

     Mentions are a specific class of notifications triggered by other users.
     By using @username notation, other curators can draw special attention to
     a revision, comment or other CIViC entity specifically targeted at the
     mentioned curator. These are typically used when a curator or editor
     requires your input or action, although they can be used when a response
     is specifically targeted to another user.

     If you are logged into CIViC and have notifications pending, this will be
     indicated in the top right corner of the site with a number beside your
     username. To view your notifications open the drop down menu beside your
     username and selected "Subscribed events" or "Mentions" option. If you do
     not have any active notifications, you can always see your notification
     history by selecting the "My Account" option. On the notifications page,
     you can browse and filter notifications and mark them as read. To view
     past notifications marked as read, select "All" or "Mentions" on the
     left, and check the "Show Read" option.

     **Community Page**

     The Community Page includes a leaderboard and a list of current curators,
     editors and admins using CIViC.

     - The Leaderboard can be used to identify other users that you may want to
       direct Mentions to when you have specific questions about actions in
       CIViC. Seeing your own username on the Leaderboard simply requires
       increasing your personal statistics shown on your User Profile page to
       become one of the top users in that category.
     - Finding usernames, user roles and user profiles can be best accomplished
       through the User listing on the Community Page.
