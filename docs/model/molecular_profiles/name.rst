.. _molecular-profile-name:

Name
====
The **Molecular Profile Name** describes the specific molecular profile being interpreted for clinical utility. Selecting a Molecular Profile Name in the Molecular Profile list for a Gene will bring up a Molecular Profile specific page with a description, aliases, molecular profile score, details of underlying variant(s) and associated Evidence Items. 
 

Understanding Molecular Profile Names
-------------------------------------
The Molecular Profile Name concisely describes the gene/variant components (and their relationships) which define the molecular profile. The Molecular Profile Name is comprised of one or more CIViC Variant Names along with the relationship between Variants. For more explanation visit the :doc:`Molecular Profiles Overview <../molecular_profiles/overview>`.  

Adding New Molecular Profile Names
----------------------------------
New CIViC Molecular Profile Names are entered into the database at the first instance of curation of evidence for the given molecular profile. At the time of entering an Evidence Item for a new molecular profile, the name is automatally generated from the specific variant components. For a simple molecular profile this only requires finding a single gene and then finding (or creating) the variant name. For a complex molecular profile each gene/variant is found individually and then an expression is constructed which describes the relationship between variants. These relationships are specified with boolean operators (AND, OR, NOT) and parentheses to express arbitrarily complex relationships. Upon creation, the molecular profile components are re-ordered (alpha-numerically) to prevent creation of duplicates Molecular Profiles.

Curating Molecular Profile Names
--------------------------------
Curators should strive for the shortest and most intuitive representation of the Molecular Profile. Aliases that provide common short-hand, abbreviations or alternate expressions of the Molecular Profile are encouraged. 

