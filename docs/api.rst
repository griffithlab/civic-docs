CIViC API
=========

V2 API
------

In April 2022 CIViC V2 was launched, which includes a new GraphQL API. The
old API is still available at v1.civicdb.org/api. It accesses a frozen
datadump and does not include any new data since the switchover. While we
expect the V1 API to be accessible for a few more months (deprecation date
forthcoming) any new integrations should use the V2 API and existing
integrations should switch to the V2 API as soon as possible. Please contact
us at help@civicdb.org for assistance.

The V2 documentation can be found `here <https://griffithlab.github.io/civic-v2/>`_.

A graphical userface for accessing the new API can be found `here
<https://civicdb.org/api/graphiql>`_.

Please stay tuned for a more comprehensive API user guide.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   api/v2/linking


V1 API (deprecated)
-------------------

CIViC provides a simple API that can be used over HTTP in the programming language of your choice or even at the command line.

The CIViC API attempts to be RESTful whenever appropriate, which hopefully makes it intuitive to use. There are four main entities in the system that a user may interact with: Genes, Variants, Variant Groups, and Evidence Items. These entities form a hierarchy that is reflected in the API endpoints. A Gene has one or more Variants, each of which may have one or more Evidence Items. Variants may also be collected into Variant Groups.

This documentation provides example requests and responses for most endpoints. The responses are edited for brevity, but should include instances of each top level key for reference. You can toggle between viewing a request and its corresponding response using the tabs on the right of the page.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   api/v1/endpoint-types
   api/v1/genes
   api/v1/variants
   api/v1/evidence
   api/v1/variant_groups
   api/v1/assertions
   api/v1/linking
   api/v1/metadata
   api/v1/throttling
   api/v1/add_evidence
