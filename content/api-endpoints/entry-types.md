---
title: "Entry Types"
date: 2022-08-25T02:49:37+03:00
draft: false
weight: 31
---

## Endpoints

{{< hint type=note icon=gdoc_info_outline title="Namespaces" >}}
Namespaces are hierarchical representation of entry types. For example, articles.books means books entry type is child of articles entry types.
{{< /hint >}}

{{< hint type=note icon=gdoc_info_outline title="getByLimit and getByLimit Support" >}}
getByLimit support means you can add `/first_X`, `/last_X` or `/random_X` to end of the url to get first, last or random X results.
getByIndex support means you can add `/X` to end of the url to get Xth result.
X is Integer.
{{< /hint >}}

### Entry Types
| Route | Description | getByLimit Support | getByIndex Support | Example |
|---|---|---|---|---|
| /api/v1/entry-types | returns all entry types  |  ✔|  |  |
| /api/v1/entry-types/:namespace  | returns entry types by namespace |  |  | /api/v1/entry-types/articles.books.history |
| /api/v1/entry-types/:namespace-part-1/:namespace-part-2/... | returns entry types by namespace but separated each part of namespace |  ✔|  | /api/v1/entry-types/articles/books/history |

### Entry Type
| Route | Description | getByLimit Support | getByIndex Support | Example |
|---|---|---|---|---|
| /api/v1/entry-type/:namespace | returns an entry type by namespace |  |  | /api/v1/entry-type/articles.books.history |
| /api/v1/entry-type/:namespace-part-1/:namespace-part-2/...  | returns an entry type by namespace but separated each part of namespace |  |  | /api/v1/entry-type/articles/books/history |
| /api/v1/entry-type/slug/:slug | returns an entry type by slug |  |  | /api/v1/entry-type/slug/history |
| /api/v1/entry-type/id/:_id (mongodb id) |returns an entry type by id |  |  | /api/v1/entry-type/id/12e41h5ff17dd2aeb9e0a89 |
