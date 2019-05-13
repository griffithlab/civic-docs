Genes
=====

For most users, the primary entry point for the CIViC API will be the Genes endpoint. This endpoint allows a user to retrieve information about what genes are in CIViC as well as get lists of variants for specific genes.

Get a list of genes
-------------------

This endpoint returns a listing of genes in CIViC that contain at least one evidence item. Returned gene listings contain variant ids which can be used to query for more detailed variant information. This is an index style endpoint and is `paginated` by default. You can use the ``count`` and ``page`` parameters to iterate through all the variants.

.. rubric:: HTTP Request Format
.. parsed-literal::

    GET https://civicdb.org/api/genes

.. rubric:: Query Parameters
.. list-table::
   :widths: 20 10 70
   :header-rows: 1

   * - Parameter
     - Default
     - Description
   * - page
     - 1
     - Which page of results to return
   * - count
     - 25
     - How many genes to return on a single page

.. rubric:: Example Request
.. parsed-literal::

    curl https://civicdb.org/api/genes

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   {
     "_meta": {
       "current_page": 1,
       "per_page": 25,
       "total_pages": 11,
       "total_count": 267,
       "links": {
         "next": "https://civicdb.org/api/genes?count=25&page=2",
         "previous": null
       }
     },
     "records": [
       {
         "id": 1,
         "name": "ALK",
         "entrez_id": 238,
         "description": "ALK amplifications, fusions and mutations have been shown to be driving events in non-small cell lung cancer. While crizontinib has demonstrated efficacy in treating the amplification, mutations in ALK have been shown to confer resistance to current tyrosine kinase inhibitors. Second-generation TKI's have seen varied success in treating these resistant cases, and the HSP90 inhibitor 17-AAG has been shown to be cytostatic in ALK-altered cell lines.",
         "variants": [
           {
             "name": "DEL4-11",
             "id": 550,
             "evidence_items": {
               "accepted_count": 1,
               "rejected_count": 0,
               "submitted_count": 0
             }
           },
           {
             "name": "CLTC-ALK",
             "id": 520,
             "evidence_items": {
               "accepted_count": 3,
               "rejected_count": 0,
               "submitted_count": 0
             }
           },
           {
             "name": "EML4-ALK  V1180L",
             "id": 528,
             "evidence_items": {
               "accepted_count": 5,
               "rejected_count": 0,
               "submitted_count": 0
             }
           },
         ],
         "aliases": [
           "NBLST3",
           "CD246"
         ],
         "type": "gene"
       },
       {
         "id": 2,
         "name": "AKT1",
         "entrez_id": 207,
         "description": "AKT1, also referred to as protein kinase B, is a known oncogene. AKT activation relies on the PI3K pathway, and is recognized as a critical node in the pathway. The E17 hotspot is the most characterized of AKT1 mutations, and has been shown to result in activation of the protein. Mutations in AKT1 have also been shown to confer resistance to allosteric kinase inhibitors in vitro.",
         "variants": [
           {
             "name": "Q79K",
             "id": 169,
             "evidence_items": {
               "accepted_count": 1,
               "rejected_count": 0,
               "submitted_count": 0
             }
           }
         ],
         "aliases": [
           "RAC-ALPHA",
           "PKB",
           "AKT",
           "PKB-ALPHA",
           "RAC",
           "CWS6",
           "PRKBA"
         ],
         "type": "gene"
       },
     ]
   }

Get details for a specific gene
-------------------------------

This endpoint retrieves details about a specific gene.

Note that the default behavior of this endpoint is to use internal CIViC ids. If you want to use Entrez ids or gene symbols, you need to specify the ``identifier_type`` parameter.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/genes/:id

.. rubric:: Query Parameters
.. list-table::
   :widths: 20 10 70
   :header-rows: 1

   * - Parameter
     - Valid Values
     - Description
   * - identifier_type
     - ``entrez_id``, ``entrez_symbol``, ``civic_id``
     - Type of gene identifier used in your query

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/genes/ALK?identifier_type=entrez_symbol

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   {
     "id": 1,
     "name": "ALK",
     "entrez_id": 238,
     "description": "ALK amplifications, fusions and mutations have been shown to be driving events in non-small cell lung cancer. While crizontinib has demonstrated efficacy in treating the amplification, mutations in ALK have been shown to confer resistance to current tyrosine kinase inhibitors. Second-generation TKI's have seen varied success in treating these resistant cases, and the HSP90 inhibitor 17-AAG has been shown to be cytostatic in ALK-altered cell lines.",
     "variants": [
       {
         "name": "EML4-ALK L1152R",
         "id": 307,
         "evidence_items": {
           "accepted_count": 1,
           "rejected_count": 0,
           "submitted_count": 0
         }
       },
       {
         "name": "F1245C",
         "id": 549,
         "evidence_items": {
           "accepted_count": 2,
           "rejected_count": 0,
           "submitted_count": 0
         }
       },
     ],
     "aliases": [
       "NBLST3",
       "CD246"
     ],
     "type": "gene",
     "variant_groups": [
       {
         "id": 11,
         "name": "ALK Fusions",
         "description": "ALK fusion positive non-small cell lung cancer (NSCLC) is treated as its own subset of NSCLC. Many ALK fusions that have been seen as recurrent in cancer serve to increase the activity of the ALK oncogene relative to normal cells. While EML4 is the most common fusion partner, other 5' partners have been observed. The EML4-ALK fusion has shown sensitivity to targeted tyrosine kinase inhibitors such as crizotinib. ",
         "variants": [
           {
             "id": 520,
             "entrez_name": "ALK",
             "gene_id": 1,
             "entrez_id": 238,
             "name": "CLTC-ALK",
             "description": "The t(2;17)(p23;q23) translocation results in the CLTC-ALK fusion protein, the most common ALK fusion observed in diffuse large B cell lymphoma (DLBCL). ALK-rearranged DLBCL is less responsive to CHOP chemotherapy. Preclinical work indicates that CLTC-ALK DLBCL is responsive to ALK inhibition in cell lines and mouse models, and two case studies show short response followed by progression when heavily pretreated and advanced ALK-positive DLBCL is treated with crizotinib (one case CLTC-ALK, one case an unknown ALK fusion).",
             "type": "variant",
             "variant_types": [
               {
                 "id": 120,
                 "name": "transcript_fusion",
                 "display_name": "Transcript Fusion",
                 "so_id": "SO:0001886",
                 "description": "A feature fusion where the deletion brings together transcript regions.",
                 "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001886"
               }
             ],
             "evidence_items": {
               "accepted_count": 3,
               "rejected_count": 0,
               "submitted_count": 0
             },
             "coordinates": {
               "chromosome": "17",
               "start": "57697219",
               "stop": "57768072",
               "reference_bases": null,
               "variant_bases": null,
               "representative_transcript": "ENST00000269122.3",
               "chromosome2": "2",
               "start2": "29415640",
               "stop2": "29446394",
               "representative_transcript2": "ENST00000389048.3",
               "ensembl_version": 75,
               "reference_build": "GRCh37"
             }
           },
           {
             "id": 514,
             "entrez_name": "ALK",
             "gene_id": 1,
             "entrez_id": 238,
             "name": "RANBP2-ALK",
             "description": "",
             "type": "variant",
             "variant_types": [
               {
                 "id": 120,
                 "name": "transcript_fusion",
                 "display_name": "Transcript Fusion",
                 "so_id": "SO:0001886",
                 "description": "A feature fusion where the deletion brings together transcript regions.",
                 "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001886"
               }
             ],
             "evidence_items": {
               "accepted_count": 1,
               "rejected_count": 0,
               "submitted_count": 0
             },
             "coordinates": {
               "chromosome": "2",
               "start": "109335937",
               "stop": "109375004",
               "reference_bases": null,
               "variant_bases": null,
               "representative_transcript": "ENST00000283195.6",
               "chromosome2": "2",
               "start2": "29415640",
               "stop2": "29446394",
               "representative_transcript2": "ENST00000389048.3",
               "ensembl_version": 75,
               "reference_build": "GRCh37"
             }
           },
         ],
         "type": "variant_group"
       }
     ],
     "lifecycle_actions": {},
     "sources": [
       {
         "id": 2,
         "name": "ALK in lung cancer: past, present, and future.",
         "citation": "Shaw et al., 2013, J. Clin. Oncol.",
         "pubmed_id": "23401436",
         "source_url": "http://www.ncbi.nlm.nih.gov/pubmed/23401436",
         "open_access": true,
         "pmc_id": "PMC4209068",
         "publication_date": {
           "year": 2013,
           "month": 3,
           "day": 10
         },
         "journal": "J. Clin. Oncol.",
         "full_journal_title": "Journal of clinical oncology : official journal of the American Society of Clinical Oncology",
         "status": "fully curated"
       }
     ],
     "errors": {}
   }

Get several genes at once via an identifier
-------------------------------------------

The endpoint can be used to fetch overview information for multiple genes at the same time. It supports the same ``identifier_types`` as the detail endpoint.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/genes/:id1,:id2

.. rubric:: Query Parameters
.. list-table::
   :widths: 20 10 70
   :header-rows: 1

   * - Parameter
     - Valid Values
     - Description
   * - identifier_type
     - ``entrez_id``, ``entrez_symbol``, ``civic_id``
     - Type of gene identifier used in your query

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/genes/TP53,BRAF?identifier_type=entrez_symbol

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   [
     {
       "id": 5,
       "name": "BRAF",
       "entrez_id": 673,
       "description": "BRAF mutations are found to be recurrent in many cancer types. Of these, the mutation of valine 600 to glutamic acid (V600E) is the most prevalent. V600E has been determined to be an activating mutation, and cells that harbor it, along with other V600 mutations are sensitive to the BRAF inhibitor dabrafenib. It is also common to use MEK inhibition as a substitute for BRAF inhibitors, and the MEK inhibitor trametinib has seen some success in BRAF mutant melanomas. BRAF mutations have also been correlated with poor prognosis in many cancer types, although there is at least one study that questions this conclusion in papillary thyroid cancer.",
       "variants": [
         {
           "name": "D594G",
           "id": 611,
           "evidence_items": {
             "accepted_count": 3,
             "rejected_count": 0,
             "submitted_count": 0
           }
         },
         {
           "name": "L597V",
           "id": 585,
           "evidence_items": {
             "accepted_count": 1,
             "rejected_count": 0,
             "submitted_count": 0
           }
         },
       ],
       "aliases": [
         "RAFB1",
         "NS7",
         "BRAF1",
         "B-RAF1"
       ],
       "type": "gene"
     },
     {
       "id": 45,
       "name": "TP53",
       "entrez_id": 7157,
       "description": "TP53 mutations are universal across cancer types. Loss of tumor suppressors is most recognized by large deleterious events, such as frameshift mutations, or premature stop codons. In TP53 however, many of the observed mutations in cancer are found to be single nucleotide variants, or missense mutations. These variants are also very broadly distributed throughout the gene, not localizing in any particular hotspot. While a large proportion of cancer genomics research is focused on somatic variants, TP53 is also of note in the germline. Germline TP53 mutations are the hallmark of Li-Fraumeni syndrome, and many (both germline and somatic) have been found to have prognostic impact on patient outcomes. The significance of many polymorphisms in susceptibility and prognosis of disease is still very much up for debate.",
       "variants": [
         {
           "name": "P72R",
           "id": 531,
           "evidence_items": {
             "accepted_count": 3,
             "rejected_count": 0,
             "submitted_count": 0
           }
         },
       ],
       "aliases": [
         "TRP53",
         "P53",
         "LFS1",
         "BCC7"
       ],
       "type": "gene"
     }
   ]


