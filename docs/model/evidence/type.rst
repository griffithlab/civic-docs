.. include:: /generated/civic.docs-aliases.rst

.. _evidence-type:

Type
====
The Evidence Type refers to the type of clinical (or biological) association described by the Evidence Item’s clinical summary.

Understanding Evidence Types
----------------------------
Six Evidence Types are currently supported: Predictive (i.e. Therapeutic), Diagnostic, Prognostic, Predisposing, Oncogenic, and Functional. Each Evidence Type describes the clinical or biological effect a Molecular Profile (MP) has on the following: therapeutic response (Predictive), determining a patient’s diagnosis or disease subtype (Diagnostic), predicting disease progression or patient survival (Prognostic), disease susceptibility (Predisposing), or biological alterations relevant to a cancer phenotype (Oncogenic) or protein function (Functional). Selecting an Evidence Type has implications on available selections for Significance, which are detailed on the :ref:`Evidence Significance page <evidence-significance>`.


.. list-table::
   :widths: 10 5 85
   :header-rows: 1
   :class: cvc-icon-table

   * - Type
     - Symbol
     - Definition
   * - Diagnostic
     - |attribute-diagnostic|
     - Evidence pertains to a variant's impact on patient diagnosis (cancer subtype)
   * - Predictive
     - |attribute-predictive|
     - Evidence pertains to a variant's effect on therapeutic response
   * - Prognostic
     - |attribute-prognostic|
     - Evidence pertains to a variant's impact on disease progression, severity, or patient survival.
   * - Predisposing
     - |attribute-predisposing|
     - Evidence pertains to a germline Molecular Profile's role in conferring susceptibility to disease (including pathogenicity evaluations)
   * - Oncogenic
     - |attribute-oncogenic|
     - Evidence pertains to a somatic variant's involvement in tumor pathogenesis as described by the Hallmarks of Cancer.
   * - Functional
     - |attribute-functional|
     - Evidence pertains to a variant that alters biological function from the reference state.

Extensive documentation for curating Evidence types is provided on the :ref:`Curating Evidence page <curating-evidence-general>`. Be sure to closly study the examples for each type.

