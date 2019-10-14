Evidence Overview
=================

The following figure shows the attributes of a CIViC Evidence Item, and the options or values available for each.

.. image:: /images/figures/CIViC_evidence-item-fields_v1b.png

The rows in the following table describe the minimal components of a CIViC Evidence Item. Several Evidence Statements are synthesized at the Variant level into Variant Summaries but each Evidence Statement is directly linked to a single article in PubMed. *More specific guidelines about Evidence Item components can be found in additional help tabs*.


**Evidence Attributes**

.. list-table::
   :widths: 10 50 20 20
   :header-rows: 1

   * - Attribute
     - Description
     - Example
     - Source
   * - :ref:`evidence-gene`
     - The symbol and ID of the gene implicated.
     - ESR1 (Entrez ID: 2099)
     - CIViC (Entrez)
   * - :ref:`evidence-variant`
     - Genomic event/mutation (Single nucleotide variant,
       Insertion/deletion, Gene fusion, Copy number variant, etc.)
       implicated.
     - Y537S
     - CIViC
   * - :ref:`evidence-statement`
     - Human readable interpretation. Free-form text
       summary of this event’s potential clinical interpretations. This
       interpretation is the synthesis of all other information about an
       event and its relevance to clinical action and should be the living
       product of active discussion.
     - This study of 178 non-small cell lung
       cancer patients, the appearance of T790M mutation lead to resistance
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
       details on how to enter evidence of each of the four types:
       Predictive, Prognostic, Predisposing and Diagnostic. See 'Evidence
       Type' tab for more information.
     - Predictive - The variant is
       predictive of sensitivity or resistance to a therapeutic.
     - CIViC
   * - :ref:`evidence-direction`
     - An indicator of whether the evidence statement
       supports or refutes the clinical significance of an event. See
       'Evidence Type' tab for more information.
     - Supports - the evidence supports the clinical significance.
     - CIViC
   * - :ref:`evidence-clinical_significance`
     - The association with diagnostic/prognostic end
       point or treatment. See 'Evidence Type' tab for more information.
     - Resistant or Non-response - mutation is associated with resistance
       to therapy.
     - CIViC
   * - :ref:`evidence-origin`
     - Presumed cellular origin of the Variant in samples
       from the literature citation where the clinical effect of this
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
     - Lorem Ipsum
     - Lorem Ispum
     - Lorem Ipsum
   * - :ref:`evidence-drug`
     - For predictive evidence, indicates the therapy for which
       sensitivity or resistance is indicated (With PubChem ID if
       available).
     - Tamoxifen, Raloxifene (PubChem CIDs: 2733526, 5053).
     - CIViC (PubChem)
   * - Drug Interaction Type
     - For predictive evidence involving more than
       one drug, specifies the relationship between these drugs by
       indicating whether the drugs are Subtitutes for each other or are
       used in Sequential or Combination treatments.
     - Substitutes - The
       drugs listed are often considered to be of the same family, or
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
   * - :ref:`evidence-clinical_trial`
     - Lorem Ipsum
     - Lorem Ispum
     - Lorem Ipsum
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

