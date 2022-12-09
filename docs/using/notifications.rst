Notifications & Mentions
========================

CIViC provides a notification system that helps users track updates to monitored entities, and mentions of their username within comments. Editors and admins can also be prompted to view specific comments by utilizing special :ref:`comment macros<comment-macros>`.

Notifications Page
------------------
Notifications and mentions are displayed in the Account page, under the Notifications tab. To view the Account section, click the arrow next to your user button at the top right of the header. Then click on the My Account link near the bottom of the dropdown that will appear. The Notifications page will be displayed.

The Notifications page consists of a notification list and a sidebar that enables viewing by notification category and filtering by username. Notification categories include:

.. list-table::
   :widths: 30 70
   :header-rows: 0

   * - Subscribed Events
     - Notifications from subscribed entities, whenever that entity or sub-entity is modified or commented upon.
   * - Mentions
     - Notifications from commentors using the @[username] or @[editor/admin] macro
   * - System Updates
     - Placeholder for notifications from a future system that will show CIViC software update details
   * - Messages
     - Placeholder for notifications from a future internal messaging system
 
Entity Notifications
--------------------
Users are automatically subscribed to notifications for an entity if they add or suggest changes to it. When a user is subscribed to an entity, they will receive notifications for all activity related to that entity and its children: suggested changes submitted/accepted/rejected, comments made, sub-entities added.

Notifications will also be generated for activity related to child entities, so a subscription to a variant will also include notifications for all evidence associated with that variant.

Editor and Admin Mentions
-------------------------
:ref:`Comment macros<comment-macros>` enable mentioning specific users, or all admins/editors. When ``@janesmith`` is included in a comment, then the user ``janesmith`` will receive a notification allowing her to visit and read that specific comment. If ``@editors`` or ``@admins`` is included in a comment, then all editors or admins will receive a notification, allowing them to easily view that specific comment. These mentions will appear in the Mentions category of a user's notifications.



