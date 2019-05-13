Assertions
==========

The assertions endpoint allows users to enumerate all of the assertions present in CIViC as well as retrieve more detailed information on a specific assertion. This is the endpoint that should be used to obtain a complete listing of every assertion in CIViC.

Get a list of assertions
------------------------

This endpoint returns a listing of assertions in CIViC. This index style endpoint is `paginated` by default. You can use the ``count`` and ``page`` parameters or the ``previous`` and ``next`` links to iterate through all the assertions.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/assertions

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
     - How many assertions to return on a single page

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/assertions

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   {
       "_meta": {
           "current_page": 1,
           "per_page": 6,
           "total_pages": 1,
           "total_count": 6,
           "links": {
               "next": null,
               "previous": null
         }
       },
       "records": [
       {
           "id": 1,
           "type": "assertion",
           "name": "AID1",
           "summary": "HER2 amplification predicts sensitivity to Trastuzumab",
           "description": "HER2 amplification defines a clinically relevant subtype of breast cancer. HER2 amplification predicts sensitivity to various targeted therapies including the monoclonal antibody Trastuzumab. The use of Trastuzumab, often in combination with chemotherapy and/or endocrine therapy (depending on hormone receptor status), is now standard of care for HER2-positive breast cancer patients.",
           "gene": {
               "name": "ERBB2",
               "id": 20
           },
           "variant": {
               "name": "AMPLIFICATION",
               "id": 306
           },
           "disease": {
               "id": 368,
               "name": "Her2-receptor Positive Breast Cancer",
               "display_name": "Her2-receptor Positive Breast Cancer",
               "doid": "0060079",
               "url": "http://www.disease-ontology.org/?id=DOID:0060079"
           },
           "drugs": [
             {
               "id": 84,
               "name": "Trastuzumab",
               "pubchem_id": null
             }
           ],
           "evidence_type": "Predictive",
           "evidence_direction": "Supports",
           "clinical_significance": "Sensitivity",
           "evidence_item_count": 3,
           "fda_regulatory_approval": true,
           "status": "rejected",
           "open_change_count": 0,
           "pending_evidence_count": 0
       },
       {
           "id": 2,
           "type": "assertion",
           "name": "AID2",
           "summary": "HER2 amplification predicts sensitivity to Trastuzumab",
           "description": "HER2 amplification defines a clinically relevant subtype of breast cancer. HER2 amplification predicts sensitivity to various targeted therapies including the monoclonal antibody Trastuzumab. The use of Trastuzumab, often in combination with chemotherapy and/or endocrine therapy (depending on hormone receptor status), is now standard of care for HER2-positive breast cancer patients.",
           "gene": {
               "name": "ERBB2",
               "id": 20
           },
           "variant": {
               "name": "AMPLIFICATION",
               "id": 306
           },
           "disease": {
               "id": 368,
               "name": "Her2-receptor Positive Breast Cancer",
               "display_name": "Her2-receptor Positive Breast Cancer",
               "doid": "0060079",
               "url": "http://www.disease-ontology.org/?id=DOID:0060079"
           },
           "drugs": [
             {
               "id": 84,
               "name": "Trastuzumab",
               "pubchem_id": null
             }
           ],
           "evidence_type": "Predictive",
           "evidence_direction": "Supports",
           "clinical_significance": "Sensitivity",
           "evidence_item_count": 3,
           "fda_regulatory_approval": true,
           "status": "accepted",
           "open_change_count": 0,
           "pending_evidence_count": 0
       }
     ]
   }

Get details for a specific assertion
------------------------------------

This endpoint retrieves details about a specific assertion, given its internal CIViC id.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/assertions/:id

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/assertions/2

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   {
       "id": 2,
       "type": "assertion",
       "name": "AID2",
       "summary": "HER2 amplification predicts sensitivity to Trastuzumab",
       "description": "HER2 amplification defines a clinically relevant subtype of breast cancer. HER2 amplification predicts sensitivity to various targeted therapies including the monoclonal antibody Trastuzumab. The use of Trastuzumab, often in combination with chemotherapy and/or endocrine therapy (depending on hormone receptor status), is now standard of care for HER2-positive breast cancer patients.",
       "gene": {
           "name": "ERBB2",
           "id": 20
       },
       "variant": {
           "name": "AMPLIFICATION",
           "id": 306
       },
       "disease": {
           "id": 368,
           "name": "Her2-receptor Positive Breast Cancer",
           "display_name": "Her2-receptor Positive Breast Cancer",
           "doid": "0060079",
           "url": "http://www.disease-ontology.org/?id=DOID:0060079"
       },
       "drugs": [
       {
           "id": 84,
           "name": "Trastuzumab",
           "pubchem_id": null
       }
       ],
       "evidence_type": "Predictive",
       "evidence_direction": "Supports",
       "clinical_significance": "Sensitivity",
       "evidence_item_count": 3,
       "fda_regulatory_approval": true,
       "status": "accepted",
       "open_change_count": 0,
       "pending_evidence_count": 0,
       "nccn_guideline": "Breast Cancer",
       "nccn_guideline_version": "3.2017",
       "amp_level": "Tier I - Level A",
       "evidence_items": [
       {
           "id": 528,
           "name": "EID528",
           "description": "A randomized clinical trial of 469 patients with previously untreated, HER2-positive, metastatic breast cancer demonstrated improved time to disease progression, objective response rate, and duration of response for patients who received trastuzumab in addition to chemotherapy compared to chemotherapy alone.",
           "disease": {
               "id": 368,
               "name": "Her2-receptor Positive Breast Cancer",
               "display_name": "Her2-receptor Positive Breast Cancer",
               "doid": "0060079",
               "url": "http://www.disease-ontology.org/?id=DOID:0060079"
           },
           "drugs": [
           {
               "id": 84,
               "name": "Trastuzumab",
               "pubchem_id": null
           }
           ],
           "rating": 5,
           "evidence_level": "B",
           "evidence_type": "Predictive",
           "clinical_significance": "Sensitivity",
           "evidence_direction": "Supports",
           "variant_origin": "Somatic Mutation",
           "drug_interaction_type": null,
           "status": "accepted",
           "open_change_count": 0,
           "type": "evidence",
           "source": {
               "id": 328,
               "name": "Use of chemotherapy plus a monoclonal antibody against HER2 for metastatic breast cancer that overexpresses HER2.",
               "citation": "Slamon et al., 2001, N. Engl. J. Med.",
               "pubmed_id": "11248153",
               "source_url": "http://www.ncbi.nlm.nih.gov/pubmed/11248153",
               "open_access": null,
               "pmc_id": null,
               "publication_date": {
                   "year": 2001,
                   "month": 3,
                   "day": 15
               },
               "journal": "N. Engl. J. Med.",
               "full_journal_title": "The New England journal of medicine",
               "status": "fully curated",
               "is_review": false,
               "clinical_trials": []
           },
           "variant_id": 306,
           "phenotypes": [],
           "errors": {},
           "lifecycle_actions": {
               "submitted": {
                   "timestamp": "2015-08-25T15:42:25.527Z",
                   "user": {
                       "id": 3,
                       "name": "Obi Griffith",
                       "last_seen_at": "2018-02-28T17:11:03.923Z",
                       "username": "obigriffith",
                       "role": "admin",
                       "avatar_url": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Research Scientist",
                       "orcid": "0000-0002-0843-4271",
                       "display_name": "obigriffith",
                       "created_at": "2015-02-26T02:53:49.147Z",
                       "url": "http://genome.wustl.edu/people/individual/obi-griffith/",
                       "twitter_handle": "obigriffith",
                       "facebook_profile": "",
                       "linkedin_profile": "obigriffith",
                       "bio": "Dr. Griffith is Assistant Professor of Medicine and Assistant Director of the McDonnell Genome Institute at Washington University School of Medicine. He has worked in genomics and bioinformatics since the earliest phase of reference genome sequencing. He contributed to the Mammalian Gene Collection, producing some of the first full-length sequences for many human genes. He also was part of a small team of bioinformaticians that helped sequence and release the first whole genome reference sequence for the severe acute respiratory syndrome (SARS) virus at the height of the 2003 epidemic. He has contributed to the identification of molecular markers at the DNA, RNA and protein level that are useful for diagnosis and prognosis of thyroid, breast, lymphoma and other cancers. His lab’s research is focused on the development of informatics resources and personalized medicine strategies for cancer using genomic technologies. He is a co-creator of the CIViC resource.",
                       "featured_expert": true,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": "",
                       "organization": {
                           "id": 1,
                           "name": "The McDonnell Genome Institute",
                           "url": "http://genome.wustl.edu/",
                           "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                           "profile_image": {
                               "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                           }
                       }
                   }
               },
               "last_modified": {
                   "timestamp": "2017-11-01T11:41:27.713Z",
                   "user": {
                       "id": 418,
                       "name": "Paul Roepman",
                       "last_seen_at": "2018-02-14T11:56:51.985Z",
                       "username": "PaulRoepman",
                       "role": "curator",
                       "avatar_url": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Clinical Scientist",
                       "orcid": "0000-0003-1566-0258",
                       "display_name": "PaulRoepman",
                       "created_at": "2017-04-04T11:32:56.753Z",
                       "url": null,
                       "twitter_handle": null,
                       "facebook_profile": null,
                       "linkedin_profile": "proepman",
                       "bio": "",
                       "featured_expert": false,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": null,
                       "organization": {}
                   }
               },
               "last_reviewed": {
                   "timestamp": "2018-01-11T18:47:57.238Z",
                   "user": {
                       "id": 3,
                       "name": "Obi Griffith",
                       "last_seen_at": "2018-02-28T17:11:03.923Z",
                       "username": "obigriffith",
                       "role": "admin",
                       "avatar_url": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Research Scientist",
                       "orcid": "0000-0002-0843-4271",
                       "display_name": "obigriffith",
                       "created_at": "2015-02-26T02:53:49.147Z",
                       "url": "http://genome.wustl.edu/people/individual/obi-griffith/",
                       "twitter_handle": "obigriffith",
                       "facebook_profile": "",
                       "linkedin_profile": "obigriffith",
                       "bio": "Dr. Griffith is Assistant Professor of Medicine and Assistant Director of the McDonnell Genome Institute at Washington University School of Medicine. He has worked in genomics and bioinformatics since the earliest phase of reference genome sequencing. He contributed to the Mammalian Gene Collection, producing some of the first full-length sequences for many human genes. He also was part of a small team of bioinformaticians that helped sequence and release the first whole genome reference sequence for the severe acute respiratory syndrome (SARS) virus at the height of the 2003 epidemic. He has contributed to the identification of molecular markers at the DNA, RNA and protein level that are useful for diagnosis and prognosis of thyroid, breast, lymphoma and other cancers. His lab’s research is focused on the development of informatics resources and personalized medicine strategies for cancer using genomic technologies. He is a co-creator of the CIViC resource.",
                       "featured_expert": true,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": "",
                       "organization": {
                           "id": 1,
                           "name": "The McDonnell Genome Institute",
                           "url": "http://genome.wustl.edu/",
                           "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                           "profile_image": {
                               "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                           }
                       }
                   }
               },
               "last_commented_on": {
                   "timestamp": "2017-11-01T10:55:28.039Z",
                   "user": {
                       "id": 418,
                       "name": "Paul Roepman",
                       "last_seen_at": "2018-02-14T11:56:51.985Z",
                       "username": "PaulRoepman",
                       "role": "curator",
                       "avatar_url": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Clinical Scientist",
                       "orcid": "0000-0003-1566-0258",
                       "display_name": "PaulRoepman",
                       "created_at": "2017-04-04T11:32:56.753Z",
                       "url": null,
                       "twitter_handle": null,
                       "facebook_profile": null,
                       "linkedin_profile": "proepman",
                       "bio": "",
                       "featured_expert": false,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": null,
                       "organization": {}
                   }
               },
               "accepted": {
                   "timestamp": "2015-08-25T15:42:25.527Z",
                   "user": {
                       "id": 41,
                       "name": "Nick Spies",
                       "last_seen_at": "2018-02-13T20:09:25.261Z",
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
                       "facebook_profile": "",
                       "linkedin_profile": "",
                       "bio": "Nick Spies is a staff analyst at the McDonnell Genome Institute and an MD student at Washington University School of Medicine. He has made substantial contributions to the development of genome analysis tools and resources at the Genome Institute including the Drug-Gene Interaction Database. He is a founding member of the CIViC team, helping to define the CIViC data model, and a leading content curator and a feature development consultant.",
                       "featured_expert": true,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": "",
                       "organization": {
                           "id": 1,
                           "name": "The McDonnell Genome Institute",
                           "url": "http://genome.wustl.edu/",
                           "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                           "profile_image": {
                               "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                           }
                       }
                   }
               }
           },
           "fields_with_pending_changes": {},
           "gene_id": 20,
           "state_params": {
               "evidence_item": {
                   "id": 528,
                   "name": "EID528"
               },
               "variant": {
                   "id": 306,
                   "name": "AMPLIFICATION"
               },
               "gene": {
                   "id": 20,
                   "name": "ERBB2"
               }
           }
       },
       {
           "id": 529,
           "name": "EID529",
           "description": "A randomized clinical trial of 186 patients with previously untreated, HER2-positive, metastatic breast cancer demonstrated improved overall survival, response rate, response duration, time to progression, and time to treatment failure for patients who received trastuzumab in addition to chemotherapy (docetaxel) compared to chemotherapy alone.",
           "disease": {
               "id": 368,
               "name": "Her2-receptor Positive Breast Cancer",
               "display_name": "Her2-receptor Positive Breast Cancer",
               "doid": "0060079",
               "url": "http://www.disease-ontology.org/?id=DOID:0060079"
           },
           "drugs": [
           {
               "id": 84,
               "name": "Trastuzumab",
               "pubchem_id": null
           }
           ],
           "rating": 5,
           "evidence_level": "B",
           "evidence_type": "Predictive",
           "clinical_significance": "Sensitivity",
           "evidence_direction": "Supports",
           "variant_origin": "Somatic Mutation",
           "drug_interaction_type": null,
           "status": "accepted",
           "open_change_count": 0,
           "type": "evidence",
           "source": {
               "id": 329,
               "name": "Randomized phase II trial of the efficacy and safety of trastuzumab combined with docetaxel in patients with human epidermal growth factor receptor 2-positive metastatic breast cancer administered as first-line treatment: the M77001 study group.",
               "citation": "Marty et al., 2005, J. Clin. Oncol.",
               "pubmed_id": "15911866",
               "source_url": "http://www.ncbi.nlm.nih.gov/pubmed/15911866",
               "open_access": null,
               "pmc_id": null,
               "publication_date": {
                   "year": 2005,
                   "month": 7,
                   "day": 1
               },
               "journal": "J. Clin. Oncol.",
               "full_journal_title": "Journal of clinical oncology : official journal of the American Society of Clinical Oncology",
               "status": "fully curated",
               "is_review": false,
               "clinical_trials": []
           },
           "variant_id": 306,
           "phenotypes": [],
           "errors": {},
           "lifecycle_actions": {
               "submitted": {
                   "timestamp": "2015-08-25T16:20:01.514Z",
                   "user": {
                       "id": 3,
                       "name": "Obi Griffith",
                       "last_seen_at": "2018-02-28T17:11:03.923Z",
                       "username": "obigriffith",
                       "role": "admin",
                       "avatar_url": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Research Scientist",
                       "orcid": "0000-0002-0843-4271",
                       "display_name": "obigriffith",
                       "created_at": "2015-02-26T02:53:49.147Z",
                       "url": "http://genome.wustl.edu/people/individual/obi-griffith/",
                       "twitter_handle": "obigriffith",
                       "facebook_profile": "",
                       "linkedin_profile": "obigriffith",
                       "bio": "Dr. Griffith is Assistant Professor of Medicine and Assistant Director of the McDonnell Genome Institute at Washington University School of Medicine. He has worked in genomics and bioinformatics since the earliest phase of reference genome sequencing. He contributed to the Mammalian Gene Collection, producing some of the first full-length sequences for many human genes. He also was part of a small team of bioinformaticians that helped sequence and release the first whole genome reference sequence for the severe acute respiratory syndrome (SARS) virus at the height of the 2003 epidemic. He has contributed to the identification of molecular markers at the DNA, RNA and protein level that are useful for diagnosis and prognosis of thyroid, breast, lymphoma and other cancers. His lab’s research is focused on the development of informatics resources and personalized medicine strategies for cancer using genomic technologies. He is a co-creator of the CIViC resource.",
                       "featured_expert": true,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": "",
                       "organization": {
                           "id": 1,
                           "name": "The McDonnell Genome Institute",
                           "url": "http://genome.wustl.edu/",
                           "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                           "profile_image": {
                               "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                           }
                       }
                   }
               },
               "last_modified": {
                   "timestamp": "2017-11-01T11:42:05.451Z",
                   "user": {
                       "id": 418,
                       "name": "Paul Roepman",
                       "last_seen_at": "2018-02-14T11:56:51.985Z",
                       "username": "PaulRoepman",
                       "role": "curator",
                       "avatar_url": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Clinical Scientist",
                       "orcid": "0000-0003-1566-0258",
                       "display_name": "PaulRoepman",
                       "created_at": "2017-04-04T11:32:56.753Z",
                       "url": null,
                       "twitter_handle": null,
                       "facebook_profile": null,
                       "linkedin_profile": "proepman",
                       "bio": "",
                       "featured_expert": false,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": null,
                       "organization": {}
                   }
               },
               "last_reviewed": {
                   "timestamp": "2018-01-11T18:48:23.019Z",
                   "user": {
                       "id": 3,
                       "name": "Obi Griffith",
                       "last_seen_at": "2018-02-28T17:11:03.923Z",
                       "username": "obigriffith",
                       "role": "admin",
                       "avatar_url": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Research Scientist",
                       "orcid": "0000-0002-0843-4271",
                       "display_name": "obigriffith",
                       "created_at": "2015-02-26T02:53:49.147Z",
                       "url": "http://genome.wustl.edu/people/individual/obi-griffith/",
                       "twitter_handle": "obigriffith",
                       "facebook_profile": "",
                       "linkedin_profile": "obigriffith",
                       "bio": "Dr. Griffith is Assistant Professor of Medicine and Assistant Director of the McDonnell Genome Institute at Washington University School of Medicine. He has worked in genomics and bioinformatics since the earliest phase of reference genome sequencing. He contributed to the Mammalian Gene Collection, producing some of the first full-length sequences for many human genes. He also was part of a small team of bioinformaticians that helped sequence and release the first whole genome reference sequence for the severe acute respiratory syndrome (SARS) virus at the height of the 2003 epidemic. He has contributed to the identification of molecular markers at the DNA, RNA and protein level that are useful for diagnosis and prognosis of thyroid, breast, lymphoma and other cancers. His lab’s research is focused on the development of informatics resources and personalized medicine strategies for cancer using genomic technologies. He is a co-creator of the CIViC resource.",
                       "featured_expert": true,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": "",
                       "organization": {
                           "id": 1,
                           "name": "The McDonnell Genome Institute",
                           "url": "http://genome.wustl.edu/",
                           "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                           "profile_image": {
                               "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                           }
                       }
                   }
               },
               "last_commented_on": {
                   "timestamp": "2017-11-01T10:55:46.360Z",
                   "user": {
                       "id": 418,
                       "name": "Paul Roepman",
                       "last_seen_at": "2018-02-14T11:56:51.985Z",
                       "username": "PaulRoepman",
                       "role": "curator",
                       "avatar_url": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Clinical Scientist",
                       "orcid": "0000-0003-1566-0258",
                       "display_name": "PaulRoepman",
                       "created_at": "2017-04-04T11:32:56.753Z",
                       "url": null,
                       "twitter_handle": null,
                       "facebook_profile": null,
                       "linkedin_profile": "proepman",
                       "bio": "",
                       "featured_expert": false,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": null,
                       "organization": {}
                   }
               },
               "accepted": {
                   "timestamp": "2015-08-25T16:20:01.514Z",
                   "user": {
                       "id": 41,
                       "name": "Nick Spies",
                       "last_seen_at": "2018-02-13T20:09:25.261Z",
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
                       "facebook_profile": "",
                       "linkedin_profile": "",
                       "bio": "Nick Spies is a staff analyst at the McDonnell Genome Institute and an MD student at Washington University School of Medicine. He has made substantial contributions to the development of genome analysis tools and resources at the Genome Institute including the Drug-Gene Interaction Database. He is a founding member of the CIViC team, helping to define the CIViC data model, and a leading content curator and a feature development consultant.",
                       "featured_expert": true,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": "",
                       "organization": {
                           "id": 1,
                           "name": "The McDonnell Genome Institute",
                           "url": "http://genome.wustl.edu/",
                           "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                           "profile_image": {
                               "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                           }
                       }
                   }
               }
           },
           "fields_with_pending_changes": {},
           "gene_id": 20,
           "state_params": {
               "evidence_item": {
                   "id": 529,
                   "name": "EID529"
               },
               "variant": {
                   "id": 306,
                   "name": "AMPLIFICATION"
               },
               "gene": {
                   "id": 20,
                   "name": "ERBB2"
               }
           }
       },
       {
           "id": 1122,
           "name": "EID1122",
           "description": "HERA was a Phase III trial assessing application of trastuzumab in an extended adjuvant setting.  Patients were HER2 positive with completely excised invasive BC, node positive or negative, and having undergone prior adjuvant or neo-adjuvant chemotherapy.  In the 3 arm study patients were given trastuzumab courses of 1 year, 2 years, or untreated.  At the first planned interim analysis, trastuzumab treatment for one year was compared with observation alone.  A significant difference in disease-free survival was seen with 220 DFS events out of 1693 in the observation arm versus 127 DFS events out of 1694 in the 1 year trastuzumab arm.  1 year adjuvant trastuzumab is currently the standard of care.",
           "disease": {
               "id": 368,
               "name": "Her2-receptor Positive Breast Cancer",
               "display_name": "Her2-receptor Positive Breast Cancer",
               "doid": "0060079",
               "url": "http://www.disease-ontology.org/?id=DOID:0060079"
           },
           "drugs": [
           {
               "id": 84,
               "name": "Trastuzumab",
               "pubchem_id": null
           }
           ],
           "rating": 4,
           "evidence_level": "A",
           "evidence_type": "Predictive",
           "clinical_significance": "Sensitivity",
           "evidence_direction": "Supports",
           "variant_origin": "Somatic Mutation",
           "drug_interaction_type": null,
           "status": "accepted",
           "open_change_count": 0,
           "type": "evidence",
           "source": {
               "id": 777,
               "name": "Trastuzumab after adjuvant chemotherapy in HER2-positive breast cancer.",
               "citation": "Piccart-Gebhart et al., 2005, N. Engl. J. Med.",
               "pubmed_id": "16236737",
               "source_url": "http://www.ncbi.nlm.nih.gov/pubmed/16236737",
               "open_access": null,
               "pmc_id": null,
               "publication_date": {
                   "year": 2005,
                   "month": 10,
                   "day": 20
               },
               "journal": "N. Engl. J. Med.",
               "full_journal_title": "The New England journal of medicine",
               "status": "fully curated",
               "is_review": false,
               "clinical_trials": []
           },
           "variant_id": 306,
           "phenotypes": [],
           "errors": {},
           "lifecycle_actions": {
               "submitted": {
                   "timestamp": "2016-02-26T08:41:00.728Z",
                   "user": {
                       "id": 110,
                       "name": "Arpad Danos",
                       "last_seen_at": "2018-03-06T19:06:13.119Z",
                       "username": "arpaddanos",
                       "role": "admin",
                       "avatar_url": "https://secure.gravatar.com/avatar/45c2db32371a9f86e1f6190f57758d77.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/45c2db32371a9f86e1f6190f57758d77.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/45c2db32371a9f86e1f6190f57758d77.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/45c2db32371a9f86e1f6190f57758d77.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/45c2db32371a9f86e1f6190f57758d77.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Research Scientist",
                       "orcid": "",
                       "display_name": "arpaddanos",
                       "created_at": "2016-01-27T00:20:51.218Z",
                       "url": "",
                       "twitter_handle": "",
                       "facebook_profile": "",
                       "linkedin_profile": "",
                       "bio": "",
                       "featured_expert": false,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": "",
                       "organization": {
                           "id": 1,
                           "name": "The McDonnell Genome Institute",
                           "url": "http://genome.wustl.edu/",
                           "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                           "profile_image": {
                               "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                           }
                       }
                   }
               },
               "last_modified": {
                   "timestamp": "2017-11-01T11:40:09.927Z",
                   "user": {
                       "id": 418,
                       "name": "Paul Roepman",
                       "last_seen_at": "2018-02-14T11:56:51.985Z",
                       "username": "PaulRoepman",
                       "role": "curator",
                       "avatar_url": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Clinical Scientist",
                       "orcid": "0000-0003-1566-0258",
                       "display_name": "PaulRoepman",
                       "created_at": "2017-04-04T11:32:56.753Z",
                       "url": null,
                       "twitter_handle": null,
                       "facebook_profile": null,
                       "linkedin_profile": "proepman",
                       "bio": "",
                       "featured_expert": false,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": null,
                       "organization": {}
                   }
               },
               "last_reviewed": {
                   "timestamp": "2017-12-04T15:42:23.750Z",
                   "user": {
                       "id": 179,
                       "name": "Erica Barnell",
                       "last_seen_at": "2018-03-05T15:46:24.463Z",
                       "username": "ebarnell",
                       "role": "admin",
                       "avatar_url": "https://secure.gravatar.com/avatar/b9800d871c67538acd31728e8f509c80.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/b9800d871c67538acd31728e8f509c80.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/b9800d871c67538acd31728e8f509c80.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/b9800d871c67538acd31728e8f509c80.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/b9800d871c67538acd31728e8f509c80.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Research Scientist",
                       "orcid": "0000-0003-1631-1201",
                       "display_name": "ebarnell",
                       "created_at": "2016-07-06T14:48:11.341Z",
                       "url": "",
                       "twitter_handle": "",
                       "facebook_profile": "",
                       "linkedin_profile": "https://www.linkedin.com/in/erica-barnell-72b16a60",
                       "bio": "",
                       "featured_expert": false,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": "",
                       "organization": {
                           "id": 1,
                           "name": "The McDonnell Genome Institute",
                           "url": "http://genome.wustl.edu/",
                           "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                           "profile_image": {
                               "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                           }
                       }
                   }
               },
               "last_commented_on": {
                   "timestamp": "2017-11-01T10:54:47.582Z",
                   "user": {
                       "id": 418,
                       "name": "Paul Roepman",
                       "last_seen_at": "2018-02-14T11:56:51.985Z",
                       "username": "PaulRoepman",
                       "role": "curator",
                       "avatar_url": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                       "avatars": {
                           "x128": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=128",
                           "x64": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=64",
                           "x32": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=32",
                           "x14": "https://secure.gravatar.com/avatar/5e89a792925cb4b4e355c11a7b6c253d.png?d=identicon&r=pg&s=14"
                       },
                       "area_of_expertise": "Clinical Scientist",
                       "orcid": "0000-0003-1566-0258",
                       "display_name": "PaulRoepman",
                       "created_at": "2017-04-04T11:32:56.753Z",
                       "url": null,
                       "twitter_handle": null,
                       "facebook_profile": null,
                       "linkedin_profile": "proepman",
                       "bio": "",
                       "featured_expert": false,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": null,
                       "organization": {}
                   }
               },
               "accepted": {
                   "timestamp": "2016-02-26T14:59:53.268Z",
                   "user": {
                       "id": 41,
                       "name": "Nick Spies",
                       "last_seen_at": "2018-02-13T20:09:25.261Z",
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
                       "facebook_profile": "",
                       "linkedin_profile": "",
                       "bio": "Nick Spies is a staff analyst at the McDonnell Genome Institute and an MD student at Washington University School of Medicine. He has made substantial contributions to the development of genome analysis tools and resources at the Genome Institute including the Drug-Gene Interaction Database. He is a founding member of the CIViC team, helping to define the CIViC data model, and a leading content curator and a feature development consultant.",
                       "featured_expert": true,
                       "accepted_license": null,
                       "signup_complete": null,
                       "affiliation": "",
                       "organization": {
                           "id": 1,
                           "name": "The McDonnell Genome Institute",
                           "url": "http://genome.wustl.edu/",
                           "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                           "profile_image": {
                               "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                               "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                           }
                       }
                   }
               }
           },
           "fields_with_pending_changes": {},
           "gene_id": 20,
           "state_params": {
               "evidence_item": {
                   "id": 1122,
                   "name": "EID1122"
               },
               "variant": {
                   "id": 306,
                   "name": "AMPLIFICATION"
               },
               "gene": {
                   "id": 20,
                   "name": "ERBB2"
               }
           }
       }
       ],
       "acmg_codes": [],
       "drug_interaction_type": null,
       "fda_companion_test": true,
       "allele_registry_id": null,
       "phenotypes": [],
       "variant_origin": null,
       "lifecycle_actions": {
           "submitted": {
               "timestamp": "2018-01-11T19:34:41.434Z",
               "user": {
                   "id": 3,
                   "name": "Obi Griffith",
                   "last_seen_at": "2018-02-28T17:11:03.923Z",
                   "username": "obigriffith",
                   "role": "admin",
                   "avatar_url": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=32",
                   "avatars": {
                       "x128": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=128",
                       "x64": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=64",
                       "x32": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=32",
                       "x14": "https://secure.gravatar.com/avatar/4c468e9a95d6135e02eb66ee5f2fb574.png?d=identicon&r=pg&s=14"
                   },
                   "area_of_expertise": "Research Scientist",
                   "orcid": "0000-0002-0843-4271",
                   "display_name": "obigriffith",
                   "created_at": "2015-02-26T02:53:49.147Z",
                   "url": "http://genome.wustl.edu/people/individual/obi-griffith/",
                   "twitter_handle": "obigriffith",
                   "facebook_profile": "",
                   "linkedin_profile": "obigriffith",
                   "bio": "Dr. Griffith is Assistant Professor of Medicine and Assistant Director of the McDonnell Genome Institute at Washington University School of Medicine. He has worked in genomics and bioinformatics since the earliest phase of reference genome sequencing. He contributed to the Mammalian Gene Collection, producing some of the first full-length sequences for many human genes. He also was part of a small team of bioinformaticians that helped sequence and release the first whole genome reference sequence for the severe acute respiratory syndrome (SARS) virus at the height of the 2003 epidemic. He has contributed to the identification of molecular markers at the DNA, RNA and protein level that are useful for diagnosis and prognosis of thyroid, breast, lymphoma and other cancers. His lab’s research is focused on the development of informatics resources and personalized medicine strategies for cancer using genomic technologies. He is a co-creator of the CIViC resource.",
                   "featured_expert": true,
                   "accepted_license": null,
                   "signup_complete": null,
                   "affiliation": "",
                   "organization": {
                       "id": 1,
                       "name": "The McDonnell Genome Institute",
                       "url": "http://genome.wustl.edu/",
                       "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                       "profile_image": {
                           "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                       }
                   }
               }
           },
           "last_commented_on": {
               "timestamp": "2018-02-01T17:09:50.933Z",
               "user": {
                   "id": 517,
                   "name": "Susanna Kiwala",
                   "last_seen_at": "2018-03-07T16:34:21.576Z",
                   "username": "susannakiwala",
                   "role": "admin",
                   "avatar_url": "https://secure.gravatar.com/avatar/d41d8cd98f00b204e9800998ecf8427e.png?d=identicon&r=pg&s=32",
                   "avatars": {
                       "x128": "https://secure.gravatar.com/avatar/3214c84f88bf30642f2de9ab8c5e1c7f.png?d=identicon&r=pg&s=128",
                       "x64": "https://secure.gravatar.com/avatar/3214c84f88bf30642f2de9ab8c5e1c7f.png?d=identicon&r=pg&s=64",
                       "x32": "https://secure.gravatar.com/avatar/3214c84f88bf30642f2de9ab8c5e1c7f.png?d=identicon&r=pg&s=32",
                       "x14": "https://secure.gravatar.com/avatar/3214c84f88bf30642f2de9ab8c5e1c7f.png?d=identicon&r=pg&s=14"
                   },
                   "area_of_expertise": null,
                   "orcid": "",
                   "display_name": "susannakiwala",
                   "created_at": "2017-08-03T19:20:57.776Z",
                   "url": "",
                   "twitter_handle": "",
                   "facebook_profile": "",
                   "linkedin_profile": "",
                   "bio": "",
                   "featured_expert": false,
                   "accepted_license": null,
                   "signup_complete": null,
                   "affiliation": "",
                   "organization": {
                       "id": 1,
                       "name": "The McDonnell Genome Institute",
                       "url": "http://genome.wustl.edu/",
                       "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                       "profile_image": {
                           "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                       }
                   }
               }
           },
           "accepted": {
               "timestamp": "2018-01-17T16:41:35.694Z",
               "user": {
                   "id": 6,
                   "name": "Kilannin Krysiak",
                   "last_seen_at": "2018-03-06T23:19:03.508Z",
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
                   "bio": "Dr. Krysiak is an Instructor at the McDonnell Genome Institute at Washington University School of Medicine where she is involved in the comprehensive genomic analysis of cancer patient cohorts and “n-of-1” studies. She received her PhD in Molecular Genetics and Genomics at Washington University in St. Louis where she focused on the genetics of myelodysplastic syndrome through advanced flow cytometry techniques, primary cell culture and mouse models. She is a founding member of the CIViC team, helping to define the CIViC data model, and a leading content curator and feature development consultant.",
                   "featured_expert": true,
                   "accepted_license": null,
                   "signup_complete": null,
                   "affiliation": "",
                   "organization": {
                       "id": 1,
                       "name": "The McDonnell Genome Institute",
                       "url": "http://genome.wustl.edu/",
                       "description": "The McDonnell Genome Institute (MGI) is a world leader in the fast-paced, constantly changing field of genomics. A truly unique institution, we are pushing the limits of academic research by creating, testing, and implementing new approaches to the study of biology with the goal of understanding human health and disease, as well as evolution and the biology of other organisms.",
                       "profile_image": {
                           "x256": "/system/organizations/profile_images/000/000/001/x256/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x128": "/system/organizations/profile_images/000/000/001/x128/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x64": "/system/organizations/profile_images/000/000/001/x64/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x32": "/system/organizations/profile_images/000/000/001/x32/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976",
                           "x14": "/system/organizations/profile_images/000/000/001/x14/MGI_STANDARD4_logo_brown-example_v1b.png?1494525976"
                       }
                   }
               }
           }
       },
       "provisional_values": {},
       "errors": {}
   }
