---
title: "Entries"
date: 2022-08-29T12:56:41+03:00
draft: false
weight: 32
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

{{< hint type=note icon=gdoc_info_outline title="Property keys and their values" >}}
Property keys are changes depending on entry types and their fields that you added. Each field name is property key and its value is property value.
{{< /hint >}}

### Entries

| Route | Description | getByLimit Support | getByIndex Support | Example |
|---|---|---|---|---|
| /api/v1/entries |  returns all entries | ✔ |  |  |
| /api/v1/entries/:namespace | returns entries by namespace | ✔ |  | /api/v1/entries/articles.books.history |

### Entry

| Route | Description | getByLimit Support | getByIndex Support | Example |
|---|---|---|---|---|
| /api/v1/entry/:slug  | returns an entry by slug |  |  | /api/v1/entry/why-should-you-read-books |
| /api/v1/entry/:property-key/:property-value | returns entries depending on a property key and value |  ✔|  ✔|  /api/v1/entry/published/true |
