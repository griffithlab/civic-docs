.. _molecular-profile-name:

Name
====
The **Molecular Profile Name** describes the specific molecular profile being interpreted for clinical utility. Selecting a Molecular Profile Name in the Molecular Profile list for a Gene will bring up a Molecular Profile specific page with a Description, Aliases, Molecular Profile Score, details of underlying Variant(s) and associated Evidence Items. 
 

Understanding Molecular Profile Names
-------------------------------------
The Molecular Profile Name concisely describes the Gene/Variant components (and their relationships) which define the Molecular Profile. The Molecular Profile Name is comprised of one or more CIViC Variant Names along with the relationship between Variants. For more detailed explanation visit the :doc:`Molecular Profiles Overview <../molecular_profiles/overview>`.  

Adding New Molecular Profile Names
----------------------------------
New CIViC Molecular Profile Names are entered into the database at the first instance of curation of evidence for the given Molecular Profile. At the time of entering an Evidence Item for a new Molecular Profile, the Name is automatally generated from the specific Variant components. For a simple Molecular Profile this only requires finding a single Gene and then finding (or creating) the Variant Name. For a complex Molecular Profile each Gene/Variant is found individually and then an expression is constructed which describes the relationship between variants. These relationships are specified with boolean operators (AND, OR, NOT) and parentheses to express arbitrarily complex relationships. Upon creation, the Molecular Profile components are **re-ordered (alpha-numerically)** to prevent creation of duplicate Molecular Profiles.

Curating Molecular Profile Names
--------------------------------
Curators should strive for the shortest and most intuitive representation of the Molecular Profile. Aliases that provide common short-hand, abbreviations or alternate expressions of the Molecular Profile are encouraged. 

