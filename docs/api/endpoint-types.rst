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
.. command-output:: curl -s https://civicdb.org/api/genes?count=1 | jq '.'
   :shell:

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

    curl https://civicdb.org/api/genes/533

.. rubric:: Example /genes Detail Response
.. command-output:: curl -s https://civicdb.org/api/genes/533 | jq '.'
   :shell:
