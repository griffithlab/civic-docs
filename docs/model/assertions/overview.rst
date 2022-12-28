Assertions Overview
===================
An assertion classifies the clinical significance of a variant-disease association under recognized guidelines (see AMP Classification, NCCN Guidelines, for more).

..
   Filename: BGA-113_assertion-model  Artboard: model

.. thumbnail:: /images/figures/assertions-overview_fig1.png
   :alt: Figure showing an overview of the attributes and associations of a CIViC Assertion
   :title: Figure 1: Assertion Attributes and Associations
   :show_caption: True

|

The CIViC Assertion (AID) summarizes a collection of Evidence Items (EIDs) that covers predictive/therapeutic, diagnostic, prognostic, predisposing or oncogenic information for a molecular profile (variant) in a specific cancer context (Figure 1). Functional Assertions are not currently supported. In general, an Assertion of a certain Type (e.g. Diagnostic) will be supported by a collection of Evidence Items (EIDs) of the same type, but Functional EIDs may be used to support Assertions of other types. The collection of EIDs associated with an Assertion should cover the important clinically relevant findings for the variant in the context of the specific cancer (and drug entity for Predictive Assertions). Assertion summaries mention NCCN or other practice guidelines related to the variant, as well as FDA drug approvals. In place of the curator assigned star rating found in CIViC Evidence Items, CIViC Assertions utilize widely adopted, published guidelines for variant tiering and pathogenicity/oncogenicity assessment, which are detailed below. CIViC Assertions are the primary entity that make up CIViC submissions to ClinVar.

CIViC currently has two main types of Assertions: those based on variants of primarily somatic origin (predictive/therapeutic, prognostic, diagnostic, and oncogenic) and those based on variants of primarily germline origin (predisposing). When the number and quality of Predictive, Prognostic, Diagnostic, Predisposing or Oncogenic Evidence Items (EIDs) in CIViC sufficiently cover what is known for a particular Molecular Profile and cancer type, then a corresponding assertion may be created in CIViC.

