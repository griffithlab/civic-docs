Users
=====

CIViC depends on its users to add to its knowledgebase and curate its content. This section details how to create a new user account, user account management, and various other features related to users and organizations.

User Creation
-------------
CIViC account creation and authentication uses Open Authentication (OAuth), which delegates authentication to third-party services. This allows CIViC to provide quick one-click account creation, as long as new users have an account on our supported OAuth providers. Currently, these providers are GMail, ORCHID, and Github. Ensure that you have an account with one of these services before creating a new CIViC account.

To create a new user, click the 'Sign In/Sign Up' button located at the top right corner of the header area. A sign-up window will appear, prompting a choice between the three services that we support. After clicking on your preferred authentication service provider, you'll be redirected to its login page to provide your credentials (these will NOT be transmitted to CIViC). After logging in, you will be asked to give permission to provide CIViC your username. GMail users will also be asked permission to provide CIViC your email address. If you are currently logged into the service, it may skip the login screen and take you directly to the permissions screen.

You will then be returned to CIViC, logged in with a new curator account.

User Roles
----------
CIViC users have one of three roles: curator, editor and admin. Curators may submit evidence, assertions, and source suggestions. They may also submit suggested changes to all entities. Editors may do everything that curators do, plus approve and reject items submitted by curators. Administrators have access to the CIViC server admin console and may crate/modify users, organizations, and other administrative tasks available only via the admin console.


.. list-table::
   :header-rows: 1

   * - Role
     - | Submit
       | Evidence,
       | Assertions,
       | Sources
     - | Submit
       | Suggested
       | Changes
     - | Approve
       | Submissions
     - | Approve
       | Suggested
       | Changes
     - | Edit
       | Database
       | Records
   * - Curator
     - |check|
     - |check|
     - |times|
     - |times|
     - |times|
   * - Editor
     - |check|
     - |check|
     - |check|
     - |check|
     - |times|
   * - Administrator
     - |check|
     - |check|
     - |check|
     - |check|
     - |check|

Currently, Curators are only elevated to Editor roles via invitation.

User Details
------------
Users have a default display name, based on the username provided by the OAuth method used to create the account. Additional fields are also included to allow users to provide more information about themselves to the CIViC community. These details are displayed on the user's profile page and on their user cards.

.. list-table::
   :header-rows: 1

   * - Field
     - Description
   * - Name
     - User's full name
   * - User Name
     - Short nickname that will appear on user buttons and throughout the user interface. This is initially generated from the username provided by the OAuth provider used to initially login to CIViC.
   * - Email Address
     - User's email address. The address will not be public and will only be used for sending CIViC notifications and updates.
   * - Areas of Expertise
     - One of three target user roles: Patient Advocate, Clinical Scientist, and Research Scientist
   * - ORCID
     - Open Research and Contributor ID
   * - Personal Website
     - A link to a user's personal website
   * - Biography
     - A short biography of the user, ideally including professional qualifications for performing CIViC curation.
   * - Country
     - User's primary country of residence/research.
   * - Twitter, Facebook and Linkedin Handles
     - User's social media nicknames, used to display a link to their social media pages on their profile and user cards.

Viewing Users
-------------
Throughout the CIViC interface, users are displayed in three ways: user buttons, user cards, and the user profile.

.. thumbnail:: /images/figures/user-elements.png
   :alt: Screenshot of an example user profile
   :title: Example user profile
   :show_caption: True

|

User buttons appear where we need to indicate a user where space is limited, primarily on CIViC entity summaries' activity histories. User cards are shown when more space is available to display more info about a user. And the profile page shows all public information on an individual user. Clicking on a user button, or the user avatar on the cards will take you to the user's page. 
 
Finding Users
-------------
`The Contributors section <https://civicdb.org/users/>`_ of the application displays a list of users that can be filtered by display name, organization, role, or recent activity date:

.. thumbnail:: /images/figures/community-user-search.png
   :alt: Screenshot of the CIViC contributors grid view
   :title: Contributors view
   :show_caption: True

|

Locate users of interest by filtering by display name, organization, role, area of expertise. Sorting and time-limit options are also provided. 

