Introduction to CIViC
=====================

The Clinical Interpretation of Variants in Cancer (CIViC) knowledgebase is a free and open resource for public use, available online at `civicdb.org <http://civicdb.org>`_. To get started using and contributing to CIViC, we recommend that you :doc:`review the Video Tutorials <using/videos>`. These videos cover CIViC and its goals; finding documentation and help resources; browsing and searching knowledgebase contents; adding new evidence, variant summaries, coordinates, gene summaries, and assertions to CIViC; and editing existing CIViC content.

For a primer on the fundamentals of cancer variant interpretation, we highly recommend that new users start by reading the CIViC paper and these recently published Standards and Guidelines proposals:

- `CIViC is a community knowledgebase for expert crowdsourcing the clinical interpretation of variants in cancer. <http://www.nature.com/ng/journal/v49/n2/full/ng.3774.html>`_
- `Standard operating procedure for curation and clinical interpretation of variants in cancer. <https://www.ncbi.nlm.nih.gov/pubmed/31779674>`_
- `ACMG/AMP - Standards and guidelines for the interpretation of sequence variants. <https://www.ncbi.nlm.nih.gov/pubmed/25741868>`_
- `ClinGen - Somatic cancer variant curation and harmonization through consensus minimum variant level data (MVLD). <https://www.ncbi.nlm.nih.gov/pubmed/27814769>`_
- `AMP/ASCO/CAP - Standards and guidelines for the interpretation and reporting of sequence variants in cancer. <https://www.ncbi.nlm.nih.gov/pubmed/27993330>`_
- `ClinGen/CGC/VICC - Standards for the classification of pathogenicity of somatic variants in cancer (oncogenicity). <https://pubmed.ncbi.nlm.nih.gov/35101336/>`_
- `Evaluating the Clinical Validity of Gene-Disease Associations: An Evidence-Based Framework Developed by the Clinical Genome Resource <https://www.ncbi.nlm.nih.gov/pubmed/28552198>`_
- `Standardized decision support in next generation sequencing reports of somatic cancer variants <https://www.ncbi.nlm.nih.gov/pubmed/24768039>`_

The CIViC Ecosystem of Collaborators, Moderators, and Other Stakeholders
------------------------------------------------------------------------

The CIViC project aims to facilitate a collaborative ecosystem of research scientists, clinical scientists, and patient advocates dedicated to curating an accurate and relevant knowledgebase of clinical interpretations of cancer variants. A principle goal of CIViC is to systematically document the evidence that supports any variant interpretation. The diagram below shows how the various stakeholders in the CIViC ecosystem collaborate to curate and utilize the knowledgebase.

.. thumbnail:: images/GP-125_CIViC_main-process_v5b.png
   :alt: Figure depicting the CIViC Ecosystem of Collaborators, Moderators, and Other Stakeholders
   :title: The CIViC Ecosystem of Collaborators, Moderators, and Other Stakeholders
   :show_caption: True

|

Using the CIViC Help Docs
-------------------------
Navigate the CIViC Help Docs with the navigation menu to the left of each page or the Table of Contents below. :doc:`About <about>` pages provide a high level overview of the CIViC resource. :doc:`Using CIViC <using>` pages provide detailed instructions (including videos) on how to browse, search, and use CIViC data. :doc:`Curating CIViC <curating>` pages provide general instruction for contributor (curators and editors) on how to add content to the knowledgebase and :doc:`CIViC Knowledge Model <model>` pages provide detailed definitions and curation instruction for each concept/field in CIViC. Finally, :doc:`CIViC API <api>` and :doc:`Get Help <help>` pages provide additional guidance on using the CIViC API and getting more help.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   about
   model
   curating
   using
   api
   help

..
   Kludge to make aliases file importable using hidden table of contents -
   Without this, Sphinx will display warnings about an unlinked file

..
   .. toctree::
      :hidden:

      generated/civic-docs.aliases.rst
