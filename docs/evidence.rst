.. _evidence:

The CIViC Evidence Item
=======================

.. image:: images/GP-113_CIViC_schema-collaboration_SCHEMA_v3a.png
   :align: right
   :scale: 50%

At the heart of CIViC is the clinical evidence statement. The clinical
evidence statement is a piece of information that has been manually curated
from trustable medical literature about a variant or genomic 'event' that has
implications in cancer predisposition, diagnosis (aka molecular
classification), prognosis, or predictive response to therapy. For example,
“Patients with BRAF V600 mutations respond well to the drug dabrafenib”. A
variant may be a single nucleotide substitution, a small insertion or
deletion, an RNA gene fusion, a chromosomal rearrangement, an RNA expression
pattern (e.g. over-expression), etc. Each clinical evidence statement
corresponds to a single citable publication. Ready to jump into the
literature? First you will need to login (or create an account if you don't
have one yet). Once you are logged in, you can check out our `ranked list of
high priority genes
<https://github.com/genome/civic-server/tree/master/public/downloads/RankedCivicGeneCandidates.tsv>`_
or visit the `Source Suggestion queue <https://civicdb.org/curation/sources>`_ for inspiration.

.. content-tabs::

  .. tab-container:: tab1
     :title: Overview

     The rows in the following table describe the minimal components of a
     CIViC Evidence Item. Several Evidence Statements are synthesized at the
     Variant level into Variant Summaries but each Evidence Statement is
     directly linked to a single article in PubMed. *More specific guidelines
     about Evidence Item components can be found in additional help tabs*.

     **General Guidelines**

     - Evidence Statements should be:

       - derived from primary literature sources (not review articles) whenever
         possible.
       - as concise as possible while providing sufficient experiemental detail to
         interpret and evaluate the evidence (N values, statistics, etc).
       - a single Predictive, Predisposing, Diagnostic or Prognostic assertion,
         not a combination.
       - aimed at a general audience, avoiding field-specific acronyms and
         colloquialisms.

     - Multiple, separate Evidence Items can be and often are derived from a
       single publication.
     - Generally, assertions involving drugs should be classified as being of
       the Predictive Evidence Type.
     - Star Ratings should be based on the strength of the specific assertion.
       Multiple assertions from the same publication can have different star
       ratings.

     **Evidence Attributes**

     .. list-table::
        :widths: 10 50 20 20
        :header-rows: 1

        * - Attribute
          - Description
          - Example
          - Source
        * - Gene
          - The symbol and ID of the gene implicated.
          - ESR1 (Entrez ID: 2099)
          - CIViC (Entrez)
        * - Variant
          - Genomic event/mutation (Single nucleotide variant,
            Insertion/deletion, Gene fusion, Copy number variant, etc.)
            implicated.
          - Y537S
          - CIViC
        * - Evidence Statement
          - Human readable interpretation. Free-form text
            summary of this event’s potential clinical interpretations. This
            interpretation is the synthesis of all other information about an
            event and its relevance to clinical action and should be the living
            product of active discussion.
          - This study of 178 non-small cell lung
            cancer patients, the appearance of T790M mutation lead to resistance
            to gefitinib.
          - CIViC
        * - Evidence Level
          - The type of experiment from which the evidence is
            curated. From inferential, to proven association in clinical
            medicine. Refer to the additional documentation on evidence levels
            for definitions of the five levels allowed in CIViC: validated,
            clinical, pre-clinical, case study, and inferential.
          - Level B - Clinical Evidence.
          - CIViC
        * - Evidence Type
          - Category of clinical action/relevance implicated by
            event. Refer to the additional documentation on evidence types for
            details on how to enter evidence of each of the four types:
            Predictive, Prognostic, Predisposing and Diagnostic. See 'Evidence
            Type' tab for more information.
          - Predictive - The variant is
            predictive of sensitivity or resistance to a therapeutic.
          - CIViC
        * - Evidence Direction
          - An indicator of whether the evidence statement
            supports or refutes the clinical significance of an event. See
            'Evidence Type' tab for more information.
          - Supports - the evidence supports the clinical significance.
          - CIViC
        * - Clinical Significance
          - The association with diagnostic/prognostic end
            point or treatment. See 'Evidence Type' tab for more information.
          - Resistant or Non-response - mutation is associated with resistance
            to therapy.
          - CIViC
        * - Variant Origin
          - Presumed cellular origin of the Variant in samples
            from the literature citation where the clinical effect of this
            Variant is being evaluated.
          - Somatic
          - CIViC
        * - Disease
          - Specific disease or disease subtype that is associated
            with this event and its clinical implication. Links directly to
            Disease Ontology.
          - Estrogen-receptor positive breast cancer (DOID: 0060075).
          - CIViC (Disease Ontology)
        * - Drug
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
        * - Trust Rating
          - A rating on a 5-star scale, portraying the curators
            trust in the experiments from which the evidence is curated. Refer
            to the additional documentation on trust ratings for guidance on how
            to score an evidence item.
          - 5-stars - Strong, well supported
            evidence from a lab or journal with respected academic standing.
            Experiments are well controlled, and results are clean and
            reproducible across multiple replicates.
          - CIViC

  .. tab-container:: tab2
     :title: Variant Origin

     The Variant Origin identifies whether the variant is presumed as an
     inherited (germline mutation) or acquired (somatic mutation) event in the
     context of the study. We generally consider somatic events to be the first
     priority, as this is an area that has not been as well addressed by existing
     resources. However, germline mutations with established clinical relevance
     are acceptable. Germline polymorphisms (>1% allele frequency in the
     population) are considered low priority, again unless there is an
     established clinical significance. Polymorphisms described in association
     studies should be curated with great caution and may face additional
     scrutiny from CIViC moderators. For some variant types, the variant origin
     field may be unknown or N/A. For example, EXPRESSION variants are neither
     germline nor somatic. Fusion variants are an unusual case in that they are
     often observed in the transcriptome but are usually accompanied by an
     underlying somatic (or germline) mutation. Most fusions should be entered as
     somatic. If in doubt, please note the issue at the time of your submission
     to encourage discussion during the moderation stage.

     **Variant Origin Guidelines**

     .. list-table::
        :widths: 10 70 20
        :header-rows: 1

        * - Variant Origin
          - Comments
          - Examples
        * - Somatic Mutation
          - Highest priority variants in CIViC.

            May include presumed somatic variants largely driven by the usage in
            the original publication but should be approached with caution in
            instances of tumor-only analysis.

            Includes fusions.
          - `DNAJB1-PRKACA (EID532)
            <https://civic.genome.wustl.edu/events/genes/17/summary/variants/31/summary/evidence/532/summary#evidence>`_

            `BRAF V600E (EID1409)
            <https://civic.genome.wustl.edu/events/genes/5/summary/variants/12/summary/evidence/1409/summary#evidence>`_

            `KRAS Exon 20 Mutation (EID993)
            <https://civic.genome.wustl.edu/events/genes/30/summary/variants/75/summary/evidence/993/summary#evidence>`_

            `EGFR Amplification (EID473)
            <https://civic.genome.wustl.edu/events/genes/19/summary/variants/190/summary/evidence/473/summary#evidence>`_
        * - Germline Mutation
          - Consist of heritable rare variants. Generally, <1% of the
            population relevant to the publication being cited.
          - `GSTP1 I105V (EID670)
            <https://civic.genome.wustl.edu/events/genes/2473/summary/variants/259/summary/evidence/670/summary#evidence>`_

            `BRCA2 Mutation (EID1371)
            <https://civic.genome.wustl.edu/events/genes/7/summary/variants/186/summary/evidence/1371/summary#evidence>`_
        * - Germline Polymorphism
          - Defined as variants with >1% allele frequency in the population
            relevant to the publication where the evidence is derived.

            Are welcome in CIViC, however, generally considered low priority for
            curation efforts.
          - `UGT1A1*28 (EID1792)
            <https://civic.genome.wustl.edu/events/genes/12422/summary/variants/729/summary/evidence/1792/summary#evidence>`_
        * - Unknown
          - May be used in instances where the publication is ambiguous about
            the origin of the variant although ordinarily an origin would be
            known (e.g., tumor-only analysis, analyses including both germline
            and somatic variants).
          - `FANCC Loss-of-function (EID1307)
            <https://civic.genome.wustl.edu/events/genes/1811/summary/variants/534/summary/evidence/1307/summary#evidence>`_
        * - N/A
          - For variants such as 'Expression' where a germline or somatic
            origin is not applicable.
          - `CD274 Expression (EID1167)
            <https://civic.genome.wustl.edu/events/genes/11335/summary/variants/276/summary/evidence/1167/summary#evidence>`_

  .. tab-container:: tab3
     :title: Evidence Types

     When curating evidence statements from published sources, to discern
     whether a variant has a "clinical interpretation", we use the data model
     below. Evidence statements describe how a variant was demonstrated to (1)
     be predictive of drug response, (2) be correlated with prognostic
     outcome, (3) be of diagnostic utility in determining cancer subtype (aka
     molecular classification), or (4) predispose a person to a type of
     cancer. If an evidence item can not be placed in one of these four
     categories (Predictive, Prognostic, Diagnostic, Predisposing), it likely
     lies outside of the scope of CIViC. However, published statements about a
     gene or variant that cannot be placed within these categories can still
     be added to the gene and variant summaries.

     .. raw:: html

        <table>
            <colgroup>
                <col width="150">
                <col width="250">
                <col width="400">
                <col width="920">
            </colgroup>
            <tbody>
                <tr>
                    <th>Evidence Type</th>
                    <th>Evidence Direction</th>
                    <th>Clinical Significance</th>
                    <th>Example</th>
                </tr>
                <tr>
                    <td rowspan="6">
                        <b>Predictive:</b>
                        <i>Evidence pertaining to a variant's effect on
                        therapeutic response </i>
                    </td>
                    <td rowspan="3">
                        "Supports:"
                        "The experiment or study supports this variant's
                        response to a drug"
                    </td>
                    <td>
                        "Sensitivity/Reponse:"
                        "Variant is associated with positive response to
                        treatment (e.g. sensitivity to drug)"
                    </td>
                    <td>
                        Breast cancer cell lines with a PIK3CA H1047R mutation
                        showed increased sensitivity to CH5132799 compared to
                        cells with wild-type PIK3CA gene.
                    </td>
                </tr>
                <tr>
                    <td>
                        N/A:
                        Variant does not inform clinical action
                    </td>
                    <td>
                        OSI-906, an IGF1R/INSR inhibitor, does not have a
                        significant effect on chemotherapy resistant
                        castration-resistant prostate cancer cell lines.
                    </td>
                </tr>
                <tr>
                    <td>
                        Resistance:
                        Variant is associated with negative treatment response
                        (e.g. resistance to drug)
                    </td>
                    <td>
                        In NSCLC, Exon 2 KRAS mutations were associated with
                        resistance to the EGFR kinase inhibitors gefitinib and
                        erlotinib.
                    </td>
                </tr>
                <tr>
                    <td rowspan="3">
                        Does not support:

                        The experiment or study does not support, or was
                        inconclusive of an interaction between the variant and
                        a drug
                    </td>
                    <td>
                        Sensitivity/Response:
                        Variant is associated with positive response to
                        treatment (e.g. sensitivity to drug)
                    </td>
                    <td>
                        BRAF V600E mutation does not predict response in
                        patients treated with dacarbazine or temozolomide.
                    </td>
                </tr>
                <tr>
                    <td>
                        N/A:
                        Variant does not inform clinical action
                    </td>
                    <td>
                        There is no statistical difference in progression free
                        survival between lung cancer patients with or without
                        an EGFR L858R mutation following treatment with
                        gefitinib or erlotinib.
                    </td>
                </tr>
                <tr>
                    <td>
                        Resistance:
                        Variant is associated with negative treatment response
                        (e.g. resistance to drug)
                    </td>
                    <td>
                        In the setting of BRAF(V600E), NF1 loss resulted in
                        elevated activation of RAS-GTP but does not show
                        resistance to MEK inhibitors.
                    </td>
                </tr>
                <tr>
                    <td rowspan="4">
                        Diagnostic:

                        Evidence pertaining to a variant’s impact on patient
                        diagnosis
                    </td>
                    <td rowspan="2">
                        Supports:

                        The experiment or study supports variant’s impact on
                        the diagnosis of disease or subtype
                    </td>
                    <td>
                        Positive:
                        Variant is associated with diagnosis of disease or
                        subtype
                    </td>
                    <td>
                        BRAF V600E is shown to be associated with the
                        tall-cell variant of papillary thyroid carcinoma
                        (PTC). Supports use to confirm a diagnosis.
                    </td>
                </tr>
                <tr>
                    <td>
                        Negative:
                        Variant is associated with the lack of diagnosis of
                        disease or subtype
                    </td>
                    <td>
                        JAK2 V617F is not associated with lymphoid leukemia
                        (B-lineage ALL, T-ALL or CLL). Supports use to exclude
                        a diagnosis.
                    </td>
                </tr>
                <tr>
                    <td rowspan="2">
                        Does not support:

                        The experiment or study does not support the variant’s
                        impact on diagnosis of disease or subtype
                    </td>
                    <td>
                        Positive:
                        Variant is associated with diagnosis of disease or
                        subtype
                    </td>
                    <td>
                        Frequency of NPM1 mutations was not different in
                        normal karyotype acute myeloid leukemia patients with
                        CEPBA, NRAS or KIT mutations. Does NOT support use to
                        confirm a diagnosis.
                    </td>
                </tr>
                <tr>
                    <td>
                        Negative:
                        Variant is associated with the lack of diagnosis of
                        disease or subtype
                    </td>
                    <td>
                        Study 1 found that, contrary to what was previously
                        believed, mutation X does NOT in fact exclude disease
                        subtype A. Does NOT support use to exclude a
                        diagnosis.
                    </td>
                </tr>
                <tr>
                    <td rowspan="6">
                        Prognostic:

                        Evidence pertaining to a variant’s impact on disease
                        progression, severity, or patient survival
                    </td>
                    <td rowspan="3">
                        Supports:

                        The experiment or study supports a variant’s impact on
                        prognostic outcome
                    </td>
                    <td>
                        Good Outcome:
                        Variant is associated with a better overall patient
                        outcome
                    </td>
                    <td>
                        In AML, patients with IDH2 R140K mutation have
                        improved overall survival compared to those with
                        wild-type IDH2.
                    </td>
                </tr>
                <tr>
                    <td>
                        N/A:
                        Variant does not inform clinical action
                    </td>
                    <td>
                        In renal clear cell carcinoma, patients with VHL
                        mutations did not have a significant impact on cancer
                        specific survival.
                    </td>
                </tr>
                <tr>
                    <td>
                        Poor Outcome:
                        Variant is associated with a worse overall patient
                        outcome
                    </td>
                    <td>
                        WT1 mutations were associated with shorter overall and
                        disease free survival in a cohort of cytogenetically
                        normal, young AML patients.
                    </td>
                </tr>
                <tr>
                    <td rowspan="3">
                        Does not support:

                        The experiment or study does not support a prognostic
                        association between variant and outcome
                    </td>
                    <td>
                        Good Outcome:
                        Variant is associated with a better overall patient
                        outcome
                    </td>
                    <td>
                        Mutation X was not shown to be associated with
                        improved overall survival.
                    </td>
                </tr>
                <tr>
                    <td>
                        N/A:
                        Variant does not inform clinical action
                    </td>
                    <td>
                        Size of the FLT3-ITD mutant duplication had no impact
                        on overall survival or relapse rate.
                    </td>
                </tr>
                <tr>
                    <td>
                        Poor Outcome:
                        Variant is associated with a worse overall patient
                        outcome
                    </td>
                    <td>
                        Unlike other studies that suggest a poorer outcome,
                        BRAF mutation in this study was not correlated with
                        poorer prognosis in papillary thyroid cancer.
                    </td>
                </tr>
                <tr>
                    <td rowspan="5">
                        Predisposing:

                        Evidence pertains to a variant's role in conferring
                        susceptibility to a disease
                    </td>
                    <td rowspan="5">
                        Supports:

                        The experiment or study supports a variant’s impact on
                        predisposition to a cancer
                    </td>
                    <td>
                        Pathogenic:
                        Very strong evidence the variant is pathogenic.
                    </td>
                    <td>
                        Refer to the <a
                        href="http://www.nature.com/gim/journal/v17/n5/pdf/gim201530a.pdf">ACMG Standards and Guidelines</a> for
                        details.
                    </td>
                </tr>
                <tr>
                    <td>
                        Likely Pathogenic:
                        Strong evidence (">90% certainty") the variant is
                        pathogenic.
                    </td>
                    <td>
                        Refer to the <a
                        href="http://www.nature.com/gim/journal/v17/n5/pdf/gim201530a.pdf">ACMG Standards and Guidelines</a> for
                        details.
                    </td>
                </tr>
                <tr>
                    <td>
                        Benign:
                        Very strong evidence the variant is benign.
                    </td>
                    <td>
                        Refer to the <a
                        href="http://www.nature.com/gim/journal/v17/n5/pdf/gim201530a.pdf">ACMG Standards and Guidelines</a> for
                        details.
                    </td>
                </tr>
                <tr>
                    <td>
                        Likely Benign:
                        Strong evidence (">90% certainty") the variant is
                        benign.
                    </td>
                    <td>
                        Refer to the <a
                        href="http://www.nature.com/gim/journal/v17/n5/pdf/gim201530a.pdf">ACMG Standards and Guidelines</a> for
                        details.
                    </td>
                </tr>
                <tr>
                    <td>
                        Uncertain Significance:
                        The variant does not fullfill the ACMG criteria for
                        pathogenic/benign, or the evidence is conflicting.
                    </td>
                    <td>
                        Refer to the <a
                        href="http://www.nature.com/gim/journal/v17/n5/pdf/gim201530a.pdf">ACMG Standards and Guidelines</a> for
                        details.
                    </td>
                </tr>
            </tbody>
        </table>

  .. tab-container:: tab4
     :title: Evidence Levels

     Each evidence statement is the result of an experiment, trial or study in
     published literature. It is important to capture the nature of these
     experiments in the evidence entry. Evidence levels allow for the subject
     of an evidence item to be presented in a simple, standardized fashion.
     The evidence level is also an indication of how close each assertion is
     to actual application in the clinic. Please, note that while evidence
     statements of all levels are acceptable in CIViC, by far the highest
     priority are levels A and B, followed by C, D, E. Our top priority is to
     document the evidence for application of variant interpretations to real
     patients in the clinic today. The more time and development needed to
     determine the relevance of a variant to real patients in the clinic, the
     lower the priority for curation. Reviewing and approving evidence items
     requires a serious time committment by the community. Please keep this in
     mind and try to direct your efforts to the most immediately clinically
     relevant evidence first.

     .. list-table::
        :widths: 10 20 70
        :header-rows: 1

        * - Level
          - Definition
          - Example and further comments
        * - A
            Validated association
          - Proven/consensus association in human medicine.
          - *"AML with mutated NPM1" is a provisional entity in WHO classification of acute
            myeloid leukemia (AML). This mutation should be tested for in
            clinical trials and is recommended for testing in patients with
            cytogenetically normal AML.* Validated associations are often in
            routine clinical practice already or are the subject of major
            clinical trial efforts.
        * - B
            Clinical evidence
          - Clinical trial or other primary patient data
            supports association.
          - *BRAF V600E is correlated with poor
            prognosis in papillary thyroid cancer in a study of 187 patients
            with PTC and other thyroid diseases.* The evidence should be
            supported by observations in multiple patients. Additional support
            from functional data is desirable but not required.
        * - C
            Case study
          - Individual case reports from clinical journals.
          - *A single patient with FLT3 over-expression responded to the FLT3
            inhibitor sunitinib.* The study may have involved a large number of
            patients, but the statement was supported by only a single
            patient. In some cases, observations from just a handful of
            patients (e.g. 2-3) or a single family may also be considered a
            case study/report.
        * - D
            Preclinical evidence
          - In vivo or in vitro models support association.
          - *Experiments showed that AG1296 is effective in
            triggering apoptosis in cells with the FLT3 internal tandem
            duplication.* The study may have involved some patient data, but
            support for this statement was limited to in vivo or in vitro
            models (e.g. mouse studies, cell lines, molecular assays, etc.).
        * - E
            Inferential association
          - Indirect evidence.
          - *CD33 and CD123 expression were significantly increased in patients with NPM1
            mutation with FLT3-ITD, indicating these patients may respond to
            combined anti-CD33 and anti-CD123 therapy.* The assertion is at
            least one step removed from a direct association between a variant
            and clinical relevance.

  .. tab-container:: tab5
     :title: Trust Ratings

     In order to quickly discern how much trust curators and users have in a
     single evidence statement, a five star trust rating system is used. Each
     evidence item is given a rating, from 1 to 5 stars, based on the quality
     of the evidence the statement summarizes. This rating depends on a number
     of factors, including journal impact, study size, quality control,
     orthogonal validation, and reproducibility. It should be noted that this
     rating is largely subjective and may be debated (hopefully within the
     CIViC interface). Also the rating should be specific to the evidence
     statement. The overall publication/study might be high quality in a high
     impact publication, but the evidence statement may refer to a single
     conclusion in the study, and that part of the study might not be well
     supported. For example, the assertion may relate to patients with a
     particular mutation, and the study might involve an impressive 500
     patients, but if only 2 patients have the mutation in question, the
     quality rating may be low for this evidence statement.

     .. list-table::
        :widths: 10 90
        :header-rows: 1

        * - Trust Rating
          - Definition
        * - .. raw:: html

               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
          - Strong, well supported evidence from a lab or journal with respected academic standing. Experiments are well controlled, and results are clean and reproducible across multiple replicates. Evidence confirmed using independent methods. The study is statistically well powered.
        * - .. raw:: html

               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
          - Strong, well supported evidence. Experiments are well controlled, and results are convincing. Any discrepancies from expected results are well-explained and not concerning.
        * - .. raw:: html

               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
          - Evidence is convincing, but not supported by a breadth of experiments. May be smaller scale projects, or novel results without many follow-up experiments. Discrepancies from expected results are explained and not concerning.
        * - .. raw:: html

               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
          - Evidence is not well supported by experimental data, and little follow-up data is available. Publication is from a journal with low academic impact. Experiments may lack proper controls, have small sample size, or are not statistically convincing.
        * - .. raw:: html

               <span class="glyphicon glyphicon-star"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
               <span class="glyphicon glyphicon-star-empty"></span>
          - Claim is not supported well by experimental evidence. Results are not reproducible, or have very small sample size. No follow-up is done to validate novel claims.
