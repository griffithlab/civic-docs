.. role:: raw-html(raw)
   :format: html

Comments
========

Encouraging a transparent curation process is one of the goals of the CIViC knowledgebase. To that end, it is possible (and encouraged) to record relevant curation details, motivivations, questions for other curators or editors in the form of comments on primary CIViC entities.

Each CIViC entity capable of accepting suggested changes also includes a comment thread. These comments can be viewed by clicking on an entity's 'Talk' tab, then the middle 'Comments' tab that will appear beneath the entity summary. 

Initial Comments
----------------
The forms for adding new evidence or assertions includes a comment field, intended to include a note from the curator describing why the record should be included in CIViC. This comment will be displayed at the top of the comment thread. Note that this comment is not required so many records will not include an initial comment.

Creating Comments
-----------------
To create a comment, ensure you are logged in, navigate to the entity you wish to comment upon, click the entity's Talk tab, then the Comments tab. At the bottom of the page, there will be displayed a textarea in which you may enter your comment.

Above the comment area are two buttons, 'Compose' and 'Preview', with Compose being selected by default. Click Preview to see how your message will appear with all the formatting and links applied.

When you are satisfied with your comment, press 'Submit Comment', and your message will be immediately appended to the entity's comment thread.

Comment Formatting
~~~~~~~~~~~~~~~~~~
Emphasis, styling, images and links may be added to comments using a subset of Markdown syntax:

.. list-table::
   :widths: 20 80
   :header-rows: 1

   * - Effect
     - Syntax
   * - Headers
     - :raw-html:`<pre># This is an &lt;h1&gt; tag<br/>
       ## This is an &lt;h2&gt; tag<br/>
       ###### This is an &lt;h6&gt; tag</pre>`
   * - Emphasis
     - :raw-html:`<pre>*This text will be italic*
       _This will also be italic_<br/>
       **This text will be bold**
       __This will also be bold__<br/>
       *Italics and boldface **can be** combined*</pre>`
   * - Lists
     - :raw-html:`<strong>Ordered</strong>
       <pre>* Item 1
       * Item 2
       * Item 2a
       * Item 2b
       * Item 3</pre>
       <strong>Unordered</strong>
       <pre>1. Item 1
       2. Item 2
       3. Item 3
       * Item 3a
       * Item 3b</pre>`
   * - Images
     - :raw-html:`<pre>![this cool diagram](http://site.com/images/cool.png)<br/><br/>Format: ![Alt Text](url)</pre>`
   * - Blockquotes
     - :raw-html:`<pre>As Charles Darwin said:
       &gt;It is not the strongest
       &gt;of the species that survive,
       &gt;nor the most intelligent,
       &gt;but the one most responsive to change.</pre>`
   * - Inline code
     - :raw-html:`I think you should use an
       &#96;&lt;addr&gt;&#96; element here instead.`

Comment Macros
~~~~~~~~~~~~~~
Using macros, you may easily insert links to CIViC entities, mention and notify users.

.. rubric:: @username mention macro
'@' followed by a user's display name will be displayed as a link to the user's profile page, and generate a notification to the mentioned user. This is useful for calling a user's attention to a particular comment.

Type '@', and the first couple letters of a user's name, and CIViC will show you a dropdown menu of users with matching display names. Hit enter to insert an user mention link, which will display in the rendered comment as a link to the user's profile page, and generate a notification to the mentioned user.

.. rubric:: @admins and @editors mention macros
Adding '@admin' or '@editor' to your message will generate a mention notification for all users with the admin or editor role, respectively:

.. list-table::
   :widths: 100
   :header-rows: 0

   * - :raw-html:`<pre>Hey @admins, could I please get someone to approve this new evidence item?</pre>`

