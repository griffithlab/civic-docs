Variants
========

The variants endpoint allows users to enumerate all of the variants present in CIViC as well as retrieve more detailed information on a specific variant. A common use case would be to get a list of variants for a gene using the genes endpoint and then fetching detailed information for each variant via the variants endpoint.

Get a list of variants
----------------------

This endpoint returns a listing of variants in CIViC that contain at least one evidence item. This index style endpoint is `paginated` by default. You can use the ``count`` and ``page`` parameters or the ``previous`` and ``next`` links to iterate through all the variants.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/variants

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
     - How many variants to return on a single page

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/variants

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   {
     "_meta": {
       "current_page": 1,
       "per_page": 25,
       "total_pages": 30,
       "total_count": 729,
       "links": {
         "next": "https://civicdb.org/api/variants?count=25&page=2",
         "previous": null
       }
     },
     "records": [
       {
         "id": 1,
         "entrez_name": "ABL1",
         "gene_id": 4,
         "entrez_id": 25,
         "name": "BCR-ABL",
         "description": "The BCR-ABL fusion protein, commonly referred to as the Philadelphia chromosome, is one of the most studied fusion genes in cancer. It has widely been considered the initiating event in chronic myelogenous leukemia (CML). However, despite its ability to initiate disease in mice, its status as an initiating mutation is in dispute. In what is commonly used as the poster-child for targeted therapeutics, the development and use of imatinib in the clinic has led to profound improvements in the prognosis of the disease. However, imatinib resistance is still seen in patients with mutations in the ABL kinase domain of the fusion, most notably the T315I variant. In patients resistant to imatinib, either acquired or otherwise, second generation BCR-ABL TKI's (dasatinib and ponatinib) have seen some success in delivering a tumor response.",
         "type": "variant",
         "variant_types": [
         ],
         "evidence_items": {
           "accepted_count": 7,
           "rejected_count": 0,
           "submitted_count": 0
         },
         "coordinates": {
           "chromosome": "22",
           "start": "23522397",
           "stop": "23632600",
           "reference_bases": null,
           "variant_bases": null,
           "representative_transcript": "ENST00000305877.8",
           "chromosome2": "9",
           "start2": "133729451",
           "stop2": "133763063",
           "representative_transcript2": "ENST00000318560.5",
           "ensembl_version": 75,
           "reference_build": "GRCh37"
         }
       },
       {
         "id": 28,
         "entrez_name": "CEBPA",
         "gene_id": 15,
         "entrez_id": 1050,
         "name": "N-TERMINAL FRAME SHIFT",
         "description": "CEBPA N-terminal frame shift mutations that result in a premature stop codon are associated with cytogenetically normal acute myeloid leukemia (CN-AML). CEBPA mutations are associated with a favorable prognosis; however, NPM1 and FLT3 mutations should also be assessed in CN-AML patients as concurrent mutations may have prognostic implications. N-terminal frame shift mutations within amino acids 1-120 have been shown to disrupt expression of the full-length 42kDa isoform while maintaining expression of a 30kDa isoform (translated from the AUG at full-length protein isoform amino acid M120). This 30kDa isoform exhibits dominant negative activity.",
         "type": "variant",
         "variant_types": [
           {
             "id": 134,
             "name": "frameshift_truncation",
             "display_name": "Frameshift Truncation",
             "so_id": "SO:0001910",
             "description": "A frameshift variant that causes the translational reading frame to be shortened relative to the reference feature.",
             "url": "http://www.sequenceontology.org/browser/current_svn/term/SO:0001910"
           },
         ],
         "evidence_items": {
           "accepted_count": 2,
           "rejected_count": 0,
           "submitted_count": 0
         },
         "coordinates": {
           "chromosome": "19",
           "start": "33792961",
           "stop": "33793470",
           "reference_bases": null,
           "variant_bases": null,
           "representative_transcript": "ENST00000498907.2",
           "chromosome2": null,
           "start2": null,
           "stop2": null,
           "representative_transcript2": null,
           "ensembl_version": 75,
           "reference_build": "GRCh37"
         }
       }
     ]
   }

Get details for a specific variant
----------------------------------

This endpoint retrieves details about a specific variant, given its internal CIViC id.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/variants/:id

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/variants/8

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   {
     "id": 8,
     "entrez_name": "ALK",
     "gene_id": 1,
     "entrez_id": 238,
     "name": "F1174L",
     "description": "ALK F1174L has been observed as recurrent in neuroblastoma, non-small cell lung cancer (NSCLC), and other cancer types. Neuroblastoma cells containing this mutation have shown resistance to low doses of criztonib. However, increased dosage can overcome this resistance in cell lines studies. TAE684 has also proven effective in both NSCLC and neuroblastoma F1174L containing cells.",
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
     "evidence_items": [
       {
         "id": 1271,
         "name": "EID1271",
         "description": "In a Phase I trial (NCT00939770) of the drug crizotinib in pediatric patients, a subset of 11 neuroblastoma patients were characterized for mutations in ALK. Of these 11 patients, 4 had the F1174L mutation. Among these 4 patients, stable disease (SD) was observed in one, and progressive disease (PD) was observed in 3 others after administration of crizotinib. In contrast, in the remaining 7 patients with mutations different than F1174L, 4 had PD, 2 had SD and one had complete response as best response after initiation of crizotinib.",
         "disease": {
           "id": 13,
           "name": "Neuroblastoma",
           "display_name": "Neuroblastoma",
           "doid": "769",
           "url": "http://www.disease-ontology.org/?id=DOID:769"
         },
         "drugs": [
           {
             "id": 12,
             "name": "Crizotinib",
             "pubchem_id": null
           }
         ],
         "rating": 3,
         "evidence_level": "B",
         "evidence_type": "Predictive",
         "clinical_significance": "Sensitivity",
         "evidence_direction": "Does Not Support",
         "variant_origin": "Somatic Mutation",
         "drug_interaction_type": null,
         "status": "accepted",
         "open_change_count": 0,
         "type": "evidence",
         "source": {
           "id": 859,
           "name": "Safety and activity of crizotinib for paediatric patients with refractory solid tumours or anaplastic large-cell lymphoma: a Children's Oncology Group phase 1 consortium study.",
           "citation": "Mossé et al., 2013, Lancet Oncol.",
           "pubmed_id": "23598171",
           "source_url": "http://www.ncbi.nlm.nih.gov/pubmed/23598171",
           "open_access": true,
           "pmc_id": "PMC3730818",
           "publication_date": {
             "year": 2013,
             "month": 5
           },
           "journal": "Lancet Oncol.",
           "full_journal_title": "The Lancet. Oncology",
           "status": "fully curated"
         },
         "variant_id": 8
       },
     ],
     "coordinates": {
       "chromosome": "2",
       "start": "29443695",
       "stop": "29443695",
       "reference_bases": "G",
       "variant_bases": "T",
       "representative_transcript": "ENST00000389048.3",
       "chromosome2": null,
       "start2": null,
       "stop2": null,
       "representative_transcript2": null,
       "ensembl_version": 75,
       "reference_build": "GRCh37"
     },
     "variant_groups": [
       {
         "id": 3,
         "name": "Crizotinib Resistance",
         "description": "The ALK oncogene has long been considered a driving factor in non-small cell lung cancer (NSCLC). The targeted tyrosine kinase inhibitor criztonib has shown to be effective in ALK-mutant NSCLC. However, in patients that have shown acquired resistance to crizotinib, missense mutations in the tyrosine kinase domain have shown to drive this resistance. ",
         "variants": [
           {
             "id": 6,
             "entrez_name": "ALK",
             "gene_id": 1,
             "entrez_id": 238,
             "name": "EML4-ALK C1156Y",
             "description": "In patients with non-small cell lung cancer exhibiting EML4-ALK fusion, C1156Y has been shown to confer resistance to crizotinib. Case reports indicate that secondary mutations can modulate drug sensitivity. EML4-ALK C1156Y/L1196M maintained crizotinib resistance while the lorlatinib resistant combination EML4-ALK C1156Y/L1198F re-sensitized the tumor to crizotinib treatment.",
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
               "chromosome": "2",
               "start": "29445258",
               "stop": "29445258",
               "reference_bases": "C",
               "variant_bases": "T",
               "representative_transcript": "ENST00000389048.3",
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
       }
     ],
     "variant_aliases": [],
     "hgvs_expressions": [],
     "clinvar_entries": [],
     "lifecycle_actions": {
       "last_reviewed": {
         "order": 1,
         "timestamp": "2016-05-03T15:11:18.404Z",
         "user": {
           "id": 6,
           "email": "kkrysiak@genome.wustl.edu",
           "name": "Kilannin Krysiak",
           "last_seen_at": "2017-01-04T16:05:02.406Z",
           "username": "kkrysiak",
           "role": "admin",
           "avatar_url": "https://secure.gravatar.com/avatar/17180f9afc9f7f04fff97197c1ee5cb6.png?d=identicon&r=pg&s=32",
           "avatars": {
             "x128": "https://secure.gravatar.com/avatar/17180f9afc9f7f04fff97197c1ee5cb6.png?d=identicon&r=pg&s=128",
             "x64": "https://secure.gravatar.com/avatar/17180f9afc9f7f04fff97197c1ee5cb6.png?d=identicon&r=pg&s=64",
             "x32": "https://secure.gravatar.com/avatar/17180f9afc9f7f04fff97197c1ee5cb6.png?d=identicon&r=pg&s=32",
             "x14": "https://secure.gravatar.com/avatar/17180f9afc9f7f04fff97197c1ee5cb6.png?d=identicon&r=pg&s=14"
           },
           "area_of_expertise": "Research Scientist",
           "orcid": "0000-0002-6299-9230",
           "display_name": "kkrysiak",
           "created_at": "2015-02-26T04:14:20.953Z",
           "url": "",
           "twitter_handle": "",
           "facebook_profile": "",
           "linkedin_profile": "kilannin-krysiak-69047819",
           "bio": "Dr. Krysiak is a staff scientist at the McDonnell Genome Institute at Washington University School of Medicine where she is involved in the comprehensive genomic analysis of cancer patient cohorts and “n-of-1” studies. She received her PhD in Molecular Genetics and Genomics at Washington University in St. Louis where she focused on the genetics of myelodysplastic syndrome through advanced flow cytometry techniques, primary cell culture and mouse models. She is a founding member of the CIViC team, helping to define the CIViC knowledge model, and a leading content curator and feature development consultant.",
           "featured_expert": true,
           "accepted_license": null,
           "signup_complete": null
         }
       }
     },
     "sources": [],
     "errors": {}
   }
