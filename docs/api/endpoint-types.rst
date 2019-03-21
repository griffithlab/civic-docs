Endpoint Types
==============
The API for consuming CIViC data can mostly be broken down into two different types of endpoints: **index** and **detail**.

Index Endpoints
---------------
The index endpoints provide high level overview information about a collection of entities all at once and allow a user to page through all the entities in the system. Index endpoints provide two top-level keys in their JSON structure: :code:`_meta` and :code:`records`.

.. rubric:: Example /genes Request
.. parsed-literal::

    curl https://civicdb.org/api/genes

.. rubric:: Example /genes Response (partial)
.. code-block:: json
   :linenos: 

   {
     "_meta": {
         "current_page": 1,
         "per_page": 25,
         "total_pages": 13,
         "total_count": 312,
         "links": {
             "next": "https://civicdb.org/api/genes?count=25&page=2",
             "previous": null
         }
     },
     "records": ["... 25 gene objects ..."]
   }

Meta Attribute
~~~~~~~~~~~~~~
As seen to above, the :code:`_meta` section contains information about the total number of available records, the page size, and provides links to the next and previous page of results. These links can be used to easily traverse all of the records in CIViC. A :code:`null` entry for :code:`next` (or :code:`previous`) indicates that you have reached the end of the collection.

Records Attribute
~~~~~~~~~~~~~~~~~
The records section will contain the actual objects requested in the API call (ie: genes, variants or evidence_items)

If you do not wish to use the links in the :code:`_meta` section, index endpoints also accept manual pagination parameters in the query string:

.. rubric:: Example /genes Request with Manual Pagination
.. parsed-literal::

    curl https://civicdb.org/api/genes?page=2&count=25

.. rubric:: Meta Pagination Parameters
.. list-table::
   :widths: 15 15 70
   :header-rows: 1

   * - Parameter
     - Default
     - Description
   * - page
     - 1
     - Which page of results to return
   * - count
     - 25
     - How many records to return on a single page

Detail Endpoints
----------------
Detail endpoints return the full CIViC record for a single entity, specified explicitly by id. In addition to the high level overview information returned by the index endpoint, this complete record will include information about data provenance, timestamps, and secondary relationships. Unlike the index endpoints, detail endpoints do not have separate :code:`_meta` and :code:`records` sections as only a single record is returned.

.. rubric:: Example /genes Detail Request
.. parsed-literal::

    curl https://civicdb.org/api/genes/19

.. rubric:: Example /genes Detail Response (partial)

.. code-block:: json
   :linenos: 

   {
      "id": 19,
      "name": "EGFR",
      "entrez_id": 1956,
      "description": "EGFR is widely recognized for its importance in cancer. Amplification and mutations have been shown to be driving events in many cancer types. Its role in non-small cell lung cancer, glioblastoma and basal-like breast cancers has spurred many research and drug development efforts. Tyrosine kinase inhibitors have shown efficacy in EGFR amplfied tumors, most notably gefitinib and erlotinib. Mutations in EGFR have been shown to confer resistance to these drugs, particularly the variant T790M, which has been functionally characterized as a resistance marker for both of these drugs. The later generation TKI's have seen some success in treating these resistant cases, and targeted sequencing of the EGFR locus has become a common practice in treatment of non-small cell lung cancer. Overproduction of ligands is another possible mechanism of activation of EGFR. ERBB ligands include EGF, TGF-a, AREG, EPG, BTC, HB-EGF, EPR and NRG1-4 (for detailed information please refer to the respective ligand section). In ligand-activated cancers, Cetuximab appears to be more effective than tyrosine-kinase inhibitors (Arteaga et. al.).",
      "variants": [ "213 items" ],
      "aliases": [
            "EGFR",
            "mENA",
            "PIG61",
            "NISBD2",
            "HER1",
            "ERBB1",
            "ERBB"
      ],
      "type": "gene",
      "lifecycle_actions": { "2 items" },
      "sources": [ "3 items" ],
      "provisional_values": {},
      "errors": {}
   }

