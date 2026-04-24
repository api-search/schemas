---
description: SearchResult schema from Backstage search API
layout: schema
name: SearchResult
properties_list:
- description: The document type (e.g., software-catalog, techdocs).
  name: type
  type: string
- description: ''
  name: document
  type: object
- description: Relevance rank of the result.
  name: rank
  type: number
- description: ''
  name: highlight
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/search-search-result-schema.json
slug: search-search-result
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: SearchResult
---
