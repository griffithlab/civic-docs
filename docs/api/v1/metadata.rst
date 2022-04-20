Metadata
========

All core CIViC entities support several metadata endpoints that allow users to view discussion, revision history, and moderation history.

These endpoints can be accessed by appending an additional path segment onto a detail view URL. For example, to see the discussion thread for the Variant with CIViC id 5, you could access the endpoint:

.. parsed-literal::

   https://civicdb.org/api/variants/5/comments

Additionally, due to the hierarchical nature of CIViC entities, you can append the type of a child entity to the detail view of a parent entity in order to view the children.

For example, you could get all of the variants for a specific gene by querying ``https://civicdb.org/api/genes/:gene_id/variants`` or all the evidence_items for a specific variant at the path ``https://civicdb.org/api/variants/:variant_id/evidence_items``.

.. rubric:: Endpoint Types
.. list-table::
   :widths: 20 40 40
   :header-rows: 1

   * - Endpoint
     - Purpose
     - Example
   * - ``/comments``
     - View discussion for an entity
     - ``/api/genes/1/comments``
   * - ``/suggested_changes``
     - View proposed revisions for an entity
     - ``/api/genes/6/suggested_changes``
   * - ``/revisions``
     - View the entire revision history for an entity
     - ``/api/genes/6/revisions``

.. rubric:: Supported Endpoints for CIViC Entities
.. list-table::
   :widths: 20 40 40
   :header-rows: 1

   * - CIViC Entity
     - Base Path
     - Supported Endpoints
   * - Genes
     - ``/api/genes/:gene_id``
     - ``/comments``, ``/suggested_changes``, ``/revisions``, ``/variants``
   * - Variants
     - ``/api/variants/:variant_id``
     - ``/comments``, ``/suggested_changes``, ``/revisions``, ``/evidence_items``
   * - Evidence Items
     - ``/api/evidence_items/:eid``
     - ``/comments``, ``/suggested_changes``, ``/revisions``
   * - Variant Groups
     - ``/api/variant_groups/:variant_group_id``
     - ``/comments``, ``/suggested_changes``, ``/revisions``
   * - Assertions
     - ``/api/assertions/:aid``
     - ``/comments, /suggested_changes, /revisions``
