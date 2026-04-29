---
description: ''
layout: schema
name: lookup_object
properties_list:
- description: The string or keyword being searched on. Concurrent searches for multiple patterns is NOT supported
  name: pattern
  type: string
- description: Asset class that is being searched against
  name: entities
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-id-lookup-lookup_object-schema.json
slug: factset-id-lookup-lookup_object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"lookup_object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pattern\": {\n      \"type\": \"string\",\n      \"description\": \"The string or keyword being searched on. Concurrent searches for multiple patterns is NOT supported\\n\"\n    },\n    \"entities\": {\n      \"type\": \"array\",\n      \"description\": \"Asset class that is being searched against\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-id-lookup-lookup_object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: lookup_object
---
