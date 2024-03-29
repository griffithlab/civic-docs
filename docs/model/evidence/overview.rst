Evidence Overview
=================

The following figure shows the attributes of a CIViC Evidence Item, and the options or values available for each.

..
   Filename: BGA-113_evidence-model.graffle Artboard: model

.. thumbnail:: /images/figures/evidence_overview_fig1.png
   :alt: Figure depicting the CIViC Evidence Item's attributes and associations
   :title: Figure 1: Evidence Item Attributes and Associations
   :show_caption: True

The rows in the following table describe the minimal components of a CIViC Evidence Item. Several Evidence Statements are synthesized at the Molecular Profile (Variant) level into a Molecular Profile Description. However, each Evidence Statement is directly linked to a single article in PubMed or ASCO/ASH abstract. *More specific guidelines about Evidence Item components can be found in the additional sections outlined in the table of contents*.

**Evidence Attributes**

.. list-table::
   :widths: 10 50 20 20
   :header-rows: 1

   * - Attribute
     - Description
     - Example
     - Source
   * - :ref:`evidence-molecular-profile`
     - Gene and Genomic event(s)/mutation(s) (e.g., Single nucleotide variant,
       Insertion/deletion, Gene fusion, Copy number variant, etc.)
       implicated. May be a simple comprised of a single variant or a more complex
       combination of variants.
     - ESR1 Y537S
     - CIViC
   * - :ref:`evidence-statement`
     - Human readable interpretation. Free-form text
       summary of this molecular profile’s potential clinical interpretations. This
       interpretation is the synthesis of all other information about the
       alteration(s) and its clinical relevance and should be the living
       product of active discussion.
     - In this study of 178 non-small cell lung
       cancer patients, the appearance of EGFR T790M mutation led to resistance
       to gefitinib.
     - CIViC
   * - :ref:`evidence-level`
     - The type of experiment from which the evidence is
       curated. From inferential, to proven association in clinical
       medicine. Refer to the additional documentation on evidence levels
       for definitions of the five levels allowed in CIViC: validated,
       clinical, pre-clinical, case study, and inferential.
     - Level B - Clinical Evidence.
     - CIViC
   * - :ref:`evidence-type`
     - Category of clinical action/relevance implicated by
       event. Refer to the additional documentation on evidence types for
       details on how to enter evidence of each of the six types:
       Predictive, Prognostic, Diagnostic, Predisposing, Oncogenic and Functional. See 'Evidence
       Type' tab for more information.
     - Predictive - The molecular profile (one or more variants) is
       predictive of sensitivity or resistance to a therapeutic.
     - CIViC
   * - :ref:`evidence-direction`
     - An indicator of whether the evidence statement
       supports or refutes the significance of an event. See
       'Evidence Type' tab for more information.
     - Supports - the evidence supports the significance.
     - CIViC
   * - :ref:`evidence-significance`
     - The impact of the molecular profile (one or more variants) for predictive, prognostic, diagnostic, oncogenic or functional evidence types.
       See 'Evidence Type' tab for more information.
     - Resistant or Non-response - mutation is associated with resistance
       to therapy.
     - CIViC
   * - :ref:`evidence-origin`
     - Presumed cellular origin of the Variant in samples
       from the literature citation where the effect of this
       Variant is being evaluated.
     - Somatic
     - CIViC
   * - :ref:`evidence-disease`
     - Specific disease or disease subtype that is associated
       with this event and its clinical implication. Links directly to
       Disease Ontology.
     - Estrogen-receptor positive breast cancer (DOID: 0060075).
     - CIViC (Disease Ontology)
   * - :ref:`evidence-associated_phenotype`
     - Specific phenotypes associated with the evidence statement.
     - Pancreatic cysts (HP:0001737).
     - The Human Phenotype Ontology (HPO)
   * - :ref:`evidence-therapy`
     - For predictive evidence, indicates the therapy for which
       sensitivity or resistance is indicated (With NCIt ID if
       available).
     - Tamoxifen, Raloxifene (NCIt IDs: C62078, C62078).
     - CIViC (NCIt)
   * - Therapy Interaction Type
     - For predictive evidence involving more than
       one Therapy, specifies the relationship between the therapies (usually drugs) by
       indicating whether they are Subtitutes for each other or are
       used in Sequential or Combination treatments.
     - Substitutes - The
       therapies listed are often considered to be of the same family, or
       behave similarly in a treatment setting.
     - CIViC
   * - Citation
     - Publication where the event was described/explored
       automatically generated from curator-provided PubMed ID and links to
       internal CIViC publication page showing all Evidence Items from the
       publication.
     - Toy et al., 2013, Nat. Genet. (PMID: 24185512)
     - CIViC (PubMed)
   * - PubMed ID
     - PubMed ID for publication where the event was
       described/explored with direct link to PubMed.
     - 24185512
     - CIViC (PubMed)
   * - :ref:`evidence-clinical-trial`
     - Clinical trial associated with the evidence item. 
     - NCT01154140
     - ClinicalTrials.gov
   * - :ref:`evidence-evidence_rating`
     - A rating on a 5-star scale, portraying the curators
       trust in the experiments from which the evidence is curated. Refer
       to the additional documentation on trust ratings for guidance on how
       to score an evidence item.
     - 5-stars - Strong, well supported
       evidence from a lab or journal with respected academic standing.
       Experiments are well controlled, and results are clean and
       reproducible across multiple replicates.
     - CIViC

