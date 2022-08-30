---
title: "Overview"
date: 2022-08-26T15:40:03+03:00
draft: false
weight: 11
---

## What is simpl:api ?

simpl:api is a basic API builder that allows users to build an API easily for their front-end application or website. The main focus of this project is small applications and websites but also can be used for micro applications in large systems.

There are 5 key parts of the system. Let's take a glance at them one by one:

### Entry Types

Entry types are like classes that you give a shape in your hand. You can set its name, design its fields(object properties) as you want. For example; you can create '`Animals`' entry type and set '`weight`' and '`sex`' as its fields (properties) and you can restrict value type of '`weight`' as `integer` and its maximum length to `3` , similarly, you can set value type of '`sex`' as string and limit its length to `6`.

### Entries

If you think of entry types as classes, entries are objects that are derived from those classes. How you can write an entry is dependent on the structure of its entry type. Let's continue with '`Animals`' example, we want to register an '`Animal`' to database. what we can enter is only limited to `entry name`, `weight`, and `sex`. Of course, weight must be `integer` and its maximum length is `3` and `sex` must be `string` and its maximum length is `6`.

### Users

Users are designed to use the dashboard. To use API, you don't need a user account. Each user has a permission group (user group) which can be restricted their permissions.

### Permission Groups

Permission groups designed to limit permissions of users depending on necessities and use cases. `Admin` is special permission group which have exclusive permissions that cannot be changed whitout editing the code. Other permission group's can be restricted by `namespace` (entry types). Privileges that can be restricted are `Create`,`Read`,`Update`,`Delete`.

### Settings

Settings allows you to change privileges of each permission group and generate or remove API keys. Settings can only be accessed through dashboard and only admins can access this page.
