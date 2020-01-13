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

   curl https://civicdb.org/api/evidence_items?count=1

.. rubric:: Example Response
.. command-output:: curl -s https://civicdb.org/api/evidence_items?count=1 | python -m json.tool
   :shell:

Get details for a specific evidence item
----------------------------------------

This endpoint retrieves details about a specific evidence item, given its internal CIViC id.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/evidence_items/:id

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/evidence_items/512

.. rubric:: Example Response
.. command-output:: curl -s https://civicdb.org/api/evidence_items/512 | python -m json.tool
   :shell:
