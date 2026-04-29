---
description: Paginated list of inventory items
layout: schema
name: InventoryList
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
schema_file: json-schema/acuity-brands-inventory-list-schema.json
slug: acuity-brands-inventory-list
source_filename: acuity-brands-inventory-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/acuity-brands/acuity-brands-inventory-list-schema.json\",\n  \"title\": \"InventoryList\",\n  \"description\": \"Paginated list of inventory items\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InventoryItem\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 5000\n    },\n    \"cursor\": {\n      \"type\": \"string\",\n      \"example\": \"eyJwYWdlIjoyfQ==\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/json-schema/acuity-brands-inventory-list-schema.json
tags: []
title: InventoryList
---
