---
title: Manager Assistant
description: Authorize a member of the organization as Manager Assistant to maintain member accounts and subordinate organizations on behalf of the person in charge
weight: 2
---

# Function Overview

The person in charge of an organization usually has to maintain the member accounts of the organization (add members, modify information, reset passwords, disable accounts, etc.). When the person in charge is on a business trip, on leave or busy with other things, one member of the organization can be designated to handle these tasks instead. That designated member is the **Manager Assistant**.

- **Person in charge**: the account automatically created by the platform when the organization is created. It is the highest administrator of the organization, and an organization has only one person in charge.
- **Manager Assistant**: a delegate designated by the person in charge from the **members of the organization**, who can manage the members and organization information of this organization and its subordinate organizations in **Organizational Structure** on behalf of the person in charge.

All screenshots in this article can be clicked to view the full-size image.

Before starting, please distinguish three things that are easy to confuse:

1. **Manager Assistant is not a role.** It does not appear in the selectable options of **Role**; it is a separate identity. After authorization, a yellow **Manager Assistant** tag is added to the Role column of the member list.
2. **Manager Assistant does not expand the data scope.** The assistant can still only see the plants and devices within their own data permissions. The assistant identity only adds management operations in **Organizational Structure**.
3. **Only the person in charge can grant and revoke it.** The assistant cannot see the **Manager Assistant** tab and cannot authorize anyone else.

## 1. What can and cannot be done

| Operation | Manager Assistant |
| --- | --- |
| View the organizational structure | Yes, within the organization the assistant belongs to and its subordinate organizations |
| Add members, modify member information, enable/disable accounts, reset passwords | Yes, limited to members of this organization and its subordinate organizations |
| Transfer members, delete members | Yes, but the person in charge of an organization cannot be transferred or deleted |
| Create a subordinate organization | Yes |
| Modify, transfer, delete subordinate organizations | Yes |
| Modify the organization information of the assistant's own organization | No |
| Operate the person in charge or other Manager Assistants of the organization | No |
| Grant or revoke Manager Assistant | No, the tab is not visible to the assistant |
| See more plant or device data | No, the data permissions are not expanded by the assistant identity |

> Note: the operation permissions of the assistant in **Organizational Structure** are basically the same as those of the person in charge, but the "No" items above are hard limits; the corresponding buttons are greyed out or not shown at all.
>
> Whether the **Measurement Group** tab is visible and whether the assistant can maintain measurement groups is decided by the member's own role and is not affected by the Manager Assistant identity.

## 2. Preparation before authorization

Check the following items one by one before authorization. If any item is not met, the authorization will fail or the member will not see the menu after logging in:

1. **Log in with the account of the person in charge of the organization**. Assistants and ordinary members have no authorization entry.
2. **The designated member is already a member of this organization**. A Manager Assistant can only be selected from the **members of this organization**; members of subordinate organizations cannot be authorized directly.
3. **The role of the designated member includes the menu permission of Organizational Structure**. This is the step most often missed:
   - The person in charge can go to **Member List → Modify → Role** and select a role that already includes the **Organizational Structure** menu permission for this member (the person in charge can only select roles they own);
   - If there is no such role among the selectable ones, please contact the platform administrator: select the **Organization management → Organizational Structure** menu for the role in role management, or let the administrator assign a suitable role directly.
   - The authorization dialog also reminds you of this: **you need to manually assign a role that includes the Organization module menu permission**.
4. **The person in charge cannot set themselves as an assistant**. The person in charge does not appear in the drop-down list.

## 3. Grant Manager Assistant

### 3.1 Open the "Manager Assistant" tab

1. Log in to the Solarhub Web platform.
2. Click **Organization management → Organizational Structure** in the left menu.
3. Click **Manager Assistant** in the tab bar on the right.

<a href="../../../../photo/docs/organization/assistant-tab.webp" target="_blank" rel="noopener"><img src="../../../../photo/docs/organization/assistant-tab.webp"></a>

> Note: the **Manager Assistant** tab is **only visible to the person in charge of the organization**. If you cannot see this tab, the current account is not the person in charge, or you have already been set as an assistant (an assistant cannot manage assistants).

> This tab always manages **the organization you belong to** and does not follow the organization tree on the left. That is, even if a subordinate organization is selected on the left, the list here still shows the assistants of your own organization.

### 3.2 Select a member and grant

1. Click the **Select a member of this organization** drop-down.
2. Search by the member's name, user name or email (the drop-down item is shown as "Name (User Name)"), then select the member.
3. Click the **Grant Assistant** button on the right.

<a href="../../../../photo/docs/organization/assistant-select.webp" target="_blank" rel="noopener"><img src="../../../../photo/docs/organization/assistant-select.webp"></a>

> The drop-down only lists members of this organization who are **not yet assistants**; the person in charge is not shown. Members who have already been authorized no longer appear in the candidates.

### 3.3 Confirm the authorization

1. A confirmation dialog appears with the text "Set the user as the manager assistant? (Note: you need to manually assign a role that includes the Organization module menu permission)".
2. Check that the member is correct and click **OK**; click **Cancel** to give up.

<a href="../../../../photo/docs/organization/assistant-confirm.webp" target="_blank" rel="noopener"><img src="../../../../photo/docs/organization/assistant-confirm.webp"></a>

### 3.4 Authorization successful

The page shows "Successful Operation" at the top, and the member appears in the list of the **Manager Assistant** tab, showing user name, name, role, email and phone number.

<a href="../../../../photo/docs/organization/assistant-success.webp" target="_blank" rel="noopener"><img src="../../../../photo/docs/organization/assistant-success.webp"></a>

> After granting or revoking, the platform clears the login session of the member. Please tell the member to **log in again** so that the new identity takes effect; if the member is using the platform at that moment, they will be forced to log out, so it is better to inform them in advance.

## 4. How to confirm after authorization

After authorization, you can confirm it in two places:

### 4.1 The "Manager Assistant" tab

If the member appears in the list of the **Manager Assistant** tab, the authorization has taken effect. The **Revoke** button on the right of the row is used to revoke the authorization; see the next section.

### 4.2 The tag in the "Member List"

Switch to the **Member List** tab; a yellow **Manager Assistant** tag is added to the Role column of that member's row. The original role tags are still kept, which means the assistant identity is added on top of the original roles and does not replace them.

<a href="../../../../photo/docs/organization/assistant-tag.webp" target="_blank" rel="noopener"><img src="../../../../photo/docs/organization/assistant-tag.webp"></a>

If the member still cannot see the **Organization management** menu after logging in again, it is usually because **the role lacks the Organizational Structure menu permission**. Handling:

1. Find the member in the **Member List** and click **Modify** in the Operation column.
2. In the **Member Information Modified** panel, find **Role** and select a role that includes the **Organizational Structure** menu permission (the figure below is an example; the actual role names depend on the platform configuration).
3. Click **Save**, then ask the member to log in again.

<a href="../../../../photo/docs/organization/assistant-role.webp" target="_blank" rel="noopener"><img src="../../../../photo/docs/organization/assistant-role.webp" width="600" height="777"></a>

> Modifying the role only affects menus and operation permissions and does not revoke the Manager Assistant identity. After saving, both the role tags and the yellow **Manager Assistant** tag are shown in the member list.

## 5. Revoke Manager Assistant

When the member no longer needs to handle these tasks, the person in charge revokes the assistant identity:

1. Go to the **Organization management → Organizational Structure → Manager Assistant** tab.
2. Find the member in the list and click **Revoke** in the Operation column.

<a href="../../../../photo/docs/organization/assistant-revoke.webp" target="_blank" rel="noopener"><img src="../../../../photo/docs/organization/assistant-revoke.webp"></a>

3. Click **OK** in the confirmation dialog. After the page shows the operation succeeded, the **Manager Assistant** tag of the member disappears.

After revocation:

- The member is still a normal member of the organization and **will not be deleted**; the original roles, measurement groups and data permissions remain unchanged;
- The member immediately loses the management operations in the organizational structure;
- The platform clears the login session of the member, and the change takes effect after logging in again.

## 6. FAQ

**Q1: I cannot see the "Manager Assistant" tab in "Organizational Structure"?**

Only the person in charge of the organization can see it. Please confirm that the current account is the person in charge of the organization; if you are the assistant yourself, you cannot see the tab.

**Q2: The member to be authorized cannot be found in the drop-down?**

Please confirm: ① the member belongs to this organization, not a subordinate organization; ② the member is not yet a Manager Assistant; ③ the member is not the person in charge. In any of these cases the member does not appear in the candidate list.

**Q3: The authorization succeeded, but the member cannot see the "Organization management" menu after logging in?**

The assistant identity only decides **whether the member can manage the organization**; whether the menu is visible also depends on the role. Please assign a role that includes the **Organizational Structure** menu permission to the member as described in section 4.2, then ask the member to log in again.

**Q4: Can a Manager Assistant see more plant or device data?**

No. The assistant identity does not change the data permissions; the plants, devices and parameters the member sees are still decided by their own data permissions, roles and measurement groups.

**Q5: Can an assistant authorize other people as assistants?**

No. Only the person in charge can grant or revoke an assistant, and the assistant cannot see the **Manager Assistant** tab.

**Q6: Does the assistant identity remain after the assistant is transferred to another organization?**

No. The assistant identity is bound to the original organization and is automatically removed when the member is transferred to another organization; the person in charge of the new organization needs to authorize it again.

**Q7: Does revoking the assistant delete the member?**

No. Revocation only clears the **Manager Assistant** identity; the member account, roles and permissions are kept.

## 7. Notes

- Both granting and revoking force the target member to **log out and log in again**. Please inform the member in advance so that they are not interrupted during an operation.
- An organization can have multiple Manager Assistants. Please grant according to actual needs to avoid spreading permissions.
- The person in charge of an organization cannot be deleted or transferred; the account is only cleaned up together with the organization. The assistant also cannot operate the person in charge of the organization.
- When adding or modifying members, the assistant can only grant the roles and measurement groups they own and cannot grant anything beyond their own permission scope.
