.. include:: /generated/civic.docs-aliases.rst

.. _evidence-significance:

Significance
============
Significance describes how the variant is related to a specific, clinically-relevant property as described in the Evidence Statement. Significance terms vary depending on the Evidence Type (e.g. "Resistance" for Predictive Evidence, "Better Outcome" for Prognostic Evidence, etc.).

Understanding Significance
--------------------------
The available options for Significance depend on the Evidence Type selected for the Evidence statement. If a Predictive Evidence Type is selected, Significance can include: Sensitivity/Response, Resistance, Adverse Response, Reduced Sensitivity, or N/A. Each of these refers to the association between the Molecular Profile and clinical or preclinical response of the therapeutic(s). If a Diagnostic Evidence Type is selected, the Significance can be either Positive or Negative. A Positive Diagnostic Evidence Item implies that the Molecular Profile is associated with diagnosis of disease or disease subtype whereas a Negative Diagnostic Evidence Item implies lack of association. If a Prognostic Evidence Type is selected, the Significance options include: Better Outcome, Poor Outcome, or N/A. The N/A option can be used to imply that the variant does not have an impact on patient prognosis. A Functional Evidence Type should be associated with one of the following Significance values: Gain of Function, Loss of Function, Unaltered Function, Neomorphic, Dominant Negative, or Unknown. These options allow curators to indicate how the variant impacts the biological function described in the Evidence Statement. Predisposing and Oncogenic Evidence use the Significance values Predisposition/Oncogenicity and Protectiveness. However, final classification of the Significance for these Evidence Types should be established at the assertion level using the appropriate guidelines. 

.. rubric:: Significance for Predictive Evidence
.. list-table::
   :widths: 25 5 70
   :header-rows: 1
   :class: cvc-icon-table

   * - Significance
     - Icon
     - Definition
   * - Sensitivity/Response
     - |attribute-sensitivityresponse|
     - Associated with a clinical or preclinical response to treatment
   * - Reduced Sensitivity
     - |attribute-reducedsensitivity|
     - Response to treatment is lower than seen in other treatment contexts
   * - Resistance
     - |attribute-resistance|
     - Associated with clinical or preclinical resistance to treatment
   * - Adverse Response
     - |attribute-adverseresponse|
     - Associated with an adverse response to drug treatment
   * - N/A
     - |attribute-na|
     - Variant does not inform clinical interpretation

.. rubric:: Significance for Diagnostic Evidence
.. list-table::
   :widths: 25 5 70
   :header-rows: 1
   :class: cvc-icon-table

   * - Significance
     - Icon
     - Definition
   * - Positive
     - |attribute-positive|
     - Associated with diagnosis of disease or subtype
   * - Negative
     - |attribute-negative|
     - Associated with lack of disease or subtype

.. rubric:: Significance for Prognostic Evidence
.. list-table::
   :widths: 25 5 70
   :header-rows: 1
   :class: cvc-icon-table

   * - Significance
     - Icon
     - Definition
   * - Better Outcome
     - |attribute-betteroutcome|
     - Demonstrates better than expected clinical outcome
   * - Poor Outcome
     - |attribute-pooroutcome|
     - Demonstrates worse than expected clinical outcome
   * - N/A
     - |attribute-na|
     - Variant does not inform clinical action

.. rubric:: Significance for Predisposing Evidence
.. list-table::
   :widths: 25 5 70
   :header-rows: 1
   :class: cvc-icon-table

   * - Significance
     - Icon
     - Definition
   * - Predisposition
     - |attribute-predisposition|
     - Germline variant has predisposing potential for cancer, and may meet select ACMG/AMP criteria supporting pathogenic or benign classification.
   * - Protectiveness
     - |attribute-protectiveness|
     - Germline variant has properties that protect individuals from acquiring cancer.

.. rubric:: Significance for Functional Evidence
.. list-table::
   :widths: 25 5 70
   :header-rows: 1
   :class: cvc-icon-table

   * - Significance
     - Icon
     - Definition
   * - Gain of Function
     - |attribute-gainoffunction|
     - Sequence variant confers an increase in normal gene function
   * - Loss of Function
     - |attribute-lossoffunction|
     - Sequence variant confers a diminished or abolished function
   * - Unaltered Function
     - |attribute-unalteredfunction|
     - Gene product of sequence variant is unchanged
   * - Neomorphic
     - |attribute-neomorphic|
     - Sequence variant creates a novel function
   * - Dominant Negative
     - |attribute-dominantnegative|
     - Sequence variant abrogates function of wildtype allele gene product
   * - Unknown
     - |attribute-unknown|
     - Sequence variant that cannot be precisely defined by the other listed categories

.. rubric:: Significance for Oncogenic Evidence
.. list-table::
   :widths: 25 5 70
   :header-rows: 1
   :class: cvc-icon-table

   * - Significance
     - Icon
     - Definition
   * - Oncogenicity
     - |attribute-oncogenicity|
     - Somatic variant has oncogenic potential for driving cancer, and may meet select ClinGen/CGC/VICC criteria supporting pathogenic or benign classification.
   * - Protectiveness
     - |attribute-protectiveness|
     - Somatic variant has a protective role against cancer.
