**Settings for all mailing lists on lists.camaraproject.org (API Sub Projects & Sandboxes, Working Groups, (public) TSC, EUC, ...), except the ones listed later:**

* Group Email Address: _Provide a speaking email address (avoid abbreviations if possible), use "sp-" prefix for Sub Projects, "sb-" prefix for Sandboxes independent from Sub Projects, and „wg-“ prefix for Working Groups_
* Group Description: _Provide a speaking description_
* Privacy:
  * Visibility: Group list in parent group, publicly viewable messages
  * Member List Visibility: All owners, and moderators with the correct permissions
  * Email Address Visibility in Archive: Mask email address in the web archive
* Group Type and Moderation:
  * Restricted Membership: No
  * Announcement-Only Group: No
  * Message Moderation: Messages are not moderated.
  * New Members Moderation: Yes
  * Unmoderated after: 1 approved message
* Message Policies:
  * Allow Nonmembers to Post: no
  * Allow Parent Members to Post: yes _(note: parent of all subgroups is "main")_

**The following groups have specific settings (only the differences to above settings are listed):**

For "**board**" + "**tsc-private**":
* Privacy:
  * Visibility: Group not listed in parent group, messages viewable by subgroup members only
* Group Type and Moderation:
  * Restricted Membership: Yes
  * New Members Moderation: No
* Message Policies:
  * Allow Parent Members to Post: no

For "**codeowners**":
* Group Type and Moderation:
  * Restricted Membership: Yes
  * New Members Moderation: No
* Message Policies:
  * Allow Parent Members to Post: no

For "**all**":
* Group Type and Moderation:
  * Message Moderation: All Messages Moderated
  * New Members Moderated: Yes
  * Unmoderate After: Not enabled

For "**adm**":
* Group Type and Moderation:
  * Restricted Membership: Yes _(NOTE: only administrators of CAMARA are members of the group)_
  * New Members Moderation: No
* Message policies: 
  * Allow Nonmembers to Post: yes _(Messages from nonmembers messages will be moderated instead of rejected)_

For "**main**":
* Announcement-Only Group: Yes
