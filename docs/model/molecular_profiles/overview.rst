Molecular Profiles Overview
=================

CIViC Molecular Profiles combinations of one or more CIViC variants. Most Molecular Profiles are "Simple" Molecular Profiles comprised of a single variant. In most cases, these can be considered equivalent to the CIViC concept of a :doc:`Variant <../variants/overview>`. However, increasingly clinical significance must be considered in the context of multiple variants simultaneously. Complex Molecular Profiles in CIViC allow for curation for such variant combinations. Regardless of the nature of the Molecular Profile (Simple or Complex), it must have a Predictive, Prognostic, Predisposing, Diagnostic, Oncogenic, or Functional clinical relevance to be entered in CIViC.

**Molecular Profile Attributes**

.. list-table::
   :widths: 20 70 10
   :header-rows: 1

   * - Attribute
     - Description
     - Source
   * - Name
     - Name of the molecular profile. This is assembled automatically from the component gene/variant parts.
     - CIViC
   * - Description
     - User-defined description of the clinical relevance of this molecular profile.
     - CIViC
   * - Alias
     - Alternative names for this Molecular Profile
     - CIViC
   * - Sources
     - A list of PubMed IDs referring to evidence supporting
       statements made in the Molecular Profile description. Source descriptions (e.g.
       'Weisberg et al., 2007, Nat. Rev. Cancer') are pulled from the
       PubMed database at the time of submission, and are not editable.
     - CIViC (PubMed)
   * - CIViC Actionability Score
     - The CIViC Actionability Score assesses the quality and quantity of evidence submitted for each molecular profile. The
       CIViC Actionability Score is calculated by adding all Evidence Item
       Scores for each variant. The Evidence Item Score is calculated by
       multiplying the evidence level (A=10 points, B=5 points, C=3 points,
       D=1 point, E=0.25 points) by the evidence rating (Each Star = 1 point).
     - CIViC
