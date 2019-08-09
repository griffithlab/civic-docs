Users and Groups
================

CIViC depends on its users, organized into roles and groups, to add to its knowledgebase and curate its content. This section details how to create a new user account, user account are management, and various other features related to users and groups.

User Creation
-------------
CIViC account creation and authentication uses Open Authentication (OAuth), which delegates authentication to third-party services. This allows CIViC to provide quick one-click account creation, as long as new users have an account on our supported OAuth providers. Currently, these providers are GMail, ORCHID, and GitHub. Ensure that you have an account with one of these services before creating a new CIViC account.

To create a new user, click the 'Sign In/Sign Up' button located at the top right corner of the header area. A sign-up window will appear, prompting a choice between the three services that we support. After clicking on your preferred authentication service provider, you'll be redirected to its login page to provide your credentials (these will not be transmitted to CIViC). After logging in, you'll be asked to give permission to provide CIViC your username. GMail users will also be asked permission to provide CIViC your email address. If you are currently logged into the service, it may skip the login screen and take you directly to the permissions screen.

You'll then be returned to CIViC, logged in with a new curator account.

User Roles
----------
CIViC users have one of three roles: curator, editor and admin. Curators may submit evidence, assertions, and source suggestions. They may also submit suggested changes to all entities. Editors may do everything that curators do, plus approve and reject items submitted by curators. Admins have access to the CIViC server admin console and may crate/modify users, groups, and other administrative tasks available only via the admin console.


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
