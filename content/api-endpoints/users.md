---
title: "Users"
date: 2022-08-29T13:49:31+03:00
draft: false
weight: 34
---

## Endpoints

### Users

| Route | Description | getByLimit Support | getByIndex Support | Example |
|---|---|---|---|---|
| /api/v1/users/ | returns all users | ✔  |  |  |
|  /api/v1/users/:permission-group | returns users by permission group |  |  | /api/v1/users/member |
| /api/v1/users/:property-key/:property-value/  | returns users depending on a property key and value | ✔ |  | /api/v1/users/email/example@localhost.test |

{{< hint type=note icon=gdoc_info_outline title="Available property keys" >}}
Currently available property keys for users, `username`,`email` and `permission_group`
{{< /hint >}}
