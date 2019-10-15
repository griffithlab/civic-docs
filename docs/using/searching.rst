Searching
=========

CIViC provides a couple methods for searching its knowledgebase: the Quick Search bar available on all pages, and a more extensive advanced search available on the Search page.

Quick Search
------------
The quick search bar is located on every page of CIViC. On the home page it is found here:

.. image:: /images/figures/quick-search_header.png

And on all sub-pages it may be found here:

.. image:: /images/figures/quick-search_subheader.png

Any text typed into the quick search box will be matched against Gene and Variant names. Search results displayed beneath the entry box may be navigated using the arrow keys. Navigate to a selected entity by pressing the Return or Tab key.

.. image:: /images/figures/quick-search_results.png

Advanced Search
---------------
CIViC provides a method for performing complex searches for all of its major entities: Evidence, Assertions, Genes, Variants, and Sources. Click on the Search button, available on all CIViC pages, to load this advanced search interface.

.. image:: /images/figures/advanced-search.png

Tabs at the top of the interface switch between search interfaces for CIViC's major entities **(A)**. Example search buttons **(B)**, pre-populate the query builder with a variety of examples intended to showcase how users may build their own searches. Click on these to get an idea of the kinds of queries that can be constructed.

The the main query builder interface **(C-J)** allows users to specify a precise description of the results they wish to see, by building queries of the entity's attributes.

The match criteria selector **(C)** switches between using **ALL** or **ANY** of the attributes specified when performing a search. When 'all' is selected, then only results that match every attribute value the user specifies will be returned. If 'any' is selected then results will be returned if they match any of the user-specified values.

Queries are constructed by adding (or removing) entity attribute rows **(G)** using the add attribute and remove attribute buttons **(I)**. Upon initially loading the search interface, a single attribute row will be displayed. Choose an attribute of interest using the attribute selector **(D)**. Depending on the attribute, several additional form elements will be displayed **(E-F, H)**.

The second element in every attribute row **(E)** is a logical and comparison operator, allowing the user to choose how the specified value will match against existing records. These operators can include *contains/does not contain*, *is less/greater than*, *is between*, etc. Depending on the attribute type, the third form element will be a selector (for enumerated fields), a text box (for strings and numbers), or special components for certain fields, e.g. ratings **(H)**. If a range comparison operator is specified then two form fields will be provided to define the range **(H)**.

Once the query is specified by choosing attributes and providing values for all their form fields, pressing the Search button will send the query to the CIViC server. Results returned from the server are then displayed in a results table beneath the query builder. Each entity type has its own with columns relevant to its entity type.

Every unique search generates a new URL, e.g. https://civicdb.org/search/evidence/2d364b3c-0e9e-44a8-a01e-c936851c5662. This URL may be stored or sent to other users to reproduce the same search query and results in a different browser. This feature allows users to more easily discuss and share result sets relevant to their research.
