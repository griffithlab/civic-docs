.. _variants:

Variants
========

Variants are a user-defined genomic alteration related to a specific clinical
outcome. New Variants are created by the addition of a new Evidence Item
associated with the Variant.

.. content-tabs::

  .. tab-container:: tab1
     :title: Overview

     CIViC variants are usually genomic alterations, including single
     nucleotide variants (SNVs), insertion/deletion events (indels), copy
     number alterations (CNV's such as amplification or deletion), structural
     variants (SVs such as translocations and inversions), and other events
     that differ from the "normal" genome. In some cases a CIViC variant may
     represent events of the transcriptome or proteome. For example,
     'expression' or 'over-expression' is a valid variant. Regardless of the
     variant, it must have an Predictive, Prognostic, Predisposing or
     Diagnostic clinical relevance to be entered in CIViC. New curators should
     generally avoid proposing new variants that are unlike any already in
     CIViC.

     **Variant Attributes**

     .. list-table::
        :widths: 20 70 10
        :header-rows: 1

        * - Attribute
          - Description
          - Source
        * - Name
          - Description of the type of variant (e.g., 'V600E', 'BCR-ABL
            fusion', 'Loss-of-function', 'Exon 12 mutations'). Should be as
            specific and short as possible (i.e., specific amino acid changes).
          - CIViC
        * - Summary
          - User-defined summary of the clinical relevance of this
            Variant.
          - CIViC
        * - Alias
          - Alternative names for this Variant. May be more verbose (e.g.,
            'Val600Glu') versions, dbSNP IDs or alternative nomenclature used in
            the literature.
          - CIViC
        * - HGVS Expression
          - User-defined HGVS strings following HGVS
            nomenclature that represent this Variant at the DNA, RNA or protein
            level.
          - CIViC
        * - ClinVar ID
          - User-defined ClinVar ID referencing this Variant which
            will be linked directly to ClinVar. A value of "None Specified"
            indicates that the variant has not been evaluated for a ClinVar ID.
            A value of "None Found" indicates that an attempt was made to find a
            matching ClinVar Entry, but none exists. A value of "N/A" indicates
            that a ClinVar record is not applicable to the variant (e.g.
            "Overexpression" variants).
          - CIViC (ClinVar)
        * - Sources
          - A list of PubMed IDs referring to evidence supporting
            statements made in the Gene's description. Source descriptions (e.g.
            'Weisberg et al., 2007, Nat. Rev. Cancer') are pulled from the
            PubMed database at the time of submission, and are not editable.
          - CIViC (PubMed)
        * - CIViC Actionability Score
          - The CIViC Actionability Score assesses the
            quality and quantity of evidence submitted for each variant. The
            CIViC Actionability Score is calculated by adding all Evidence Item
            Scores for each variant. The Evidence Item Score is calculated by
            multiplying the evidence level (A=10 points, B=5 points, C=3 points,
            D=1 point, E=0.25 points) by the trust rating (Each Star = 1 point).
          - CIViC
        * - Variant Type(s)
          - One or more terms from the Sequence Ontology that
            describes the type of variant. Should be the most descriptive term
            applicable on a given branch (e.g., 'Conservative Missense Variant',
            'Stop Gained', 'Transcript Fusion').
          - CIViC (Sequence Ontology)
        * - **Primary Coordinates**
          -
          -
        * - Reference Build
          - NCBI or GRC human reference assembly version.
          - CIViC
        * - Chromosome
          - Name of the chromosome in which the variant occurs.
          - CIViC
        * - Start, Stop
          - Start and stop positions of the variant (1-based
            genome coordinate). Start must be less than or equal to stop.
          - CIViC
        * - Reference & Variant Bases
          - The nucleotide base of the reference and variant
            allele (e.g. 'C', 'A').
          - CIViC
        * - Representative Transcript
          - Ensembl transcript ID and version number
            for a known transcript of the gene that contains the variant (e.g.
            'ENST00000263967.3').
          - CIViC
        * - **Secondary Coordinates**
          -
          -
        * - Same as Primary
          - For fusion variants, the secondary coordinates are
            used to specify the 3' partner of the fusion gene.
          - CIViC
        * - **MyVariant.Info**
          -
          -
        * - MyVariant Info
          - Data retrieved from MyVariant.Info using the
            curated Primary Coordinates (chromosome, start, stop, reference
            base, variant base) described above as the query. Includes external
            IDs and links whenever possible with additional data displayed by
            clicking the "Details" button.
          - MyVariant.Info

  .. tab-container:: tab2
     :title: Variant Name

     **General Guidelines**

     - New Variant Names should be unique within the gene of interest.
       Otherwise, an Evidence Item should be assigned to the existing Variant
       for that gene. Before proposing a new variant, please check existing
       variants to prevent redundancy. For example, 'deletion' and 'loss'.
     - The Variant Name should be the most specific possible given the
       literature citation (i.e., V600E over V600). In general the convention is
       to use the protein representation where possible (instead of the cDNA or
       genome representation).
     - The Variant Name may:

       - be a specific animo acid change (e.g., V600E or W288fs).
       - encompass more than 1 type of genomic change (e.g., Exon 12 Mutations or
         Frameshift Truncation).
       - share the same name as a variant in another gene (e.g., G12D is a Variant
         Name for both KRAS and NRAS).

     - For fusions:

       - The Variant Name is always 5' partner - 3' partner.
       - The fusion variant is entered under only one gene. Choose the 'important'
         gene. Often, but not always, this is the 3' gene. (e.g., the BCR-ABL
         Variant is associated with ABL1 Gene)

  .. tab-container:: tab3
     :title: Variant Summary

     The Variant Summary is a user-defined description of the clinical
     relevance of this Variant. This description should discuss the Variant’s
     relevance to different cancer types, patient outcomes and treatment
     decisions. It can be thought of as an executive summary of what
     information a clinician would like to know about a Variant identified in
     a patient tumor.

     The Summary is mostly a synthesis of the Evidence Statements available
     for the Variant. Although individual Evidence Statements do not capture
     biological/mechanistic impact of Variants on gene function, such
     information can be summarized briefly here. Since the Summary is a
     synthesis of Evidence Statements in CIViC, we recommend that a Variant
     Summary only be created after the number of Evidence Statements created
     for a Variant are a reasonable reflection of the state of the literature.
     As a simple rule of thumb, if a variant has less than 5-10 evidence
     statements (or higher for some variants), the Variant is probably NOT
     ready for a Variant Summary yet.

     **Aliases**

     Variant Aliases are used to describe alternative names for a variant.
     Variants may be known by more colloquial terms, amino acid positions that
     reference transcripts of a different length, alternative IDs, etc which
     can be captured here. For example, `MTHFR A222V
     <https://civic.genome.wustl.edu/events/genes/3672/summary/variants/258/summary#variant>`_ is also known as
     rs1801133, C677T, and Ala222Val.

     **HGVS Expression**

     Multiple valid HGVS strings following HGVS nomenclature (see `HGVS
     guidelines <http://varnomen.hgvs.org/>`_) can be entered here to represent a variant at different
     levels (DNA/RNA/protein).

     **ClinVar IDs**

     Curators can associate multiple valid ClinVar IDs with a variant which
     will link directly to that ClinVar entity, allowing manual associations
     not easily resolved by programmatic methods. For more general variants,
     more than one ClinVar ID may be appropriate. Enter N/A for variants that
     aren’t expected to have a ClinVar record (e.g., Expression). Enter NONE
     FOUND to indicate a search was completed and no ClinVar record was found.
     This allows for the possibility of future searches and updates later.

     **Sources**

     Although in-line citations are not currently supported, the addition of
     citations used to generate the Variant Summary beyond those captured in
     the Evidence Statements, particularly relevant reviews, is highly
     encouraged with the intention of directing other users to more in-depth
     information about the Variant. This can be accomplished using the Sources
     field and entered by specifying the PubMed ID associated with the
     publication.

     See `EGFR T790M <https://civic.genome.wustl.edu/events/genes/19/summary/variants/34/summary#variant>`_ for examples of all of the above fields.

  .. tab-container:: tab4
     :title: CIViC Actionability Score

     The CIViC Actionability Score allows curators to assess the accumulation
     of evidence for each variant. The CIViC Actionability Score is calculated
     by adding all Evidence Item Scores for each variant. The Evidence Item
     Score is calculated by multiplying the evidence level (A=10 points, B=5
     points, C=3 points, D=1 point, E=0.25 points) by the trust rating (Each
     Star = 1 point).

     **Example of how to calculate the CIViC Actionability Score**

     Example of CIViC score determination for each DNA-based variant using the
     CIViC entry for EID497. Catagorization of the ‘Evidence Level’ and the
     ‘Trust Rating’ creates a method for scoring each evidence item, which can
     be summed to create a variant score. Variant scores were used to
     determine panel eligibility.

     .. image:: images/actionability_score_example.png

  .. tab-container:: tab5
     :title: Variant Type

     Variant types are used to classify variants within the structured
     ontology terms provided by The Sequence Ontology Project. Multiple terms
     for a variant are allowed to facilitate functional and structural effects
     of the variant. Ideally, the most specific child terms of a branch are
     used. These variant types can be used to search for variants within the
     CIViC database that meet a users' criteria via the advanced search page
     or through the API.

     **General Guidelines**

     1) Choose the most specific terms.
     2) Do not use terms that are ancestors/decendants of each other.
     3) Wherever possible use the 'sequence_variant' tree of the sequence
        ontology.

     **Variant Type Guidelines**

     .. list-table::
        :widths: 15 40 30 15
        :header-rows: 1

        * - Sequence Ontology Term
          - Sequence Ontology Definition
          - Comments
          - Examples
        * - missense_variant
          - A sequence variant, that changes one or more
            bases, resulting in a different amino acid sequence but where the
            length is preserved.
          -
          - `G12D
            <https://civic.genome.wustl.edu/events/genes/30/summary/variants/79/summary>`_
        * - stop_gained
          - A sequence variant whereby at least one base of a
            codon is changed, resulting in a premature stop codon, leading to a
            shortened polypeptide.
          - Also known as a nonsense variant.
          - `R130*
            <https://civic.genome.wustl.edu/#/events/genes/41/summary/variants/636/summary>`_
        * - protein_altering_variant
          - A sequence_variant which is predicted to
            change the protein encoded in the coding sequence.
          -
          - `G12
            <https://civic.genome.wustl.edu/events/genes/30/summary/variants/76/summary#variant>`_

            `KINASE DOMAIN MUTATION
            <https://civic.genome.wustl.edu/events/genes/20/summary/variants/413/summary>`_
        * - frameshift_truncation
          - A frameshift variant that causes the
            translational reading frame to be shortened relative to the reference
            feature.
          -
          - `V2288fs*1
            <https://civic.genome.wustl.edu/events/genes/69/summary/variants/243/summary>`_
        * - inframe_deletion
          - An inframe non synonymous variant that deletes
            bases from the coding sequence.
          -
          - `DEL I843
            <https://civic.genome.wustl.edu/events/genes/38/summary/variants/101/summary>`_

            `V560DEL
            <https://civic.genome.wustl.edu/events/genes/29/summary/variants/202/summary>`_

            `DEL 755-759
            <https://civic.genome.wustl.edu/events/genes/20/summary/variants/37/summary>`_
        * - inframe_insertion
          - An inframe non synonymous variant that inserts
            bases into in the coding sequence.
          -
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
          - `MUTATION
            <https://civic.genome.wustl.edu/events/genes/5/summary/variants/399/summary>`_
        * - exon_variant
          - A sequence variant that changes exon sequence.
          -
          - `EXON 10 MUTATION
            <https://civic.genome.wustl.edu/events/genes/37/summary/variants/106/summary>`_
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
          - `EML4-ALK
            <https://civic.genome.wustl.edu/events/genes/1/summary/variants/5/summary>`_

            `ALK FUSIONS
            <https://civic.genome.wustl.edu/events/genes/1/summary/variants/499/summary>`_
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
          - `EML4-ALK G1269A
            <https://civic.genome.wustl.edu/events/genes/1/summary/variants/308/summary#variant>`_
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
          - `REARRANGEMENT
            <https://civic.genome.wustl.edu/events/genes/4941/summary/variants/269/summary>`_
        * - wild_type
          - An attribute describing sequence with the genotype found
            in nature and/or standard laboratory stock.
          -
          - `WILD TYPE
            <https://civic.genome.wustl.edu/events/genes/5/summary/variants/426/summary>`_
        * - loss_of_heterozygosity
          - A functional variant whereby the sequence
            alteration causes a loss of function of one allele of a gene.
          -
          - `LOH
            <https://civic.genome.wustl.edu/events/genes/4645/summary/variants/302/summary>`_
        * - transcript_amplification
          - A feature amplification of a region
            containing a transcript.
          -
          - `AMPLIFICATION
            <https://civic.genome.wustl.edu/events/genes/8/summary/variants/18/summary>`_
        * - transcript_ablation
          - A feature ablation whereby the deleted region
            includes a transcript feature.
          -
          - `DELETION
            <https://civic.genome.wustl.edu/events/genes/73/summary/variants/200/summary>`_
        * - copy_number_change
          - A sequence variant where copies of a feature (CNV)
            are either increased or decreased.
          -
          - `COPY NUMBER VARIATION
            <https://civic.genome.wustl.edu/events/genes/19/summary/variants/191/summary>`_
        * - loss_of_function_variant
          - A sequence variant whereby the gene
            product has diminished or abolished function.
          -
          - `LOSS-OF-FUNCTION
            <https://civic.genome.wustl.edu/events/genes/46/summary/variants/125/summary>`_
        * - loss_of_function_variant...?

            transcript_ablation...?
          - loss_of_fuction_variant: A sequence variant whereby the gene product
            has diminished or abolished function.

            transcript_ablation: A feature ablation whereby the deleted region
            includes a transcript feature.
          - Depends on situation.
          - `LOSS
            <https://civic.genome.wustl.edu/events/genes/916/summary/variants/555/summary#variant>`_
        * - exon_loss_variant
          - A sequence variant whereby an exon is lost from
            the transcript.
          -
          - `EXON 14 SKIPPING MUTATION
            <https://civic.genome.wustl.edu/events/genes/52/summary/variants/324/summary>`_
        * - 5_prime_UTR_variant
          - A UTR variant of the 5' UTR.
          -
          - `5' UTR MUTATION
            <https://civic.genome.wustl.edu/events/genes/1741/summary/variants/255/summary>`_
        * - 3_prime_UTR_variant
          - A UTR variant of the 3' UTR.
          -
          - `3' UTR MUTATION
            <https://civic.genome.wustl.edu/events/genes/29/summary/variants/256/summary>`_
        * - N/A
          -
          - The Sequence Ontology does not currently describe expression
            or epigenetic variants.
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

  .. tab-container:: tab6
     :title: Variant Coordinates

     Genomic coordinates in CIViC are a single representation of a genomic
     alteration that can lead to a specific variant. Multiple genomic
     alterations may lead to the same variant (i.e., several changes at the
     basepair level can lead to the same amino acid change); however, CIViC
     currently provides only one possible example per variant.

     **General Guidelines**

     - Choose one representative variant per gene.
     - Coordinates are 1-based.
     - Currently we prefer variants from reference genome build 37.
     - Representative transcripts are from Ensembl.

       - Include Ensembl transcript ID and transcript version (e.g.,
         'ENST00000078429.1') and the Ensembl database version (e.g., 75). Refer
         to further documentation below for guidance on how to select a
         representative transcript.

     - The start is always the numerically smaller coordinate.
     - Complexities can be documented in the variant comments section.
     - For fusions:

       - The fusion variant is entered under only one gene. Choose the 'important'
         gene. Often, but not always, this is the 3' gene.
       - The variant name is always 5' partner - 3' partner (e.g. BCR-ABL1,
         EML4-ALK, etc.)

     **Selecting a representative transcript**

     A representative transcript is a single transcript model used as an
     example or reference point. It is also used to define the genomic
     coordinates for the variant. We present a single representative
     transcript that contains the variant of interest that ideally can be
     exported using the API and converted bioinformatically to desired
     outputs.

     Features of a representative transcript:

     - There is no one 'right' answer for representative transcript.
     - It must:

       - contain the variant (except in rare cases like promoter mutations).

     - It should:

       - be from Ensembl archived version 75 including the transcript version
         number (i.e., ENST00000078429.1 instead of ENST00000078429).
       - be a transcript that is in our IGV reference transcript file. (see below)

     - It may:

       - be the transcript with the longest ORF or most exons.
       - be the transcript that contains the 'canonical exons’ that are used in
         many transcripts.
       - be the variant that has the greatest outer coordinates.
       - be the transcript that is widely used in literature.
       - be a transcript that is compatible with interpretation/visualization in
         the literature (source paper for evidence statements).

     IGV reference transcript file

     - This file is a custom gene track file that can be loaded in IGV for
       review of coordinates.
     - It is based on a specific version of Ensembl (v75) and contains both
       transcript IDs and transcript version numbers.
     - Ensembl defined ’canonical transcripts' are highlighted with asterisks
       (***ENST00000078429.1.v75***) as a suggestion when no specific transcript
       is otherwise indicated.
     - The reference transcript file can be obtained from the civic-server git
       repository here:
       Ensembl-v75_build37-hg19_UcscGenePred_CIViC-Genes.ensGene

     **Selecting variant coordinates based on variant type**

     Start and stop positions are dependent upon the reference genome and the
     specific isoform/transcript being used.

     .. list-table::
        :widths: 50 50

        * - **Single Nucleotide Variants (SNVs)**
          -
        * - .. image:: images/ChoosingCoordinates_SNVs.png
               :scale: 50%
          -  - Start and stop coordinates are the same
             - Secondary coordinates do not apply
        * - **Insertions**
          -
        * - .. image:: images/ChoosingCoordinates_Insertions.png
               :scale: 50%
          - - Secondary coordinates do not apply
        * - **Deletions**
          -
        * - .. image:: images/ChoosingCoordinates_Deletions.png
               :scale: 50%
          - - Secondary coordinates do not apply
        * - **Fusions**
          -
        * - .. image:: images/ChoosingCoordinates_Fusions.png
               :scale: 50%
          - - Secondary coordinates correspond to the 3' partner
            - Stop1 and Start2 coordinates correspond to the edge of the nearest exon
        * - **Whole Gene alterations (altered expression, deletion, amplification)**
          -
        * - .. image:: images/ChoosingCoordinates_Whole_Gene.png
               :scale: 50%
          - - Secondary coordinates do not apply
            - Variant coordinates include UTRs
        * - **Gene Segments ('hotspot' regions including exons or domains)**
          -
        * - .. image:: images/ChoosingCoordinates_Gene_Segment.png
               :scale: 50%
          - - Secondary coordinates do not apply
