.. _variant-types:

Types
=====
Variant Type(s) are used to classify variants by Sequence Ontology terms.

Variant Types permit advanced searching for categories of variants in the CIViC interface and downstream semantic analyses of CIViC variants. Some examples of variant types are listed below.

Curating Variant Types
---------------------------
The most specific term(s) that can be applied to a given variant should be utilized. Use of the `Sequence Ontology browser <http://www.sequenceontology.org/browser/obob.cgi>`__ is recommended to identify appropriate terms. 

When choosing variant types, selection of multiple terms is supported in order to capture both functional and structural effects of the variant. However, these terms should not be ancestors or descendents of one another, and all selected terms should be descendents of the ‘sequence_variant’ term whenever possible.

Variant Type Guidelines
~~~~~~~~~~~~~~~~~~~~~~~
- Choose the most specific terms.
- Do not use terms that are ancestors/decendants of each other.
- Wherever possible use the 'sequence_variant' tree of the sequence ontology.

Curation Guidelines for Specific Sequence Ontology Types
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. list-table::
   :widths: 15 40 30
   :header-rows: 1

   * - Sequence Ontology Term
     - Sequence Ontology Definition
     - Comments
   * - missense_variant
     - A sequence variant, that changes one or more bases, resulting in a different amino acid sequence but where the length is preserved.
     -
   * - stop_gained
     - A sequence variant whereby at least one base of a codon is changed, resulting in a premature stop codon, leading to a shortened polypeptide.
     - Also known as a nonsense variant.
   * - protein_altering_variant
     - A sequence_variant which is predicted to change the protein encoded in the coding sequence.
     -
   * - frameshift_truncation
     - A frameshift variant that causes the translational reading frame to be shortened relative to the reference feature.
     -
   * - inframe_deletion
     - An inframe non synonymous variant that deletes bases from the coding sequence.
     -
   * - inframe_insertion
     - An inframe non synonymous variant that inserts
       bases into in the coding sequence.
     -
   * - [ gene_variant

       OR

       transcript_variant ]

       AND

       [ loss_of_function_variant

       OR

       gain_of_function_variant ]
     - [ gene_variant: A sequence variant where the structure of the gene is
       changed.

       OR

       transcript_variant: A sequence variant that changes the structure of
       the transcript ]

       AND

       [ loss_of_function_variant: A sequence variant whereby the gene
       product has diminished or abolished function.

       OR

       gain_of_function_variant: A sequence variant whereby new or enhanced
       function is conferred on the gene product. ]
     - Depends on situation.
   * - exon_variant
     - A sequence variant that changes exon sequence.
     -
   * - transcript_fusion

       OR RARELY...

       gene_fusion
     - transcript_fusion: A feature fusion where the deletion brings together
       transcript regions.

       OR

       gene_fusion: A sequence variant whereby a two genes have become
       joined.
     - Depends on situation.

       Note that transcript_fusion mentions "deletion" specifically as the
       genomic alteration, and both gene_fusion and transcript_fusion are children
       of feature_fusion, which also mentions "deletion" specifically.
       However, it is assumed that deletion is just one possible mechanism
       (along with translocation, inversion, etc) for bringing two gene or
       transcribed regions together. The decision of which term to use
       therefore rests on the level of specificity. If the genomic event is
       thought to result in a fusion transcript then "transcript_fusion" is
       the preferred term.
   * - transcript_fusion

       AND

       missense_variant
     - transcript_fusion: A feature fusion where the deletion brings together
       transcript regions.

       AND

       missense_variant: A sequence variant that changes one or more bases,
       resulting in a different amino acid sequence but where the length is
       preserved.
     -
   * - transcript_translocation

       OR

       feature_translocation

       OR

       transcript_fusion
     - transcript_translocation: A feature translocation where the region
       contains a transcript.

       OR

       feature_translocation: A sequence variant, caused by an alteration of
       the genomic sequence, where the structural change, a translocation, is
       greater than the extent of the underlying genomic features.

       OR

       transcript_fusion: A feature fusion where the deletion brings together
       transcript regions.
     - Depends on situation.
   * - wild_type
     - An attribute describing sequence with the genotype found
       in nature and/or standard laboratory stock.
     -
   * - loss_of_heterozygosity
     - A functional variant whereby the sequence
       alteration causes a loss of function of one allele of a gene.
     -
   * - transcript_amplification
     - A feature amplification of a region
       containing a transcript.
     -
   * - transcript_ablation
     - A feature ablation whereby the deleted region
       includes a transcript feature.
     -
   * - copy_number_change
     - A sequence variant where copies of a feature (CNV)
       are either increased or decreased.
     -
   * - loss_of_function_variant
     - A sequence variant whereby the gene
       product has diminished or abolished function.
     -
   * - loss_of_function_variant...?

       transcript_ablation...?
     - loss_of_fuction_variant: A sequence variant whereby the gene product
       has diminished or abolished function.

       transcript_ablation: A feature ablation whereby the deleted region
       includes a transcript feature.
     - Depends on situation.
   * - exon_loss_variant
     - A sequence variant whereby an exon is lost from
       the transcript.
     -
   * - 5_prime_UTR_variant
     - A UTR variant of the 5' UTR.
     -
   * - 3_prime_UTR_variant
     - A UTR variant of the 3' UTR.
     -
   * - synonymous_variant
     - A sequence variant where there is no resulting change to the encoded amino acid.
     -
   * - N/A
     -
     - The Sequence Ontology does not currently describe expression
       or epigenetic variants.

Variant Type Examples
~~~~~~~~~~~~~~~~~~~~~

.. list-table::
   :widths: 20 80
   :header-rows: 1

   * - Sequence Ontology Term
     - Examples
   * - missense_variant
     - `G12D
       <https://civicdb.org/links/variant/79>`_
   * - stop_gained
     - `R130*
       <https://civicdb.org/links/variant/636>`_
   * - protein_altering_variant
     - `G12
       <https://civicdb.org/links/variant/76>`_

       `KINASE DOMAIN MUTATION
       <https://civicdb.org/links/variant/413>`_
   * - frameshift_truncation
     - `V2288fs*1
       <https://civicdb.org/links/variant/243>`_
   * - inframe_deletion
     - `DEL I843
       <https://civicdb.org/links/variant/101>`_

       `V560DEL
       <https://civicdb.org/links/variant/202>`_

       `DEL 755-759
       <https://civicdb.org/links/variant/37>`_
   * - inframe_insertion
     - `P780INS
       <https://civicdb.org/links/variant/41>`_

       `M774INSAYVM
       <https://civicdb.org/links/variant/414>`_

       `ITD
       <https://civicdb.org/links/variant/55>`_
   * - [ gene_variant

       OR

       transcript_variant ]

       AND

       [ loss_of_function_variant

       OR

       gain_of_function_variant ]
     - `MUTATION
       <https://civicdb.org/links/variant/399>`_
   * - exon_variant
     - `EXON 10 MUTATION
       <https://civicdb.org/links/variant/106>`_
   * - transcript_fusion

       OR RARELY...

       gene_fusion
     - `EML4-ALK
       <https://civicdb.org/links/variant/5>`_

       `ALK FUSIONS
       <https://civicdb.org/links/variant/499>`_
   * - transcript_fusion

       AND

       missense_variant
     - `EML4-ALK G1269A
       <https://civicdb.org/links/variant/308>`_
   * - transcript_translocation

       OR

       feature_translocation

       OR

       transcript_fusion
     - `REARRANGEMENT
       <https://civicdb.org/links/variant/269>`_
   * - wild_type
     - `WILD TYPE
       <https://civicdb.org/links/variant/426>`_
   * - loss_of_heterozygosity
     - `LOH
       <https://civicdb.org/links/variant/302>`_
   * - transcript_amplification
     - `AMPLIFICATION
       <https://civicdb.org/links/variant/18>`_
   * - transcript_ablation
     - `DELETION
       <https://civicdb.org/links/variant/200>`_
   * - copy_number_change
     - `COPY NUMBER VARIATION
       <https://civicdb.org/links/variant/191>`_
   * - loss_of_function_variant
     - `LOSS-OF-FUNCTION
       <https://civicdb.org/links/variant/125>`_
   * - loss_of_function_variant...?

       transcript_ablation...?
     - `LOSS
       <https://civicdb.org/links/variant/555>`_
   * - exon_loss_variant
     - `EXON 14 SKIPPING MUTATION
       <https://civicdb.org/links/variant/324>`_
   * - 5_prime_UTR_variant
     - `5' UTR MUTATION
       <https://civicdb.org/links/variant/255>`_
   * - 3_prime_UTR_variant
     - `3' UTR MUTATION
       <https://civicdb.org/links/variant/256>`_
   * - N/A
     - `EXPRESSION
       <https://civicdb.org/links/variant/19>`_

       `NUCLEAR EXPRESSION
       <https://civicdb.org/links/variant/340>`_

       `CYTOPLASMIC EXPRESSION
       <https://civicdb.org/links/variant/447>`_

       `OVEREXPRESSION
       <https://civicdb.org/links/variant/20>`_

       `UNDEREXPRESSION
       <https://civicdb.org/links/variant/179>`_

       `METHYLATION
       <https://civicdb.org/links/variant/538>`_

       `PROMOTER METHYLATION
       <https://civicdb.org/links/variant/85>`_

       `PROMOTER HYPERMETHYLATION
       <https://civicdb.org/links/variant/27>`_
