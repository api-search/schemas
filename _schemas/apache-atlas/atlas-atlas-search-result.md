---
description: Result of a search query against the Atlas metadata repository.
layout: schema
name: AtlasSearchResult
properties_list:
- description: Type of search query executed.
  name: queryType
  type: string
- description: The search parameters that were used.
  name: searchParameters
  type: object
- description: List of matching entity headers.
  name: entities
  type: array
- description: Approximate total count of matching entities.
  name: approximateCount
  type: integer
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-search-result-schema.json
slug: atlas-atlas-search-result
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasSearchResult
---
