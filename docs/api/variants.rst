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

   curl https://civicdb.org/api/variants?count=1

.. rubric:: Example Response
.. command-output:: curl -s https://civicdb.org/api/variants?count=1 | jq '.'
   :shell:

Get details for a specific variant
----------------------------------

This endpoint retrieves details about a specific variant, given its internal CIViC id.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/variants/:id

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/variants/13

.. rubric:: Example Response
.. command-output:: curl -s https://civicdb.org/api/variants/13 | jq '.'
   :shell:
