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

    curl https://civicdb.org/api/genes?count=1

.. rubric:: Example Response
.. command-output:: curl -s https://civicdb.org/api/genes?count=1 | python -m json.tool
   :shell:

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

   curl https://civicdb.org/api/genes/AXL?identifier_type=entrez_symbol

.. rubric:: Example Response
.. command-output:: curl -s https://civicdb.org/api/genes/AXL?identifier_type=entrez_symbol | python -m json.tool
   :shell:

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

   curl https://civicdb.org/api/genes/AXL,CDK2?identifier_type=entrez_symbol

.. rubric:: Example Response
.. command-output:: curl -s https://civicdb.org/api/genes/AXL,CDK2?identifier_type=entrez_symbol | python -m json.tool
   :shell:
