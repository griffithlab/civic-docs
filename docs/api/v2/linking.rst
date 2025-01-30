Linking
=======

For convenience, the CIViC API provides a method for linking to entities on the front end website using only a single identifier. This allows external integrations to build links to CIViC without needing an entire hierarchy of ids. The API supports two link formats, documented below, that behave identically.

These routes will return a ``404`` response if the provided ID is not found. Otherwise, they will return a ``302`` redirect to the canonical frontend link for the entity in question.

Resource Style Links
--------------------

.. rubric:: Resource Style Link Format
.. parsed-literal::

   https://civicdb.org/links/:entity_type/:entity_id

.. rubric:: Example Resource Style Link

To link to the CIViC page for the Entrez Gene 1956 (*EGFR*) with the resource
style format:

.. parsed-literal::

   https://civicdb.org/links/entrez_id/1956

.. rubric:: Example 302 redirect
.. parsed-literal::

   https://civicdb.org/genes/19/summary

Query Parameter Links
---------------------

.. rubric:: Query Parameter Link Format
.. parsed-literal::

   https://civicdb.org/links?idtype=:entity_type&id=:entity_id

.. rubric:: Example Query Parameter Link

To link to the CIViC page for the variant with the CIViC internal ID 12 (*BRAF*
V600E) with the query parameter format:

.. parsed-literal::

   https://civicdb.org/links?idtype=variant&id=12

.. rubric:: Example 302 redirect
.. parsed-literal::

   https://civicdb.org/variants/12/summary

Supported Entity and ID Types
-----------------------------

CIViC supports the following entity and id types for generating shortened links:

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Entity Type
     - Description
   * - feature
     - CIViC Feature ID
   * - gene
     - CIViC Gene Feature ID
   * - entrez_id
     - Entrez Gene ID
   * - entrez_name
     - Entrez Name (typically HGNC Symbol)
   * - factor
     - CIViC Factor Feature ID
   * - fusion
     - CIViC Fusion Feature ID
   * - variant
     - CIViC Variant ID
   * - allele_registry
     - Variant Allele Registry ID
   * - variant_group
     - CIViC Variant Group ID
   * - evidence
     - CIViC Evidence ID
   * - assertion
     - CIViC Assertion ID
   * - disease
     - CIViC Disease ID
   * - doid
     - Disease Ontology ID
   * - drug
     - CIViC Therapy ID
   * - therapies
     - CIViC Therapy ID
   * - ncit_id
     - NCIthesaurus ID
   * - phenotype
     - CIViC Phenotype ID
   * - hpo_id
     - Human Phenotype Ontology ID
   * - revision
     - CIViC Revision ID

For more natural seeming resource based endpoints, the plural versions of the primary CViC entity types are also supported (``genes``, ``variants``, ``evidence_items``, ``variant_groups``, ``assertions``, ``revisions``) and behave identically to their singular counterparts.
