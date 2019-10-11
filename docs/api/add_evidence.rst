Constructing Add Evidence URLs
==============================

CIViC supports users constructions an Add Evidence URL that will
prefill the Add Evidence form with the values provided via URL parameters.
All values need to be URL-encoded (spaces and other special characters
replaced with %-encodings, see https://en.wikipedia.org/wiki/Percent-encoding).

.. rubric:: Base URL
.. parsed-literal::

   https://civicdb.org/add/evidence/basic?

.. rubric:: Supported Parameters
.. list-table::
   :header-rows: 1

   * - URL Attribute
     - URL Value
     - Example
     - Note
   * - geneId
     - Entrez ID
     - geneId=673
     - use geneId or geneName, but not both
   * - geneName
     - Entrez Name
     - geneName=BRAF
     - use geneId or geneName, but not both
   * - variantId
     - CIViC ID
     - variantId=1296
     - Use variantId or variantName, but not both
   * - variantName
     - CIViC Name (with special characters encoded)
     - variantName=V600E
     - Use variantId or variantName, but not both
   * - sourceType
     - A valid CIViC Source Type. Supported source types are:

       - ASCO
       - PubMed

     - sourceType=PubMed
     -
   * - citationId
     - ASCO Web ID or PubMed ID
     - citationId=123456
     - The ASCO Web ID is not the ASCO abstract number. The ASCO Web ID can be found in the URL of the abstract.
   * - variantOrigin
     - A valid CIViC Variant Origin (with special characters encoded). Supported variant origins are:

       - Somatic
       - Rare%20Germline
       - Common%20Germinline
       - N%2FA
       - Unknow

     - variantOrigin=Somatic
     -
   * - diseaseName
     - Valid CIViC Disease Name (with special characters encoded)
     - diseaseName=Cancer
     -
   * - evidenceType
     - A valid CIViC Evidence Type (with special characters encoded).
       Supported evidence types are:

       - Predictive
       - Diagnostic
       - Prognostic
       - Predisposing
       - Functional

     - evidenceType=Predisposing
     -
   * - evidenceLevel
     - A valid CIViC Evidence Level. Supported evidence levels are:

       - A
       - B
       - C
       - D
       - E

     - evidenceLevel=B
     -
   * - evidenceDirection
     - A valid CIViC Evidence Direction. Supported evidence directions are:

       - Supports
       - Does%20Not%20Support

     - evidenceDirection=Support
     -
   * - clinicalSignificance
     - A valid CIViC Clinical Significance (with special characters encoded). Supported values are:

       - Sensitivity%2FResponse
       - Resistance
       - Adverse%20Response
       - Reduced%20Sensitivity
       - Positive
       - Negative
       - Better%20Outcome
       - Poor%20Outcome
       - Pathogenic
       - Likely%20Pathogenic
       - Benign
       - Likely%20Benign
       - Uncertain%20Significance
       - Gain%20of%20Function
       - Loss%20of%20Function
       - Unaltered%20Function
       - Neomorphic
       - Unknown
       - N%2FA

     - clinicalSignificance=Benign
     - The available clinical significance depends on the evidence type
       chosen. More information about valid combinations can be found in the
       documentation for the `CIViC knowledge model <https://civic.readthedocs.io/en/latest/model/evidence/clinical_significance.html>`_.
