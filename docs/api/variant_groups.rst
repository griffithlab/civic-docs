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

   curl https://civicdb.org/api/variant_groups?count=1

.. rubric:: Example Response
.. command-output:: curl -s https://civicdb.org/api/variant_groups?count=1 | python -m json.tool
   :shell:

Get details for a specific variant group
----------------------------------------

This endpoint retrieves details about a specific variant group, given its internal CIViC id.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/variant_groups/:id

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/variant_groups/21

.. rubric:: Example Response
.. command-output:: curl -s https://civicdb.org/api/variant_groups/21 | python -m json.tool
   :shell:
