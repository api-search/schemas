---
description: SearchResultSet schema from Backstage search API
layout: schema
name: SearchResultSet
properties_list:
- description: Array of search result documents.
  name: results
  type: array
- description: Cursor to fetch the next page of results.
  name: nextPageCursor
  type: string
- description: Cursor to fetch the previous page of results.
  name: previousPageCursor
  type: string
- description: Total number of matching results.
  name: numberOfResults
  type: integer
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/search-search-result-set-schema.json
slug: search-search-result-set
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: SearchResultSet
---
