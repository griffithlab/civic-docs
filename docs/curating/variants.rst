Curating Variants
=================

A CIViC Variant represents any molecular alteration with evidence for clinical relevance in cancer. CIViC Molecular Profiles (MPs) are comprised of one or more CIViC Feature-Variant pairs. Simple MPs are comprised of one Feature-Variant, and complex MPs are comprised of combinations of two or more Feature-Variants. A new Variant is added to the CIViC database during Evidence Item creation. For a simple MP, when the first Evidence Item containing clinically relevant information for a new variant describing a biomarker is submitted, then that CIViC Variant is added to the database. Variants can also be added to the database during the creation of complex Molecular Profiles. When a complex MP contains a Variant not yet in CIViC, then when the first Evidence Item is curated for this MP, new Variants will be added to the database during the curation process.  

Once a Variant exists in the database, then Variant coordinates and other Variant-level data can also be curated in the user interface. The CIViC definition of a Variant is intentionally broad to encompass not only simple Variation. For Genes, Variants can capture a range of specific information (e.g., SNVs and indels), but also regional/categorical variation (e.g., exon mutation), or other types of variation (e.g., expression, fusions). Other Feature types all have related Variants. 

Curated fields within the Variant knowledge model for Genes include: Aliases, HGVS expressions, ClinVar IDs, Variant Type, representative Variant Coordinates and Transcript. 

Additional instruction on curating individual components of variants are provided in the :ref:`Knowledge Model docs for Variants<variants>`.
