.. _evidence-origin:

Origin
======
Presumed source of the variant in the context of this study.

Understanding Variant Origin
----------------------------
The origin of a variant in a study is important for interpreting the results in context. Studies may provide specific information about the origin of the variant (somatic with tumor/normal paired data) while others may be more ambiguous (tumor-only sequencing with a variant that may be somatic or germline, e.g., BRCA1 mutation from a breast cancer sample). Documenting Variant Origin allows for quick filtering of evidence and provides context for the study compared to other studies that involve that variant.

Curating Variant Origin
-----------------------
The Variant Origin in and Evidence Item identifies whether the variant was presumed as an inherited (germline mutation) or acquired (somatic mutation) event in the context of the study. We generally consider somatic events to be the priority, as this is an area that has not been as well addressed by existing resources. However, germline mutations with established clinical relevance are acceptable. Germline polymorphisms (>1% allele frequency in the population) are considered low priority, again unless there is an established clinical relevance. We encourage the use of large population resources such as gnomAD_ for population frequency estimations rather than relying on the frequency reported by the original study. Polymorphisms described in association studies should be curated with great caution and may face additional scrutiny from CIViC moderators. For some variant types, the variant origin field may be unknown or N/A. For example, EXPRESSION variants are neither germline nor somatic and should be marked as N/A. Fusion variants are an unusual case in that they are often observed in the transcriptome but are usually accompanied by an underlying somatic (or germline) mutation. Most fusions should be entered as somatic. If in doubt, please note the issue at the time of your submission to encourage discussion during the moderation stage.

Expression variants should be marked as 'N/A'.

Fusions are often observed in the transcriptome but are usually accompanied by an underlying somatic (or germline) mutation.

Population frequencies should be based on current population databases (e.g., gnomAD_) rather than the original report.

.. _gnomAD: https://gnomad.broadinstitute.org

.. list-table::
   :widths: 25 5 70
   :header-rows: 1

   * - Origin
     - Symbol
     - Description
   * - Somatic
     - |ellipsis-h|
     - Highest priority variants in CIViC. May include presumed somatic variants largely driven by the usage in the original publication but should be approached with caution in instances of tumor-only analysis. Includes fusions.
   * - Rare Germline
     - |ellipsis-v|
     - Consist of heritable rare variants. Generally, <1% of the population relevant to the publication being cited.
   * - Common Germline
     - |signal|
     - Defined as variants with >1% allele frequency in the population relevant to the publication where the evidence is derived. Are welcome in CIViC, however, generally considered low priority for curation efforts.
   * - Combined
     - ||
     - Variants in the corresponding Complex Molecular Profile have heterogenous/multiple origins.
   * - Unknown
     - |question-circle|
     - May be used in instances where the publication is ambiguous about the origin of the variant although ordinarily an origin would be known (e.g., tumor-only analysis, analyses including both germline and somatic variants).
   * - N/A
     - |times-circle-o|
     - For variants such as 'Expression' where a germline or somatic origin is not applicable.

.. rubric:: Examples
.. list-table::
   :widths: 25 75

   * - Somatic
     - `DNAJB1-PRKACA (EID532)
       <https://civicdb.org/links/evidence/532>`_, 
       `BRAF V600E (EID1409)
       <https://civicdb.org/links/evidence/1409>`_,
       `KRAS Exon 2 Mutation (EID993)
       <https://civicdb.org/links/evidence/993>`_,
       `EGFR Amplification (EID473)
       <https://civicdb.org/links/evidence/473>`_
   * - Rare Germline
     - `BRCA2 Mutation (EID1371)
       <https://civicdb.org/links/evidence/1371>`_
   * - Common Germline
     - `GSTP1 I105V (EID670)
       <https://civicdb.org/links/evidence/670>`_,
       `UGT1A1*28 (EID1792)
       <https://civicdb.org/links/evidence/1792>`_
   * - Unknown
     - `FANCC Loss-of-function (EID1307)
       <https://civicdb.org/links/evidence/1307>`_
   * - N/A
     - `CD274 Expression (EID1167)
       <https://civicdb.org/links/evidence/1167>`_
