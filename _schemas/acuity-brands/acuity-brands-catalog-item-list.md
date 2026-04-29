---
description: Paginated list of catalog items
layout: schema
name: CatalogItemList
properties_list:
- description: ''
  name: items
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: cursor
  type: string
provider_name: acuity-brands
provider_slug: acuity-brands
schema_file: json-schema/acuity-brands-catalog-item-list-schema.json
slug: acuity-brands-catalog-item-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/acuity-brands/acuity-brands-catalog-item-list-schema.json\",\n  \"title\": \"CatalogItemList\",\n  \"description\": \"Paginated list of catalog items\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CatalogItem\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 50000\n    },\n    \"cursor\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/json-schema/acuity-brands-catalog-item-list-schema.json
tags: []
title: CatalogItemList
---
