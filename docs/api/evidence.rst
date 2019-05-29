Evidence Items
==============

The evidence items endpoint allows users to enumerate all of the evidence items present in CIViC as well as retrieve more detailed information on a specific evidence item. This is the endpoint that should be used to obtain a complete listing of every evidence item in CIViC.

Get a list of evidence items
----------------------------

This endpoint returns a listing of evidence items in CIViC. This index style endpoint is `paginated` by default. You can use the ``count`` and ``page`` parameters or the ``previous`` and ``next`` links to iterate through all the evidence items.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/evidence_items

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
     - How many evidence items to return on a single page

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/evidence_items

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   {
     "_meta": {
       "current_page": 1,
       "per_page": 25,
       "total_pages": 69,
       "total_count": 1722,
       "links": {
         "next": "https://civicdb.org/api/evidence_items?count=25&page=2",
         "previous": null
       }
     },
     "records": [
       {
         "id": 1,
         "name": "EID1",
         "description": "JAK2 V617F is not associated with lymphoid leukemia (B-lineage ALL, T-ALL or CLL).",
         "disease": {
           "id": 1,
           "name": "Lymphoid Leukemia",
           "display_name": "Lymphoid Leukemia",
           "doid": "10747",
           "url": "http://www.disease-ontology.org/?id=DOID:10747"
         },
         "drugs": [],
         "rating": 4,
         "evidence_level": "B",
         "evidence_type": "Diagnostic",
         "clinical_significance": "Negative",
         "evidence_direction": "Supports",
         "variant_origin": "Somatic Mutation",
         "drug_interaction_type": null,
         "status": "accepted",
         "open_change_count": 0,
         "type": "evidence",
         "source": {
           "id": 51,
           "name": "The JAK2V617F activating mutation occurs in chronic myelomonocytic leukemia and acute myeloid leukemia, but not in acute lymphoblastic leukemia or chronic lymphocytic leukemia.",
           "citation": "Levine et al., 2005, Blood",
           "pubmed_id": "16081687",
           "source_url": "http://www.ncbi.nlm.nih.gov/pubmed/16081687",
           "open_access": true,
           "pmc_id": "PMC1895066",
           "publication_date": {
             "year": 2005,
             "month": 11,
             "day": 15
           },
           "journal": "Blood",
           "full_journal_title": "Blood",
           "status": "fully curated"
         },
         "variant_id": 64
       },
       {
         "id": 2,
         "name": "EID2",
         "description": "GIST tumors harboring PDGFRA D842V mutation are more likely to be benign than malignant.",
         "disease": {
           "id": 2,
           "name": "Gastrointestinal Stromal Tumor",
           "display_name": "Gastrointestinal Stromal Tumor",
           "doid": "9253",
           "url": "http://www.disease-ontology.org/?id=DOID:9253"
         },
         "drugs": [],
         "rating": 3,
         "evidence_level": "B",
         "evidence_type": "Diagnostic",
         "clinical_significance": "Negative",
         "evidence_direction": "Supports",
         "variant_origin": "Somatic Mutation",
         "drug_interaction_type": null,
         "status": "accepted",
         "open_change_count": 0,
         "type": "evidence",
         "source": {
           "id": 52,
           "name": "A great majority of GISTs with PDGFRA mutations represent gastric tumors of low or no malignant potential.",
           "citation": "Lasota et al., 2004, Lab. Invest.",
           "pubmed_id": "15146165",
           "source_url": "http://www.ncbi.nlm.nih.gov/pubmed/15146165",
           "open_access": null,
           "pmc_id": null,
           "publication_date": {
             "year": 2004,
             "month": 7
           },
           "journal": "Lab. Invest.",
           "full_journal_title": "Laboratory investigation; a journal of technical methods and pathology",
           "status": "fully curated"
         },
         "variant_id": 99
       },
     ]
   }

Get details for a specific evidence item
----------------------------------------

This endpoint retrieves details about a specific evidence item, given its internal CIViC id.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/evidence_items/:id

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/evidence_items/512

.. rubric:: Example Response (partial)
.. code-block:: json
   :linenos:

   {
     "id": 512,
     "name": "EID512",
     "description": "Nonsense mutations in SMARCA4 were associated with small cell carcinoma of the ovary, hypercalcemic type in 10/10 tumor samples, and were rarely found in other solid tumor types catalogued by TCGA.",
     "disease": {
       "id": 253,
       "name": "Small Cell Carcinoma Of The Ovary Hypercalcemic Type",
       "display_name": "Small Cell Carcinoma Of The Ovary Hypercalcemic Type",
       "doid": "7651",
       "url": "http://www.disease-ontology.org/?id=DOID:7651"
     },
     "drugs": [],
     "rating": 5,
     "evidence_level": "B",
     "evidence_type": "Diagnostic",
     "clinical_significance": "Positive",
     "evidence_direction": "Supports",
     "variant_origin": "Somatic Mutation",
     "drug_interaction_type": null,
     "status": "accepted",
     "open_change_count": 0,
     "type": "evidence",
     "source": {
       "id": 316,
       "name": "Recurrent SMARCA4 mutations in small cell carcinoma of the ovary.",
       "citation": "Jelinic et al., 2014, Nat. Genet.",
       "pubmed_id": "24658004",
       "source_url": "http://www.ncbi.nlm.nih.gov/pubmed/24658004",
       "open_access": null,
       "pmc_id": null,
       "publication_date": {
         "year": 2014,
         "month": 5
       },
       "journal": "Nat. Genet.",
       "full_journal_title": "Nature genetics",
       "status": "fully curated"
     },
     "variant_id": 217,
     "errors": {},
     "lifecycle_actions": {
       "accepted": {
         "order": 1,
         "timestamp": "2015-08-05T18:47:08.046Z",
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
           "bio": "Nick Spies is a staff analyst at the McDonnell Genome Institute and an MD student at Washington University School of Medicine. He has made substantial contributions to the development of genome analysis tools and resources at the Genome Institute including the Drug-Gene Interaction Database. He is a founding member of the CIViC team, helping to define the CIViC knowledge model, and a leading content curator and a feature development consultant.",
           "featured_expert": true,
           "accepted_license": null,
           "signup_complete": null
         }
       }
     },
     "fields_with_pending_changes": {}
   }
