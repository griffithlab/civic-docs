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

   curl https://civicdb.org/api/assertions?count=1

.. rubric:: Example Response
.. command-output:: curl -s https://civicdb.org/api/assertions?count=1 | python -m json.tool
   :shell:

Get details for a specific assertion
------------------------------------

This endpoint retrieves details about a specific assertion, given its internal CIViC id.

.. rubric:: HTTP Request Format
.. parsed-literal::

   GET https://civicdb.org/api/assertions/:id

.. rubric:: Example Request
.. parsed-literal::

   curl https://civicdb.org/api/assertions/9

.. rubric:: Example Response
.. command-output:: curl  -s https://civicdb.org/api/assertions/9 |  python -m json.tool
   :shell:
