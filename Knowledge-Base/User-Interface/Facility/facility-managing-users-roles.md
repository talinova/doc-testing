---
title: "Managing Users And Roles In Facility View"
tags: getting-started, savi, facility, ui, users, roles
date:
  created: "03/21/2022"
  modified: "09/13/2022"
description: Users and roles are how end-users access Facility View to control the project. Add each user to one or more roles. Each role has permission settings for every scene and endpoint in the project.
---

# Managing Users And Roles In Facility View


## Managing Users
<a href="../../../Assets/Knowledge-Base/User-Interface/Facility/users.png">
  <img src="../../../Assets/Knowledge-Base/User-Interface/Facility/users.png" alt="New user modal" width="700" height="">
</a>

Managing users is a big part of SAVI 3. Built on the idea of giving control to end users and staff, SAVI 3 has an extensive, but straight forward, Role system. Each user can be assigned one or more Roles. Each Role can be assigned one or more Scenes as well as have specific permissions for each device. When multiple Roles or other permissions cause a conflict, the highest permissions for each are inherited.

>***Note: A Scene can be made more restrictive with permissions but not less so (i.e., granting control of a display that is not normally part of a scene will not allow that display to be viewable or controllable in that scene).***

### Creating a New User
<a href="../../../Assets/Knowledge-Base/User-Interface/Facility/new-user-modal.png">
  <img src="../../../Assets/Knowledge-Base/User-Interface/Facility/new-user-modal.png" alt="New user modal" width="300" height="">
</a>

1. Click the **New User** button to open the modal [![new user button](../../../Assets/Knowledge-Base/User-Interface/Facility/new-user-button.png)](../../../Assets/Knowledge-Base/User-Interface/Facility/new-user-button.png)

2. Fill in the users name (Optional).
3. Assign the user a Username (Required).
4. Create a Password (Required).
5. Set an Email (Recommended).
6. Click **Create**.


## Managing Roles
<a href="../../../Assets/Knowledge-Base/User-Interface/Facility/user-roles.png">
  <img src="../../../Assets/Knowledge-Base/User-Interface/Facility/user-roles.png" alt="Facility View user roles" width="700" height="">
</a>

When assigning or editing Roles, there is no saving required. Simply select the user and check any Role you wish to give them. In the Role tab, you can change settings and they update in real-time.

To create a new Role, simply select the **New Role** button and give it a name. The new Role will appear in the list on the left. [![new role button](../../../Assets/Knowledge-Base/User-Interface/Facility/new-role-button.png)](../../../Assets/Knowledge-Base/User-Interface/Facility/new-role-button.png)

### Editing a Role

1. Ensure you are on the Role tab by selecting it from the top left.
2. Select the Role from the list on the left or search for it using the search bar.
3. Select which Scenes are available to that Role.
4. Move down the list, selecting if each device or group of devices is viewable, controllable, or completely hidden.
    * **Hidden:** Devices will not appear at all in Facility View.
    * **View:** Devices will appear in Facility View but will not be controllable.
    * **Control:** Devices will appear in Facility View and will have full control.
