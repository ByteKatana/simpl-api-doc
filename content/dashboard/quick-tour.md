---
title: "Quick Tour"
date: 2022-08-29T14:28:25+03:00
draft: false
weight: 41
---

Let's take a quick tour of the dashboard and see what's there

### Entry Types

Entry types are like classes in programming which you can design its structure. While you create an entry type, you can add as many field as you like and set their form type and value type.

![new entry type](/simpl-api-doc/img/entry-type-create.png)

Once you create the entry type, you have to give permissions to permission groups depending on your use case. You can do this on the settings page.

![settings permissions](/simpl-api-doc/img/settings-give-perm.png)

After giving permissions, you can go back to entry types page and click to `Create Entry` button to create new entry for articles entry type.
![entry types create new entry](/simpl-api-doc/img/entry-types-new-entry.png)

### Entries

Entries are like objects in programming which created from classes (entry types in our case). You have to abide structure of the entry type that you going to create entry, otherwise it will give an error under the field.

![new entry](/simpl-api-doc/img/new-entry-articles.png)

### Users

You can manage users from `Users` page. Only admins have edit and delete permissions.

![user management](/simpl-api-doc/img/users-mngnt.png)

### Permission Groups

Permission groups are basically user groups that allows you limit each groups permission depending on your use case. Only admins can access `Permission Groups` page and can create, edit and delete a permission group. By default, there are two permission group which are `Admin` and `Member`. Also each permission group has no any privilege by default but admins has some exceptional privileges which cannot be removed without editing the code.

![permission groups](/simpl-api-doc/img/perm-groups.png)

### Settings

Settings page allows you manage privileges of each permission group and create or delete API keys.

#### Permissions

- **Read** : Doesn't do anything in dashboard but you can use it in your front-end application.
- **Create** : This permission allows a permission group to create an entry for selected namespace (entry type)
- **Update** : This permission allows a permission group to update selected namespace and its entries.
- **Delete** : This permission allows a permission group to delete selected namespace and its entries.

#### Admin Exclusive Permissions

- Creating, Editing, deleting users
- Accessing `Permission Groups` page
- Creating, Editing and deleting a permission group
- Accessing `Settings` page

![settings page](/simpl-api-doc/img/settings-page.png)
