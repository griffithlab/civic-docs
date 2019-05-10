Variant Groups
==============

The variant groups endpoint allows users to enumerate all of the variant groups in CIViC and view their membership.

Get a list of variant groups
----------------------------

This endpoint returns a listing of variant groups in CIViC. This index style endpoint is `paginated` by default. You can use the ``count`` and ``page`` parameters or the ``previous`` and ``next`` links to iterate through all the variant groups.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/variant_groups

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
     - How many variant groups to return on a single page

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/variant_groups

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   {
     "_meta": {
       "current_page": 1,
       "per_page": 20,
       "total_pages": 1,
       "total_count": 20,
       "links": {
         "next": null,
         "previous": null
       }
     },
     "records": [
       {
         "id": 1,
         "name": "Imatinib Resistance",
         "description": "While imatinib has shown to be incredibly successful in treating philadelphia chromosome positive CML, patients that have shown primary or secondary resistance to the drug have been observed to harbor T315I and E255K ABL kinase domain mutations. These mutations, among others, have been observed both in primary refractory disease and acquired resistance. In gastrointestinal stromal tumors (GIST), PDGFRA 842 mutations have also been shown to confer resistance to imatinib. ",
         "variants": [
           {
             "id": 3,
             "entrez_name": "ABL1",
             "gene_id": 4,
             "entrez_id": 25,
             "name": "BCR-ABL E255K",
             "description": "While the efficacy of imatinib has revolutionized chronic myelogenous leukemia (CML) treatment, it is still not a cure-all. Both initial resistance and acquired resistance as a result of selection have been seen in a small subset of CML patients. The ABL kinase domain mutation E255K has been shown to be one such mutation that confers resistance to imatinib. Second generation TKI's (dasatinib and nilotinib) specific to BCR-ABL have shown efficacy in treating resistant cases.",
             "type": "variant",
             "variant_types": [
               {
                 "id": 120,
                 "name": "transcript_fusion",
                 "display_name": "Transcript Fusion",
                 "so_id": "SO:0001886",
                 "description": "A feature fusion where the deletion brings together transcript regions.",
                 "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001886"
               },
             ],
             "evidence_items": {
               "accepted_count": 1,
               "rejected_count": 0,
               "submitted_count": 0
             },
             "coordinates": {
               "chromosome": "9",
               "start": "133738363",
               "stop": "133738363",
               "reference_bases": "G",
               "variant_bases": "A",
               "representative_transcript": "ENST00000318560.5",
               "chromosome2": null,
               "start2": null,
               "stop2": null,
               "representative_transcript2": null,
               "ensembl_version": 75,
               "reference_build": "GRCh37"
             }
           },
           {
             "id": 101,
             "entrez_name": "PDGFRA",
             "gene_id": 38,
             "entrez_id": 5156,
             "name": "I843DEL",
             "description": "PDGFRA D842 mutations are characterized broadly as imatinib resistance mutations. This is most well characterized in gastrointestinal stromal tumors, but other cell lines containing these mutations have been shown to be resistant as well. In imatinib resistant cell lines, a number of other therapeutics have demonstrated efficacy. These include; crenolanib, sirolimus, and midostaurin (PKC412).",
             "type": "variant",
             "variant_types": [
               {
                 "id": 107,
                 "name": "inframe_deletion",
                 "display_name": "Inframe Deletion",
                 "so_id": "SO:0001822",
                 "description": "An inframe non synonymous variant that deletes bases from the coding sequence.",
                 "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001822"
               }
             ],
             "evidence_items": {
               "accepted_count": 2,
               "rejected_count": 0,
               "submitted_count": 0
             },
             "coordinates": {
               "chromosome": "4",
               "start": "55152095",
               "stop": "55152097",
               "reference_bases": "ATC",
               "variant_bases": null,
               "representative_transcript": "ENST00000257290.5",
               "chromosome2": null,
               "start2": null,
               "stop2": null,
               "representative_transcript2": null,
               "ensembl_version": 75,
               "reference_build": "GRCh37"
             }
           },
           {
             "id": 102,
             "entrez_name": "PDGFRA",
             "gene_id": 38,
             "entrez_id": 5156,
             "name": "DI842-843VM",
             "description": "PDGFRA D842 mutations are characterized broadly as imatinib resistance mutations. The DI842-843VM variant is the result of a double point mutation. This is most well characterized in gastrointestinal stromal tumors, but other cell lines containing these mutations have been shown to be resistant as well. In imatinib resistant cell lines, a number of other therapeutics have demonstrated efficacy. These include; crenolanib, sirolimus, and midostaurin (PKC412).",
             "type": "variant",
             "variant_types": [
               {
                 "id": 47,
                 "name": "missense_variant",
                 "display_name": "Missense Variant",
                 "so_id": "SO:0001583",
                 "description": "A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.",
                 "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001583"
               }
             ],
             "evidence_items": {
               "accepted_count": 1,
               "rejected_count": 0,
               "submitted_count": 0
             },
             "coordinates": {
               "chromosome": "4",
               "start": "55152093",
               "stop": "55152097",
               "reference_bases": "ACATC",
               "variant_bases": "TCATG",
               "representative_transcript": "ENST00000257290.5",
               "chromosome2": null,
               "start2": null,
               "stop2": null,
               "representative_transcript2": null,
               "ensembl_version": 75,
               "reference_build": "GRCh37"
             }
           },
           {
             "id": 98,
             "entrez_name": "PDGFRA",
             "gene_id": 38,
             "entrez_id": 5156,
             "name": "D842I",
             "description": "PDGFRA D842 mutations are characterized broadly as imatinib resistance mutations. This is most well characterized in gastrointestinal stromal tumors, but other cell lines containing these mutations have been shown to be resistant as well. In imatinib resistant cell lines, a number of other therapeutics have demonstrated efficacy. These include; crenolanib, sirolimus, and midostaurin (PKC412).",
             "type": "variant",
             "variant_types": [
               {
                 "id": 47,
                 "name": "missense_variant",
                 "display_name": "Missense Variant",
                 "so_id": "SO:0001583",
                 "description": "A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.",
                 "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001583"
               }
             ],
             "evidence_items": {
               "accepted_count": 1,
               "rejected_count": 0,
               "submitted_count": 0
             },
             "coordinates": {
               "chromosome": "4",
               "start": "55152092",
               "stop": "55152093",
               "reference_bases": "GA",
               "variant_bases": "AT",
               "representative_transcript": "ENST00000257290.5",
               "chromosome2": null,
               "start2": null,
               "stop2": null,
               "representative_transcript2": null,
               "ensembl_version": 75,
               "reference_build": "GRCh37"
             }
           },
         ],
         "type": "variant_group"
       },
     ]
   }

Get details for a specific variant group
----------------------------------------

This endpoint retrieves details about a specific variant group, given its internal CIViC id.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/variant_groups/:id

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/variant_groups/1

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   {
     "id": 1,
     "name": "Imatinib Resistance",
     "description": "While imatinib has shown to be incredibly successful in treating philadelphia chromosome positive CML, patients that have shown primary or secondary resistance to the drug have been observed to harbor T315I and E255K ABL kinase domain mutations. These mutations, among others, have been observed both in primary refractory disease and acquired resistance. In gastrointestinal stromal tumors (GIST), PDGFRA 842 mutations have also been shown to confer resistance to imatinib. ",
     "variants": [
       {
         "id": 3,
         "entrez_name": "ABL1",
         "gene_id": 4,
         "entrez_id": 25,
         "name": "BCR-ABL E255K",
         "description": "While the efficacy of imatinib has revolutionized chronic myelogenous leukemia (CML) treatment, it is still not a cure-all. Both initial resistance and acquired resistance as a result of selection have been seen in a small subset of CML patients. The ABL kinase domain mutation E255K has been shown to be one such mutation that confers resistance to imatinib. Second generation TKI's (dasatinib and nilotinib) specific to BCR-ABL have shown efficacy in treating resistant cases.",
         "type": "variant",
         "variant_types": [
           {
             "id": 120,
             "name": "transcript_fusion",
             "display_name": "Transcript Fusion",
             "so_id": "SO:0001886",
             "description": "A feature fusion where the deletion brings together transcript regions.",
             "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001886"
           },
           {
             "id": 47,
             "name": "missense_variant",
             "display_name": "Missense Variant",
             "so_id": "SO:0001583",
             "description": "A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.",
             "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001583"
           }
         ],
         "evidence_items": {
           "accepted_count": 1,
           "rejected_count": 0,
           "submitted_count": 0
         },
         "coordinates": {
           "chromosome": "9",
           "start": "133738363",
           "stop": "133738363",
           "reference_bases": "G",
           "variant_bases": "A",
           "representative_transcript": "ENST00000318560.5",
           "chromosome2": null,
           "start2": null,
           "stop2": null,
           "representative_transcript2": null,
           "ensembl_version": 75,
           "reference_build": "GRCh37"
         },
         "variant_groups": [
           {
             "id": 1,
             "name": "Imatinib Resistance",
             "description": "While imatinib has shown to be incredibly successful in treating philadelphia chromosome positive CML, patients that have shown primary or secondary resistance to the drug have been observed to harbor T315I and E255K ABL kinase domain mutations. These mutations, among others, have been observed both in primary refractory disease and acquired resistance. In gastrointestinal stromal tumors (GIST), PDGFRA 842 mutations have also been shown to confer resistance to imatinib. ",
             "variants": [
               {
                 "id": 2,
                 "entrez_name": "ABL1",
                 "gene_id": 4,
                 "entrez_id": 25,
                 "name": "BCR-ABL T334I",
                 "description": "While the efficacy of imatinib has revolutionized chronic myelogenous leukemia (CML) treatment, it is still not a cure-all. Both initial resistance and acquired resistance as a result of selection have been seen in a small subset of CML patients. The ABL kinase domain mutation T315I (aka T334I) has been shown to be one such mutation that confers resistance to imatinib. Second generation TKI's (dasatinib and ponatinib) specific to BCR-ABL have shown efficacy in treating resistant cases.",
                 "type": "variant",
                 "variant_types": [
                   {
                     "id": 47,
                     "name": "missense_variant",
                     "display_name": "Missense Variant",
                     "so_id": "SO:0001583",
                     "description": "A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.",
                     "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001583"
                   },
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
                   "chromosome": "9",
                   "start": "133748283",
                   "stop": "133748283",
                   "reference_bases": "C",
                   "variant_bases": "T",
                   "representative_transcript": "ENST00000372348.2",
                   "chromosome2": null,
                   "start2": null,
                   "stop2": null,
                   "representative_transcript2": null,
                   "ensembl_version": 75,
                   "reference_build": "GRCh37"
                 }
               },
               {
                 "id": 3,
                 "entrez_name": "ABL1",
                 "gene_id": 4,
                 "entrez_id": 25,
                 "name": "BCR-ABL E255K",
                 "description": "While the efficacy of imatinib has revolutionized chronic myelogenous leukemia (CML) treatment, it is still not a cure-all. Both initial resistance and acquired resistance as a result of selection have been seen in a small subset of CML patients. The ABL kinase domain mutation E255K has been shown to be one such mutation that confers resistance to imatinib. Second generation TKI's (dasatinib and nilotinib) specific to BCR-ABL have shown efficacy in treating resistant cases.",
                 "type": "variant",
                 "variant_types": [
                   {
                     "id": 47,
                     "name": "missense_variant",
                     "display_name": "Missense Variant",
                     "so_id": "SO:0001583",
                     "description": "A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.",
                     "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001583"
                   },
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
                   "chromosome": "9",
                   "start": "133738363",
                   "stop": "133738363",
                   "reference_bases": "G",
                   "variant_bases": "A",
                   "representative_transcript": "ENST00000318560.5",
                   "chromosome2": null,
                   "start2": null,
                   "stop2": null,
                   "representative_transcript2": null,
                   "ensembl_version": 75,
                   "reference_build": "GRCh37"
                 }
               },
               {
                 "id": 98,
                 "entrez_name": "PDGFRA",
                 "gene_id": 38,
                 "entrez_id": 5156,
                 "name": "D842I",
                 "description": "PDGFRA D842 mutations are characterized broadly as imatinib resistance mutations. This is most well characterized in gastrointestinal stromal tumors, but other cell lines containing these mutations have been shown to be resistant as well. In imatinib resistant cell lines, a number of other therapeutics have demonstrated efficacy. These include; crenolanib, sirolimus, and midostaurin (PKC412).",
                 "type": "variant",
                 "variant_types": [
                   {
                     "id": 47,
                     "name": "missense_variant",
                     "display_name": "Missense Variant",
                     "so_id": "SO:0001583",
                     "description": "A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.",
                     "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001583"
                   }
                 ],
                 "evidence_items": {
                   "accepted_count": 1,
                   "rejected_count": 0,
                   "submitted_count": 0
                 },
                 "coordinates": {
                   "chromosome": "4",
                   "start": "55152092",
                   "stop": "55152093",
                   "reference_bases": "GA",
                   "variant_bases": "AT",
                   "representative_transcript": "ENST00000257290.5",
                   "chromosome2": null,
                   "start2": null,
                   "stop2": null,
                   "representative_transcript2": null,
                   "ensembl_version": 75,
                   "reference_build": "GRCh37"
                 }
               },
               {
                 "id": 99,
                 "entrez_name": "PDGFRA",
                 "gene_id": 38,
                 "entrez_id": 5156,
                 "name": "D842V",
                 "description": "PDGFRA D842 mutations are characterized broadly as imatinib resistance mutations. This is most well characterized in gastrointestinal stromal tumors, but other cell lines containing these mutations have been shown to be resistant as well. Exogenous expression of the A842V mutation resulted in constitutive tyrosine phosphorylation of PDGFRA in the absence of ligand in 293T cells and cytokine-independent proliferation of the IL-3-dependent Ba/F3 cell line, both evidence that this is an activating mutation. In imatinib resistant cell lines, a number of other therapeutics have demonstrated efficacy. These include; crenolanib, sirolimus, and midostaurin (PKC412).",
                 "type": "variant",
                 "variant_types": [
                   {
                     "id": 47,
                     "name": "missense_variant",
                     "display_name": "Missense Variant",
                     "so_id": "SO:0001583",
                     "description": "A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.",
                     "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001583"
                   }
                 ],
                 "evidence_items": {
                   "accepted_count": 6,
                   "rejected_count": 0,
                   "submitted_count": 0
                 },
                 "coordinates": {
                   "chromosome": "4",
                   "start": "55152093",
                   "stop": "55152093",
                   "reference_bases": "A",
                   "variant_bases": "T",
                   "representative_transcript": "ENST00000257290.5",
                   "chromosome2": null,
                   "start2": null,
                   "stop2": null,
                   "representative_transcript2": null,
                   "ensembl_version": 75,
                   "reference_build": "GRCh37"
                 }
               },
               {
                 "id": 100,
                 "entrez_name": "PDGFRA",
                 "gene_id": 38,
                 "entrez_id": 5156,
                 "name": "D842Y",
                 "description": "PDGFRA D842 mutations are characterized broadly as imatinib resistance mutations. This is most well characterized in gastrointestinal stromal tumors, but other cell lines containing these mutations have been shown to be resistant as well. In imatinib resistant cell lines, a number of other therapeutics have demonstrated efficacy. These include; crenolanib, sirolimus, and midostaurin (PKC412).",
                 "type": "variant",
                 "variant_types": [
                   {
                     "id": 47,
                     "name": "missense_variant",
                     "display_name": "Missense Variant",
                     "so_id": "SO:0001583",
                     "description": "A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.",
                     "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001583"
                   }
                 ],
                 "evidence_items": {
                   "accepted_count": 1,
                   "rejected_count": 0,
                   "submitted_count": 0
                 },
                 "coordinates": {
                   "chromosome": "4",
                   "start": "55152092",
                   "stop": "55152092",
                   "reference_bases": "G",
                   "variant_bases": "T",
                   "representative_transcript": "ENST00000257290.5",
                   "chromosome2": null,
                   "start2": null,
                   "stop2": null,
                   "representative_transcript2": null,
                   "ensembl_version": 75,
                   "reference_build": "GRCh37"
                 }
               },
               {
                 "id": 101,
                 "entrez_name": "PDGFRA",
                 "gene_id": 38,
                 "entrez_id": 5156,
                 "name": "I843DEL",
                 "description": "PDGFRA D842 mutations are characterized broadly as imatinib resistance mutations. This is most well characterized in gastrointestinal stromal tumors, but other cell lines containing these mutations have been shown to be resistant as well. In imatinib resistant cell lines, a number of other therapeutics have demonstrated efficacy. These include; crenolanib, sirolimus, and midostaurin (PKC412).",
                 "type": "variant",
                 "variant_types": [
                   {
                     "id": 107,
                     "name": "inframe_deletion",
                     "display_name": "Inframe Deletion",
                     "so_id": "SO:0001822",
                     "description": "An inframe non synonymous variant that deletes bases from the coding sequence.",
                     "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001822"
                   }
                 ],
                 "evidence_items": {
                   "accepted_count": 2,
                   "rejected_count": 0,
                   "submitted_count": 0
                 },
                 "coordinates": {
                   "chromosome": "4",
                   "start": "55152095",
                   "stop": "55152097",
                   "reference_bases": "ATC",
                   "variant_bases": null,
                   "representative_transcript": "ENST00000257290.5",
                   "chromosome2": null,
                   "start2": null,
                   "stop2": null,
                   "representative_transcript2": null,
                   "ensembl_version": 75,
                   "reference_build": "GRCh37"
                 }
               },
               {
                 "id": 102,
                 "entrez_name": "PDGFRA",
                 "gene_id": 38,
                 "entrez_id": 5156,
                 "name": "DI842-843VM",
                 "description": "PDGFRA D842 mutations are characterized broadly as imatinib resistance mutations. The DI842-843VM variant is the result of a double point mutation. This is most well characterized in gastrointestinal stromal tumors, but other cell lines containing these mutations have been shown to be resistant as well. In imatinib resistant cell lines, a number of other therapeutics have demonstrated efficacy. These include; crenolanib, sirolimus, and midostaurin (PKC412).",
                 "type": "variant",
                 "variant_types": [
                   {
                     "id": 47,
                     "name": "missense_variant",
                     "display_name": "Missense Variant",
                     "so_id": "SO:0001583",
                     "description": "A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.",
                     "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001583"
                   }
                 ],
                 "evidence_items": {
                   "accepted_count": 1,
                   "rejected_count": 0,
                   "submitted_count": 0
                 },
                 "coordinates": {
                   "chromosome": "4",
                   "start": "55152093",
                   "stop": "55152097",
                   "reference_bases": "ACATC",
                   "variant_bases": "TCATG",
                   "representative_transcript": "ENST00000257290.5",
                   "chromosome2": null,
                   "start2": null,
                   "stop2": null,
                   "representative_transcript2": null,
                   "ensembl_version": 75,
                   "reference_build": "GRCh37"
                 }
               },
               {
                 "id": 241,
                 "entrez_name": "ABL1",
                 "gene_id": 4,
                 "entrez_id": 25,
                 "name": "BCR-ABL F317L",
                 "description": "BCR-ABL F317L, like the similar BCR-ABL T315I mutation, is becoming a common clinical marker for resistance to front-line therapies in CML. It has been shown to confer resistance to dasatinib, but responds well to ponatinib and other second generation inhibitors.",
                 "type": "variant",
                 "variant_types": [
                   {
                     "id": 47,
                     "name": "missense_variant",
                     "display_name": "Missense Variant",
                     "so_id": "SO:0001583",
                     "description": "A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.",
                     "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001583"
                   },
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
                   "chromosome": "9",
                   "start": "133748288",
                   "stop": "133748288",
                   "reference_bases": "T",
                   "variant_bases": "C",
                   "representative_transcript": "ENST00000318560.5",
                   "chromosome2": null,
                   "start2": null,
                   "stop2": null,
                   "representative_transcript2": null,
                   "ensembl_version": 75,
                   "reference_build": "GRCh37"
                 }
               }
             ],
             "type": "variant_group"
           }
         ]
       }
     ],
     "type": "variant_group",
     "lifecycle_actions": {
       "created": {
         "order": 1,
         "timestamp": "2015-06-21T16:49:38.943Z",
         "user": {
           "id": 41,
           "email": "nspies13@gmail.com",
           "name": "Nick Spies",
           "last_seen_at": "2016-12-02T22:15:09.110Z",
           "username": "NickSpies",
           "role": "admin",
           "avatar_url": "https://secure.gravatar.com/avatar/3376aeb8439c5ab3e5d72fa2eeed39e5.png?d=identicon&r=pg&s=32",
           "avatars": {
             "x128": "https://secure.gravatar.com/avatar/3376aeb8439c5ab3e5d72fa2eeed39e5.png?d=identicon&r=pg&s=128",
             "x64": "https://secure.gravatar.com/avatar/3376aeb8439c5ab3e5d72fa2eeed39e5.png?d=identicon&r=pg&s=64",
             "x32": "https://secure.gravatar.com/avatar/3376aeb8439c5ab3e5d72fa2eeed39e5.png?d=identicon&r=pg&s=32",
             "x14": "https://secure.gravatar.com/avatar/3376aeb8439c5ab3e5d72fa2eeed39e5.png?d=identicon&r=pg&s=14"
           },
           "area_of_expertise": "Research Scientist",
           "orcid": "",
           "display_name": "NickSpies",
           "created_at": "2015-06-12T18:13:16.508Z",
           "url": "",
           "twitter_handle": "@NickSpies13",
           "facebook_profile": null,
           "linkedin_profile": null,
           "bio": "Nick Spies is a staff analyst at the McDonnell Genome Institute and an MD student at Washington University School of Medicine. He has made substantial contributions to the development of genome analysis tools and resources at the Genome Institute including the Drug-Gene Interaction Database. He is a founding member of the CIViC team, helping to define the CIViC data model, and a leading content curator and a feature development consultant.",
           "featured_expert": true,
           "accepted_license": null,
           "signup_complete": null
         }
       }
     },
     "sources": []
   }
