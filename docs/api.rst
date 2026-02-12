CIViC API
=========

V2 API
------

The V2 API documentation can be found `here <https://griffithlab.github.io/civic-v2/>`_.

Our full API documentation can be found `on GitHub <https://griffithlab.github.io/civic-v2/>`_.

We've developed `a graphical user interface <https://civicdb.org/api/graphiql>`_ for accessing the new API, including a set of useful example queries.

A set of example usage scripts of the API in Python, R, and Ruby can be found on our `GitHub repo <https://github.com/griffithlab/civic-v2/tree/main/examples>`_.

API Usage Expectations
######################
By default, API queries against the CIViC knowledgebase are rate-limited to 3 requests / second as measured over a 5 minute window. This allows you to burst higher than that rate for brief periods, or sustain that rate indefinitely. If you generate a (free) API key and provide it with your requests, that limit does not apply. We do however, reserve the right to impose additional rate limits to curb abuse or overly excessive use. We ask that 
users with high-throughput or continuous use needs consider using `CIViCpy <https://docs.civicpy.org>`_
for these purposes.

.. toctree::
   :maxdepth: 2
   :caption: V2 Contents:

   api/v2/linking



V1 API (deprecated)
-------------------

CIViC provided a RESTful API that has been deprecated and is no longer available.
