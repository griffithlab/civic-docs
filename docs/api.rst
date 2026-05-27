CIViC API
=========

V2 API
------

The V2 API documentation can be found `here <https://griffithlab.github.io/civic-v2/>`_.

Our full API documentation can be found `on GitHub <https://griffithlab.github.io/civic-v2/>`_.

We've developed `a graphical user interface <https://civicdb.org/api/graphiql>`_ for accessing the new API, including a set of useful example queries.

A set of example usage scripts of the API in Python, R, and Ruby can be found on our `GitHub repo <https://github.com/griffithlab/civic-v2/tree/main/examples>`_.

Using API Keys in Requests
##########################
CIViC API keys authenticate API requests as the user who generated the key. They
can be used for requests that require a logged-in user, such as mutations, and
for high-throughput API clients that should not be subject to the default
anonymous request rate limit.

To generate an API key, sign in to CIViC, open your user profile, choose
``Manage API Keys``, and click ``Generate New API Key``. Copy the key when it is
created and store it in a secure location, such as a password manager. CIViC only
shows the full token at creation time; after that, the key list displays a
masked reminder. Revoke any key that is no longer needed or may have been
exposed.

Include the key in the HTTP ``Authorization`` header using the bearer token
scheme:

.. code-block:: text

   Authorization: Bearer <CIViC_API_KEY>

For example, a GraphQL request with ``curl``:

.. code-block:: bash

   curl https://civicdb.org/api/graphql \
     -H "Content-Type: application/json" \
     -H "Authorization: Bearer ${CIVIC_API_KEY}" \
     --data '{"query":"query { viewer { id username } }"}'

Or with Python:

.. code-block:: python

   import os
   import requests

   response = requests.post(
       "https://civicdb.org/api/graphql",
       headers={
           "Authorization": f"Bearer {os.environ['CIVIC_API_KEY']}",
           "Content-Type": "application/json",
       },
       json={"query": "query { viewer { id username } }"},
   )
   response.raise_for_status()
   print(response.json())

Do not place API keys in URLs, query strings, checked-in scripts, or shared
notebooks. Use environment variables or a secrets manager when running automated
clients.

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
