Genes
=====

CIViC provides a curated summary of the clinical relevance of genes, as well
as data pulled from the MyGeneInfo database. The gene summary includes the
gene's relevance to different cancer types, patient outcomes and treatment
decisions. It may also include information about the gene product's pathway
interactions, functional alterations caused by variants within the gene, and
normal functions that are relevant to its association with cancer.

.. content-tabs::

  .. tab-container:: tab1
     :title: Overview

     In order to be listed in CIViC a Gene must have at least one clinical
     Evidence Item that has been curated from the literature. A new Gene
     record will be created automatically when the first Evidence Item is
     assigned to that Gene. The official gene name according to Entrez Gene
     (assigned by HGNC) is used. Alternative gene names are autopopulated from
     MyGeneInfo and searchable throughout the database. However, new Evidence
     Items must be associated with an official gene symbol to reduce
     ambiguity.

     .. list-table::
        :widths: 15 75 10
        :header-rows: 1

        * - Attribute
          - Description
          - Source
        * - Name
          - Entrez symbol of the gene.
          - EntrezDB
        * - Summary
          - User-defined summary of the clinical relevance of this
            Gene. Curation efforts should aim to concisely summarize the
            relevance of variants in this gene to treatment prediction,
            prognosis, and diagnosis. The summary should also provide an
            overview of the most relevant cancer types. The summary may also
            include relevant mechanistic information such as pathway
            interactions, functional alterations caused by variants within this
            Gene (i.e., activating, loss-of-function, etc.), and normal
            functions key to its oncogenic properties.
          - CIViC
        * - Sources (PubMed IDs)
          - A list of PubMed IDs referring to evidence supporting
            statements made in the Gene's description. Source descriptions (e.g.
            'Weisberg et al., 2007, Nat. Rev. Cancer') are pulled from the
            PubMed database at the time of submission, and are not editable.
          - CIViC (PubMed)
        * - **MyGene.Info**
          -
          -
        * - MyGene Info
          - Data retrieved from MyGene.Info using the HGNC symbol
            as the query. Includes synonyms, protein domains, and pathways with
            additional data displayed by clicking the "Details" button.
          - MyGene.Info

  .. tab-container:: tab2
     :title: Gene Summary

     This is a user-defined description of the clinical relevance of this
     gene. Just as a Variant Summary should be a synthesis of Evidence
     Statements for a Variant, the Gene Summary should be a synthesis of the
     Variant Summaries for a Gene.

     This summary should also discuss the relevance of the Gene to different
     cancer types, patient outcomes and treatment decisions, and highlight
     differences and similarities between different variants of this gene.
     This section may include information about the gene product’s pathway
     interactions, functional alterations caused by variants within this gene
     and normal functions that are relevant to its association with cancer.
     Although individual evidence statements do not capture
     biological/mechanistic impact of variants on gene function, the Gene
     Summary is a place where this information may be summarized.

     **Sources**

     Although in-line citations are not currently supported, citations can be
     tracked using the Sources field and entered by specifying the PubMed ID
     associated with the publication. The addition of citations used to
     generate the gene description, particularly relevant reviews, is highly
     encouraged with the intention of directing other users to more in-depth
     information.
