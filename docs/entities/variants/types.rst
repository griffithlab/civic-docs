Types
=====

Understanding Variant Types
---------------------------
Nullam eu ante vel est convallis dignissim.  Fusce suscipit, wisi nec facilisis facilisis, est dui fermentum leo, quis tempor ligula erat quis odio.  Nunc porta vulputate tellus.  Nunc rutrum turpis sed pede.  Sed bibendum.  Aliquam posuere.  Nunc aliquet, augue nec adipiscing interdum, lacus tellus malesuada massa, quis varius mi purus non odio.  Pellentesque condimentum, magna ut suscipit hendrerit, ipsum augue ornare nulla, non luctus diam neque sit amet urna.  Curabitur vulputate vestibulum lorem.  Fusce sagittis, libero non molestie mollis, magna orci ultrices dolor, at vulputate neque nulla lacinia eros.  Sed id ligula quis est convallis tempor.  Curabitur lacinia pulvinar nibh.  Nam a sapien.

Curating Variant Types
---------------------------
Variant types are used to classify variants within the structured ontology terms provided by The Sequence Ontology Project. Multiple terms for a variant are allowed to facilitate functional and structural effects of the variant. Ideally, the most specific child terms of a branch are used. These variant types can be used to search for variants within the CIViC database that meet a users' criteria via the advanced search page or through the API.

.. rubric:: General Guidelines

1) Choose the most specific terms.
2) Do not use terms that are ancestors/decendants of each other.
3) Wherever possible use the 'sequence_variant' tree of the sequence ontology.

.. rubric:: Variant Type Guidelines

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
   * - N/A
     -
     - The Sequence Ontology does not currently describe expression
       or epigenetic variants.

.. rubric:: Variant Type Examples

.. list-table::
   :widths: 20 80
   :header-rows: 1

   * - Sequence Ontology Term
     - Examples
   * - missense_variant
     - `G12D
       <https://civic.genome.wustl.edu/events/genes/30/summary/variants/79/summary>`_
   * - stop_gained
     - `R130*
       <https://civic.genome.wustl.edu/#/events/genes/41/summary/variants/636/summary>`_
   * - protein_altering_variant
     - `G12
       <https://civic.genome.wustl.edu/events/genes/30/summary/variants/76/summary#variant>`_

       `KINASE DOMAIN MUTATION
       <https://civic.genome.wustl.edu/events/genes/20/summary/variants/413/summary>`_
   * - frameshift_truncation
     - `V2288fs*1
       <https://civic.genome.wustl.edu/events/genes/69/summary/variants/243/summary>`_
   * - inframe_deletion
     - `DEL I843
       <https://civic.genome.wustl.edu/events/genes/38/summary/variants/101/summary>`_

       `V560DEL
       <https://civic.genome.wustl.edu/events/genes/29/summary/variants/202/summary>`_

       `DEL 755-759
       <https://civic.genome.wustl.edu/events/genes/20/summary/variants/37/summary>`_
   * - inframe_insertion
     - `P780INS
       <https://civic.genome.wustl.edu/events/genes/20/summary/variants/41/summary>`_

       `M774INSAYVM
       <https://civic.genome.wustl.edu/events/genes/20/summary/variants/414/summary>`_

       `ITD
       <https://civic.genome.wustl.edu/events/genes/24/summary/variants/55/summary>`_
   * - [ gene_variant

       OR

       transcript_variant ]

       AND

       [ loss_of_function_variant

       OR

       gain_of_function_variant ]
     - `MUTATION
       <https://civic.genome.wustl.edu/events/genes/5/summary/variants/399/summary>`_
   * - exon_variant
     - `EXON 10 MUTATION
       <https://civic.genome.wustl.edu/events/genes/37/summary/variants/106/summary>`_
   * - transcript_fusion

       OR RARELY...

       gene_fusion
     - `EML4-ALK
       <https://civic.genome.wustl.edu/events/genes/1/summary/variants/5/summary>`_

       `ALK FUSIONS
       <https://civic.genome.wustl.edu/events/genes/1/summary/variants/499/summary>`_
   * - transcript_fusion

       AND

       missense_variant
     - `EML4-ALK G1269A
       <https://civic.genome.wustl.edu/events/genes/1/summary/variants/308/summary#variant>`_
   * - transcript_translocation

       OR

       feature_translocation

       OR

       transcript_fusion
     - `REARRANGEMENT
       <https://civic.genome.wustl.edu/events/genes/4941/summary/variants/269/summary>`_
   * - wild_type
     - `WILD TYPE
       <https://civic.genome.wustl.edu/events/genes/5/summary/variants/426/summary>`_
   * - loss_of_heterozygosity
     - `LOH
       <https://civic.genome.wustl.edu/events/genes/4645/summary/variants/302/summary>`_
   * - transcript_amplification
     - `AMPLIFICATION
       <https://civic.genome.wustl.edu/events/genes/8/summary/variants/18/summary>`_
   * - transcript_ablation
     - `DELETION
       <https://civic.genome.wustl.edu/events/genes/73/summary/variants/200/summary>`_
   * - copy_number_change
     - `COPY NUMBER VARIATION
       <https://civic.genome.wustl.edu/events/genes/19/summary/variants/191/summary>`_
   * - loss_of_function_variant
     - `LOSS-OF-FUNCTION
       <https://civic.genome.wustl.edu/events/genes/46/summary/variants/125/summary>`_
   * - loss_of_function_variant...?

       transcript_ablation...?
     - `LOSS
       <https://civic.genome.wustl.edu/events/genes/916/summary/variants/555/summary#variant>`_
   * - exon_loss_variant
     - `EXON 14 SKIPPING MUTATION
       <https://civic.genome.wustl.edu/events/genes/52/summary/variants/324/summary>`_
   * - 5_prime_UTR_variant
     - `5' UTR MUTATION
       <https://civic.genome.wustl.edu/events/genes/1741/summary/variants/255/summary>`_
   * - 3_prime_UTR_variant
     - `3' UTR MUTATION
       <https://civic.genome.wustl.edu/events/genes/29/summary/variants/256/summary>`_
   * - N/A
     - `EXPRESSION
       <https://civic.genome.wustl.edu/events/genes/8/summary/variants/19/summary>`_

       `NUCLEAR EXPRESSION
       <https://civic.genome.wustl.edu/events/genes/9171/summary/variants/340/summary>`_

       `CYTOPLASMIC EXPRESSION
       <https://civic.genome.wustl.edu/events/genes/1883/summary/variants/447/summary>`_

       `OVEREXPRESSION
       <https://civic.genome.wustl.edu/events/genes/8/summary/variants/20/summary>`_

       `UNDEREXPRESSION
       <https://civic.genome.wustl.edu/events/genes/69/summary/variants/179/summary>`_

       `METHYLATION
       <https://civic.genome.wustl.edu/events/genes/3532/summary/variants/538/summary#variant>`_

       `PROMOTER METHYLATION
       <https://civic.genome.wustl.edu/events/genes/34/summary/variants/85/summary>`_

       `PROMOTER HYPERMETHYLATION
       <https://civic.genome.wustl.edu/events/genes/14/summary/variants/27/summary>`_
